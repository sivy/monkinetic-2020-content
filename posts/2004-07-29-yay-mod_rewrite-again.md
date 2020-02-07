date: 2004-07-29
slug: yay-mod_rewrite-again
title: Yay mod_rewrite, again
---
I've found some links to my content floating around the web of the form
<code><a href="http://www.redmonk.net/discussion/thread.html$msgnum=2353">www.redmonk.net/discussion/thread.html$msgnum=2353</a></code> So I decided to route them to the same script that maps some of my other old [Conversant](http://free-conversant.com) URLs to the new site, and now the discussion-style links work after a fashion - they get [302](http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html#sec10.3.3)'d to the correct url - in this case [redmonk.net/archives/2003/10/30/winter-lawn-redux](http://redmonk.net/archives/2003/10/30/winter-lawn-redux).