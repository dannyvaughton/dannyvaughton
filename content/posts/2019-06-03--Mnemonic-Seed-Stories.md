---
title: Mnemonic Seed Stories
date: "2019-06-03T22:40:32.169Z"
template: "post"
draft: false
slug: "/mnemonic-seed-phrases"
category: "Ideas"
tags:
  - "Ideas"
  - "Cryptocurrency"
  - "Bitcoin"
description: "Storing your private key for a cryptocurrency wallet is a pain. How about Mnemonic Seed Stories?"
---

### Private Keys

Storing your private key for a cryptocurrency wallet is a pain. Losing your private key means losing access to your account, forever. And storing your private key can be a risky business in space rife with hacking & theft.

In an ideal world, a private key would be:

- Easy to read
- Easy to store, manage & secure
- Easy to memorise

This would allow you to store your key on paper in a safe location, and remember it like a password — for quick access to your account anywhere in the world. 

But, private keys look like this:

> xprv9s21ZrQH143K47JgogRrQ6WBB9WVrtPWKZGwHVnCvJ8Uyd6iSpxcVp7oy
DyQp6L37LpX22A8XkSfv686p2JZD54Fpr7ySzddz9gqTK2eAqj

A difficult to read, hard to store & impractical to memorise string of numbers & letters.

### Mnemonic Seed Phrases

Thankfully, mnemonic seed phrases are a great word-based representation of a difficult-to-read private key, allowing users to easily store & retrieve their keys.

For example, the BIP32 root key mentioned above is expressed as: 

> chicken reward swim chef tray antenna island stand cotton also reveal tomorrow mix canvas spike

Unfortunately, even when presented with a friendly string of words, users are unlikely to take the time to remember their phrase. Sure, it's easy to write down & retrieve, but not remember. The jumble of words is too long, incoherent & unwieldy. Thus, the humble Mnemonic Seed Phrase does not fit all three of our criteria — well, not at least by itself. 

### Human Memory

Humans are terrible at remembering seemly random numbers & letters. But when converted in a story with pictures, people are able to accomplish insane feats of memory. In 2015, a Japanese man by the name of Akira Haraguchi [remembered 111,700 digits of Pi](https://www.theguardian.com/science/alexs-adventures-in-numberland/2015/mar/13/pi-day-2015-memory-memorisation-world-record-japanese-akira-haraguchi) by converting numbers into syllables and then turning those syllables into stories.

### Introducing Mnemonic Seed Stories 

When presented with a Mnemonic Seed Phrase, users are usually prompted to write down their phrase on paper and then assemble a jumble of words on screen in the right order to "prove" they have remembered or at least written the phrase down.

My idea would be to generate and assemble a coherent story with simple, yet novel, pictures from words in your seed phrase. The user interface would walk you through your story like a book. After a few minutes of story repetition, you'd be asked to recall your phrase, only preceding if you have answered correctly.

Using the above example, a story could look something like this: A `chicken` is `reward`ed by a `swim`ming `chef` with a `tray` of `antennas` around an `island`... and so on.

### Challenges

Generating a seed phrase story with Bitcoins [BIP39 spec](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki) would be tricky, hence the reason I cut my story short. It's very hard to generate a coherent story with a random list of words. Some predictability is important with heavy use of simple objects, animals & adjectives — which reduces security of the seed story.

Additionally, building a timeline of images to match words & adjectives would be very difficult. For example, `a chef with a tray of antennas`. The best representation of this phrase would literally be a cartoon of a chef holding a tray of antennas. This step is not essential — Users could be presented with different images and left to imagine what they'd look like together.

### How To Build?

With the challenges presented above, it seems the easiest way to build a mnemonic seed story would be to randomly select & combine small predefined plots, and randomly substitute words with different characters, objects and adjectives. However, there's a question over security. Using this method may require a very long story and subsequently nullify the reason for generating a story in the first place.

I would love to see an AI based solution to the these challenges.
