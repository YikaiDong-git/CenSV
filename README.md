# CenSV

Interactive browser for centromeric structural variation.

<img src="docs/screenshot.jpg" alt="The CenSV browser opens with a password" width="490">

*The page as it appears before the password is entered.*

**CenSV** presents structural variants called inside human centromeric α-satellite
higher-order repeat arrays, positioned on the **T2T-CHM13 v2.0** assembly, together with the
molecular and disease associations reported for each. It is the companion browser to a
manuscript in preparation from the [Weinstock Lab](https://github.com/weinstocklab) at Emory
University.

## Browser

**https://yikaidong-git.github.io/CenSV/**

The whole browser is one self-contained page — the catalog, the annotations, the stylesheet
and the application encrypted into a single file and decrypted in your own browser. Once
loaded it runs entirely inside the tab, offline and stateless.

> **Access is restricted until publication.** The page opens with a password while the
> manuscript is in preparation; please contact the authors for it. This repository is public
> and its contents are ciphertext: the password opens every part of the file, the page's own
> text included. When the manuscript appears, the browser is republished open and the
> password retired.

Requires Chrome 80, Firefox 113 or Safari 16.4 or newer, and an `https://` address, since
browsers expose the decryption API in a secure context. A copy opened from a local folder
shows a message saying so.

## Contents

| | |
|---|---|
| `index.html` | the browser, encrypted with AES-256-GCM under a PBKDF2-HMAC-SHA256 key at 600,000 iterations |
| `docs/screenshot.jpg` | the page as it appears before the password is entered |
| `.nojekyll` | serves the file byte-for-byte through GitHub Pages |

Opening the page takes about a fifth of a second while the key is derived, once per browser
tab.

The source, the data pipeline, the verification suites and the deployment live in a companion
repository, published alongside this one when the manuscript appears.

## Cite

A citation will be added when the manuscript is published. Until then, please contact the
authors before referring to this resource.

## License

[MIT](LICENSE).
