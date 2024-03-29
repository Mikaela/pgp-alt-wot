# pgp-alt-wot

PGP keys signed by me so I don't have to validate the same keys
again-and-again and can just trust my own paper verified fingerprint in the
subsequent validations.

WoT? [Web Of Trust](https://en.wikipedia.org/wiki/Web_of_trust)

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Why?](#why)
- [Inclusion policy](#inclusion-policy)
- [Places to check for keys](#places-to-check-for-keys)
- [Mirrors](#mirrors)
- [See also](#see-also)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Why?

For example, I use [Tor Browser](https://torproject.org/) everywhere and
download it directly from their website. They have signed it using GPG (a
OpenPGP implementation) and to ensure it hasn't been tampered with, I have
to check that signature and I have two options:

- I can always [verify the signature](https://support.torproject.org/tbb/how-to-verify-signature/),
  but that takes time and I would need to verify it from both [support.torproject.org](https://support.torproject.org/tbb/how-to-verify-signature/)
  and [4bflp2c4tnynnbes.onion](http://4bflp2c4tnynnbes.onion/#how-to-verify-signature).
  But what if [they were compromised or I was under a MITM attack or lazy and verfied only one version](https://www.qubes-os.org/faq/#should-i-trust-this-website)?
- (or) I could verify the signing key carefully once, sign (or certify) it
  by myself and in the future simply verify that my own key is valid (as I
  have been doing this a few times on the other side of dualbooting and at
  family).

This second method is also [encouraged by Tails](https://tails.boum.org/install/expert/usb/index.en.html).

What if I am wrong and trust the wrong key? I think I am less likely to
trust a wrong key by verifying it carefully and signing it once than
verifying it separately every time. However if I do sign a wrong key, I can
always revoke my signature and then publish the key with my revocation
signature on public keyservers (which I don't usually do, while I cannot
control what people do with the signatures from this repository).

## Inclusion policy

- I am reasonably certain that the key belongs to whom it claims to belong
  to or I trust the key to belong to whomever it belongs to.
- I have some need of the key or have attended keysigning party with the
  key owner.
- `me/me.asc` is just my key and place where I try to keep all signatures it
  has received. Symlinks are legacy reasons and other me's are also me.

## Places to check for keys

- GitHub, Gitea and GitLab expose user public keys when you append a `.gpg`
  after their profile page (`.keys` for SSH).
- [The Internet Archive's Waybackmachine](https://web.archive.org/) is always
  a good place too especially when using together with official websites.
- Some people have similar projects or webpages for this purpose
  - [Artemis' verify page](https://artemislena.eu/services/verify.html)

## Mirrors

- main: [git.blesmrt.net/Mikaela/pgp-alt-wot](https://gitea.blesmrt.net/mikaela/pgp-alt-wot/)
- [git.piraattipuolue.fi/Mikaela/pgp-alt-wot](https://git.piraattipuolue.fi/mikaela/pgp-alt-wot)
- [git.com.de/Mikaela/pgp-alt-wot](https://git.com.de/mikaela/pgp-alt-wot) ([onion](http://gitea.qzzf2qcfbhievvs5nzkccuwddroipy62qjocqtmgcgh75vd6w57m7yad.onion/Mikaela/pgp-alt-wot))

## See also

- [Qubes OS: On Digital Signatures and Key Verification](https://www.qubes-os.org/security/verifying-signatures/)
- [Finnish Digital and Population Services Agency certificate search](https://dvv.fineid.fi/certificate-search)
  - S/MIME, not OpenPGP though
