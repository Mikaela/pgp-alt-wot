# pgp-alt-wot

PGP keys signed by me so I don't have to validate the same keys
again-and-again and can just trust my own paper verified fingerprint in the
subsequent validations.

WoT? [Web Of Trust](https://en.wikipedia.org/wiki/Web_of_trust)

* * * * *

Example use case for this repository is [Tor Browser](https://torproject.org/),
I need to download it on most of systems and I need to verify it and it's
painful to verify the PGP key all the time, while I can just verify my own
fingerprint from paper and see that it has signed the keys. I have done this
at least twice on Windowses first installing GPG through Chocolatey.

* * * * *

I don't know if there is point in putting down formal signing requirements,
but what has been my policy at the time of writing is:

NOTE: this section is written from memory so may be inaccurate

* friends - knowing for a long time through various connections and seeing
  at times seeing IDs (or visiting both directions) and otherwise having
  so deep relationship that lying about identity wouldn't be easily possible
* privacytools - confirmed from the people themselves, their websites,
  privacytools.io (WKD in git) and similar.
* software - used their verification instructions (of varying strength)
    * keepassxc.asc  mullvad.asc  tails.asc  tor-browser-developers.asc  yggdrasil.asc
    * keepassxc - checked their website through normal and Tor Browser
    * mullvad - checked their website and onion
    * tails - followed their verification instructions (including checking
      that it's signed by a Debian developer)
    * tor-browser - followed their checking instructions
    * yggdrasil - checked their website and comitted apt repo adding to git

* * * * *

TODO:

* add links to the previous section
* add OnionShare?
