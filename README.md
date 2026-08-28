# CenSV

An encrypted, single-page browser. It needs a password.

**https://yikaidong-git.github.io/CenSV/**

The path is case-sensitive. `/censv/` is a 404, not a redirect.

## What is in this repository

One file that matters, `index.html`. The page markup, the stylesheet, the application and all
of its data are gzipped into a single container and encrypted with AES-256-GCM under a
PBKDF2-HMAC-SHA256 key at 600,000 iterations. Entering the password costs about a fifth of a
second, once per browser tab, and then the page is an ordinary interactive site with no
network calls of any kind.

Publishing the ciphertext is the design rather than an oversight. Nothing here is readable
without the password — not the data, and not the page's own text, which is inside the
encrypted container along with everything else. That is what lets the file be hosted in
public at all.

The password is not in this repository, in its history, or in any repository connected to it.

## If you have arrived here without one

This is not a puzzle and there is nothing to break. It is a companion browser to a manuscript
in preparation, shared ahead of publication with a small number of readers. When the
manuscript is published this will be republished open and unencrypted, and the password will
stop mattering.

## Requirements

A current browser — Chrome 80, Firefox 113 or Safari 16.4 and newer, all released in 2023 or
earlier — and an `https://` address. Browsers offer decryption only in a secure context, so a
copy saved and opened from a local folder cannot work; it will say so plainly rather than
render an empty page.

## What is not here

The source, the data pipeline and the checks that build this file live in a private
repository. This one holds the published artefact and is regenerated wholesale on each
update, so its history is not worth reading and issues or pull requests against it will not
reach anyone. For anything else, contact the repository owner.

All rights reserved. Please do not redistribute the file or its contents.
