# CenSV

An encrypted single-page browser. It needs a password.

**https://yikaidong-git.github.io/censv/**

The page is one file. The markup, the stylesheet, the application and the data are gzipped
into a single container and encrypted with AES-256-GCM under a PBKDF2-HMAC-SHA256 key at
600,000 iterations. There is nothing readable in this repository without the password, which
is not here and will not be — publishing the ciphertext is the point, not an oversight.

Opening it costs about a fifth of a second, once per tab. It needs a current browser and an
`https://` address, because browsers only expose decryption on a secure connection.

Companion to a manuscript in preparation. The source, the build and the checks live in a
private repository; this one holds the published artefact and nothing else.
