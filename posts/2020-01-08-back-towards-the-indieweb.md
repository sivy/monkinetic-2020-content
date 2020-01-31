title: Back towards the IndieWeb
slug: back-towards-the-indieweb
date: 2020-01-08 01:25:24
tags: ,indieweb,goldfrog
---
Another aspect to creating my own blogging software: I can finally start implementing some of #indieweb principles I've been watching for a while.

One of those is [POSSE](https://indieweb.org/POSSE) (Publish Own Site, Syndicate Everywhere) - which means everything you write starts on your own site, and content is syndicated to the appropriate kinds of sites as desired. This could include things like:

- Articles are syndicated via RSS (done, no brainer)
- Short posts (notes) are automatically or optionally published whole to Twitter, Mastodon, or the microblog of your choice
- Articles are automatically or optionally shared to a microblog site with a link back to your own site

## Goldfrog + Twitter

While I generally find Twitter overwhelming and frustrating (not nearly as much so as the less-privileged do), I just finished adding a Twitter cross-poster to #goldfrog. I'll be implementing a Mastodon cross-poster in the next few days (/me waves @ [toot.cafe](https://toot.cafe)), now that I've figured out and implemented the pattern.

The Twitter cross poster will send the title, some text, and a link back to the post. So, let's see if deploying the new feature worked. :D
