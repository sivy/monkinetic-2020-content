date: 2020-02-13 04:29
mastodon_id: "103649652305193983"
mastodon_url: https://toot.cafe/@sivy/103649652305193983
slug: fun-with-barcodes
tags: barcodes,c128,golang
title: Fun with Barcodes
twitter_id: "1227812057724010497"
twitter_url: https://twitter.com/steveivy/status/1227812057724010497
---
Being the curious sort, I wondered what it would take to generate #barcodes programmatically, and found this [neat site](https://www.barcodesinc.com/generator/index.php). Here's "monkinetic.blog" rendered as a `Code 128` barcode:

![http://monkinetic.blog/uploads/monkinetic_as_a_barcode.png](http://monkinetic.blog/uploads/monkinetic_as_a_barcode.png)

Then I found a [barcode package](https://godoc.org/github.com/boombuler/barcode) for #golang, so of *course* I'm trying to decide what on this site I could generate barcodes for...
