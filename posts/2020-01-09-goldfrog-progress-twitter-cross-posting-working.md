title: Goldfrog Progress: Twitter cross-posting working
slug: goldfrog-progress-twitter-cross-posting-working
date: 2020-01-09 05:13:28
tags: twitter,goldfrog,crossposting,blogging,golang
---
I finally got cross-posting to twitter working:

![/static/images/Screen Shot 2020-01-09 at 10.09.59 AM.png](/static/images/Screen Shot 2020-01-09 at 10.09.59 AM.png)

The Twitter API part was easy, using [go-twitter](https://github.com/dghubble/go-twitter)

The hard bits were writing the code to transmogrify a Post struct into reasonably formatted content for the cross-posted tweet, and then getting the template fixes done to provide the right metadata for a given link.
