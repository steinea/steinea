---
layout: wiki
category: wiki
subcategory: concepts
title: PGP Word List
publication: Wikipedia
link: https://en.wikipedia.org/wiki/PGP_word_list
date: 2025-01-02
---

"The PGP Word List ('Pretty Good Privacy word list', also called a biometric word list for reasons explained below) is a list of words for conveying data bytes in a clear unambiguous way via a voice channel. They are analogous in purpose to the NATO phonetic alphabet, except that a longer list of words is used, each word corresponding to one of the 256 distinct numeric byte values.

The PGP Word List was designed in 1995 by Patrick Juola, a computational linguist, and Philip Zimmermann, creator of PGP. The words were carefully chosen for their phonetic distinctiveness, using genetic algorithms to select lists of words that had optimum separations in phoneme space. The candidate word lists were randomly drawn from Grady Ward's Moby Pronunciator list as raw material for the search, successively refined by the genetic algorithms. The automated search converged to an optimized solution in about 40 hours on a DEC Alpha, a particularly fast machine in that era.

The Zimmermann–Juola list was originally designed to be used in PGPfone, a secure VoIP application, to allow the two parties to verbally compare a short authentication string to detect a man-in-the-middle attack (MiTM). It was called a biometric word list because the authentication depended on the two human users recognizing each other's distinct voices as they read and compared the words over the voice channel, binding the identity of the speaker with the words, which helped protect against the MiTM attack. The list can be used in many other situations where a biometric binding of identity is not needed, so calling it a biometric word list may be imprecise. Later, it was used in PGP to compare and verify PGP public key fingerprints over a voice channel. This is known in PGP applications as the "biometric" representation. When it was applied to PGP, the list of words was further refined, with contributions by Jon Callas. More recently, it has been used in Zfone and the ZRTP protocol, the successor to PGPfone.

The list is actually composed of two lists, each containing 256 phonetically distinct words, in which each word represents a different byte value between 0 and 255. Two lists are used because reading aloud long random sequences of human words usually risks three kinds of errors: 1) transposition of two consecutive words, 2) duplicate words, or 3) omitted words. To detect all three kinds of errors, the two lists are used alternately for the even-offset bytes and the odd-offset bytes in the byte sequence. Each byte value is actually represented by two different words, depending on whether that byte appears at an even or an odd offset from the beginning of the byte sequence. The two lists are readily distinguished by the number of syllables; the even list has words of two syllables, the odd list has three. The two lists have a maximum word length of 9 and 11 letters, respectively. Using a two-list scheme was suggested by Zhahai Stewart."

*Handy tool: <https://www.dcode.fr/pgp-word-list>*
