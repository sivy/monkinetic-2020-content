date: 2004-11-10
slug: caching-improvements
title: Caching improvements
---
I've been seeing some performance losses on this site recently, between the search engines and the spambots, and more load on the T1 I'm behind, so (on [Seth](http://truerwords.net)'s excellent suggestion) I hacked |WordPress| to never send no-cache headers (which it was sending on requests of every kind). You should see a bit more zippiness from the site now.