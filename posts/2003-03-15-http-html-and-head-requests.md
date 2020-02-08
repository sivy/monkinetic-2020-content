date: 2003-03-15 00:00
slug: http-html-and-head-requests
tags: ""
title: HTTP, HTML, and HEAD requests
---
The other day I was working on a script and I wanted to get the titles for a bunch of web pages I had links to. I coded up something that downloaded each page, pulled out the title, and cached it (so that there would be no more than 1 request per URL).
