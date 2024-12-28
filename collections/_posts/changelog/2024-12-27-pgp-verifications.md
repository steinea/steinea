---
layout: changelog
category: changelog
title: PGP Verifications
date: 2024-12-27
---

I claimed a few more identities using my [PGP](/pgp/) key and [Keyoxide](https://keyoxide.org/B5B0AA7ED4509C8B). This process can be quite fussy and documentation is sparse, so I will record what has worked for me here.

The first successful addition was an ORCID claim. To do so, I followed the steps to [add an identity claim](https://docs.keyoxide.org/openpgp-profiles/gnupg/#Adding_an_identity_claim):

* <code>gpg --edit-key FINGERPRINT</code>
* <code>notation</code>
* <code>proof@ariadne.id=https://orcid.org/ORCID</code>
* <code>save</code>

ORCID claims can be backlinked from profile URLs, so I added my Keyoxide profile as a link in that list.

Then, to update my key in the openpgp.org server, I followed the steps for [using OpenPGP with GnuPG](https://docs.keyoxide.org/guides/openpgp-gnupg/):

* <code>gpg --keyserver hkps://keys.openpgp.org --send-keys FINGERPRINT</code>

This updated my key on the key server, and I was able to immediately refresh my Keyoxide profile and see the successful claim verification.

Next up was Bluesky, which after some experimentation I was also able to successfully claim. I posted the proof [here](https://bsky.app/profile/steinea.bsky.social/post/3ledxqrloyk24), and then added the claim to my PGP key as [described](https://docs.keyoxide.org/service-providers/bsky/):

* <code>proof@ariadne.id=https://bsky.app/profile/USERNAME/post/POST_ID</code>

Sent the update to the key server, refreshed Keyoxide, and voila, another successful claim!

Next, I added an OpenPGP claim, which was quite easy, since uploading my key to the openpgp.org key server already serves as the proof. I simply added the claim as [directed](https://docs.keyoxide.org/service-providers/openpgp/):

* <code>proof@ariadne.id=openpgp4fpr:OPENPGP_FINGERPRINT</code>

Lastly, I added a Forgejo claim for my Codeberg account, which also quite quick. I created an [empty repository](https://codeberg.org/steinea/keyoxide_proof) through the Codeberg web interface, and set the description to <code>openpgp4fpr:FINGERPRINT</code>. Then, I added the proof to point to this empty repo:

* <code>proof@ariadne.id=https://DOMAIN/USERNAME/REPO_NAME</code>

I'm currently having trouble with my [Liberapay](https://liberapay.com/steinea/), [SourceHut](https://git.sr.ht/~steinea/keyoxide_proof), and DNS proofs, and I'm not sure what I'm doing wrong... The Keyoxide Project has their Liberapay [claim verified](https://keyoxide.org/project@keyoxide.org) and it [looks](https://liberapay.com/Keyoxide) exactly the same as [mine](https://liberapay.com/steinea/). Likewise, they have several DNS proofs verified, but something is not working with my TXT record with Hover. Not sure how to fix it. And I haven't been able to find any Keyoxide profile with a SourceHut claim, so not sure where to start here.
