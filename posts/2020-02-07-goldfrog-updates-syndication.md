date: 2020-02-07 03:28
mastodon_id: "103615437733142227"
mastodon_url: https://toot.cafe/@sivy/103615437733142227
slug: goldfrog-updates-syndication
tags: blogging,goldfrog,indieweb
title: 'Goldfrog updates: syndication'
twitter_id: "1225622325241905152"
twitter_url: https://twitter.com/steveivy/status/1225622325241905152
---
If you follow me on social media - [Twitter](https://twitter.com/steveivy) or [Mastodon](https://toot.cafe/@sivy) - you may have seen lots of nonsense posts go by recently...

![http://monkinetic.blog/uploads/Screen Shot 2020-02-06 at 8.19.51 PM.png](http://monkinetic.blog/uploads/Screen Shot 2020-02-06 at 8.19.51 PM.png)

I've been working on improving my [POSSE](https://indieweb.org/POSSE) features here, which meant not only composing my posts and notes locally, and then publishing them to Twitter et al, but also being able to track where they "landed" (ids and links) and make it easy for users to find my content on the syndicated site.

So I dug back into my syndication code, rewrote it several times, learned some things about goroutines, learned how *not* to do some things with goroutines, and settled on a way that worked. With luck, this post and any other that is also published on Twitter or Mastodon will have links to those sites along with the post, and (at least for Twitter right now) have links to reply, favorite, or retweet the post.

As [Dave](http://scripting.com) used to be fond of saying:

> Still digging!
