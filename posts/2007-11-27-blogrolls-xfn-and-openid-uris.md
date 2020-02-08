date: 2007-11-27 00:00
slug: blogrolls-xfn-and-openid-uris
tags: ""
title: Blogrolls, XFN, and OpenID URIs
---
While writing [Whitelisting With OpenID and XFN](http://redmonk.net/archives/2007/11/25/making-a-list-whitelisting-with-openid-and-xfn/), I started thinking about what kind of work would have to go into implementing these ideas in Wordpress. One of the roadblocks I ran into was that in Wordpress (and Drupal, probably, and most other similar systems) links only support a single URI (not surprisingly). In order to support OpenID whitelisting, we need a unique identifying URI for an XFN contact - which may or may not be the same as the blog/site URI that you'd want to list in a blogroll.
