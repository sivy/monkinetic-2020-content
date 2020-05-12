date: 2020-02-19 03:48
mastodon_id: "103683470963353491"
mastodon_url: https://toot.cafe/@sivy/103683470963353491
slug: new-posting-ui-on-goldfrog
tags: webdevelopment,progressiveenhancement,goldfrog
title: New Posting UI on Goldfrog
twitter_id: "1229976451958444032"
twitter_url: https://twitter.com/steveivy/status/1229976451958444032
---
I've started messing around a bit with javascript-enhanced UIs for #goldfrog. Rather than use all of JQuery, I decided on a small subset of Jquery's functionality as implemented by [Sprint.JS](https://github.com/bendc/sprint).

1. I only load the JS for me, since I'm logged in.
2. It's only used on the home page to power the new switchable post form, and 
3. It powers a character-counter for the note UI.

Here's the new posting UI:

![http://monkinetic.blog/uploads/new_post_ui_goldfrog.png](http://monkinetic.blog/uploads/new_post_ui_goldfrog.png)

I'm trying to implement some basic [progressive enhancement](https://adactio.com/tags/progressive%20enhancement) - the forms work as is without javascript, but the switcher and the counter are niceties for me, the author.
