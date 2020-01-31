title: Towards IndieWeb: Webmention
slug: towards-indieweb-webmention
date: 2020-01-23 10:19:13
tags: indieweb,goldfrog,golang
---
For my next #indieweb trick: I'm working on adding support for [Webmention](https://www.w3.org/TR/webmention/) in #goldfrog.

https://github.com/sivy/goldfrog/issues/9

Client:

- Endpoint discovery (header, link, a)
- Send basic webmentions
- Send "special" webmentions (ie Likes)

Server:

- Provide discovery (header, link, a)
- Receive basic webmentions
- Receive "special" webmentions (ie Likes)

Ultimately I'd like to break out my webmention code into a releasable #golang module that can provide reusable `http.Handler` functions that can be plugged into any Go mux that supports them.


