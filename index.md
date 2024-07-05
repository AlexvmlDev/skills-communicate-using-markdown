# This is an `<h1>` header, which is the largest
## This is an `<h2>` header
### This is an `<h3>` header
#### This is an `<h4>` header small
##### This is an `<h5>` header more small
###### This is an `<h6>` header, which is the smallest
#
## Adding an image
![I use Arch, BTW - Meme](https://i.postimg.cc/1zd2FBqK/btwiusearch.png)
#
## Adding a code example
### 1 Pre-installation
#### 1.1 Acquire an installation image

Visit the [Download](https://archlinux.org/download/) 🔗 page and, depending on how you want to boot, acquire the ISO file or a netboot image, and the respective [GnuPG](https://wiki.archlinux.org/title/GnuPG) signature.
#### 1.2 Verify signature

It is recommended to verify the image signature before use, especially when downloading from an HTTP mirror, where downloads are generally prone to be intercepted to [serve malicious images](https://www2.cs.arizona.edu/stork/packagemanagersecurity/attacks-on-package-managers.html).

On a system with [GnuPG](https://wiki.archlinux.org/title/GnuPG) installed, do this by downloading the ISO PGP signature ([under Checksums in the page Download](https://archlinux.org/download/#checksums)) to the ISO directory, and [verifying](https://wiki.archlinux.org/title/GnuPG#Verify_a_signature) it with:

```
$ gpg --keyserver-options auto-key-retrieve --verify archlinux-version-x86_64.iso.sig
```

Alternatively, from an existing Arch Linux installation run:

```
$ pacman-key -v archlinux-version-x86_64.iso.sig
```
#
***Note:***
- The signature itself could be manipulated if it is downloaded from a mirror site, instead of from [archlinux.org](https://archlinux.org/download/) as above. In this case, ensure that the public key, which is used to decode the signature, is signed by another, trustworthy key. The ```gpg``` command will output the fingerprint of the public key.
- Another method to verify the authenticity of the signature is to ensure that the public key's fingerprint is identical to the key fingerprint of the [Arch Linux developer](https://archlinux.org/people/developers/) who signed the ISO-file. See [Wikipedia:Public-key cryptography](https://en.wikipedia.org/wiki/Public-key_cryptography) for more information on the public-key process to authenticate keys.
#
