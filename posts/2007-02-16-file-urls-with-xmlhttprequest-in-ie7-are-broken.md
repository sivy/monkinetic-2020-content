date: 2007-02-16
slug: file-urls-with-xmlhttprequest-in-ie7-are-broken
title: File:// urls with XMLHTTPRequest in IE7 are broken
---
I've been working again on a tool at work that uses [JQuery](http://jquery.org) to dynamically load various files into the content area of a locally based web page to test css-based templates. The tool was working fine in Firefox and IE6, then I recently "upgraded" to IE7 and it went all wonky on me. After a day or so of Googling, I found this post from Xavier Hanin: [IE7 support for XmlHttpRequest](http://xhab.blogspot.com/2006/11/ie7-support-for-xmlhttprequest.html) which details the fact that *IE7's XMLHTTPRequest cannot load files from disk* (file:// urls).