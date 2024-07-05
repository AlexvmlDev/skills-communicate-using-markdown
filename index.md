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

## Adding a task list as example
### [1. Pre-installation](https://wiki.archlinux.org/title/Installation_guide#Pre-installation)
- [x] [1.1 - Acquire an installation image](https://wiki.archlinux.org/title/Installation_guide#Acquire_an_installation_image)
- [x] [1.2 - Verify signature](https://wiki.archlinux.org/title/Installation_guide#Verify_signature)
- [ ] [1.3 - Prepare an installation medium](https://wiki.archlinux.org/title/Installation_guide#Prepare_an_installation_medium)
- [ ] [1.4 - Boot the live environment](https://wiki.archlinux.org/title/Installation_guide#Boot_the_live_environment)
- [ ] [1.5 - Set the console keyboard layout and font](https://wiki.archlinux.org/title/Installation_guide#Set_the_console_keyboard_layout_and_font)
- [ ] [1.6 - Verify the boot mode](https://wiki.archlinux.org/title/Installation_guide#Verify_the_boot_mode)
- [ ] [1.7 - Connect to the internet](https://wiki.archlinux.org/title/Installation_guide#Connect_to_the_internet)
- [ ] [1.8 - Update the system clock](https://wiki.archlinux.org/title/Installation_guide#Update_the_system_clock)
- [ ] [1.9 - Partition the disk](https://wiki.archlinux.org/title/Installation_guide#Partition_the_disks)
  - [ ] [1.9.1 - Example layouts](https://wiki.archlinux.org/title/Installation_guide#Example_layouts)
- [ ] [1.10 - Format the partitions](https://wiki.archlinux.org/title/Installation_guide#Format_the_partitions)
- [ ] [1.11 - Mount the file systems](https://wiki.archlinux.org/title/Installation_guide#Mount_the_file_systems)

