date: 2020-01-17 00:00
slug: towards-indieweb-notes
tags: indieweb,hashtags
title: ""
---
[POSSE](https://indieweb.org/POSSE) is the #IndieWeb acronym for *Publish (on your) Own Site, Syndicate Everywhere*. It's something I'm playing with in Goldfrog.

A common idiom is to differentiate Notes (small microblog-like posts) from Articles (longer blog posts with a title). Right now Goldfrog has a basic blog Post type, with (`ID`, `Title`, `Slug`, `Tags`, `Body`). I'd like to keep the posting experience as simple as possible, so I'm thinking about how to handle something that literally just has a `Body` (and `Tags`, because I parse and attach any #hashtags - see? - in the content).

My Posts have an ID, though a uniqueness constraint on the slug means I could use that instead. But Notes don't have a title to "slugify" (it is too a word). Goldfrog also writes every post to the filesystem as a Jekyll-compatible markdown file, so I would need to figure out what format and filename/slug would be appropriate so that they get a permalink.

**Url Options**

- 2020/01/16/note-ab43f6 *unique hash id*
- 2020/01/16/note-13:25 *HH:MM*

## Actual Progress

An upcoming build of Goldfrog will support  new "kind" of Post, albeit only differentiated by the presence of a title. I've made a few UI and backend changes to support notes:

![http://monkinetic.blog/uploads/Screen Shot 2020-01-17 at 7.58.03 AM.png](http://monkinetic.blog/uploads/Screen Shot 2020-01-17 at 7.58.03 AM.png)

- Notes get a slug that is constructed from the string "txt-" + a shortened hash based on the note's content, like `txt-8213d2c`
- Since notes are short enough to look weird on a typical post-detail page, I created a new "Daily Digest" page on the site that shows only the posts for a given day. This is the default target for the permalink for Notes. The slug is used as the `id` attribute on the note, so the link jumps directly to the note on the digest page. This results in a "permalink" like "YYYY-MM-DD/#txt-8213d2c"
- The Syndicate options (currently for Twitter and Mastodon) are now enabled by default for notes.
- Clicking the "post form" link takes me to a longer post form with options for a title, custom slug, tags, and a larger content area for writing.

## Still to work out

- I'm thinking about implementing [Webmentions](https://webmention.net/draft/) for Goldfrog, since I control the code. <evil laugh>
- I'm still pondering how to connect a post or note with it's syndicated version, to allow likes from this site to propagate to the syndicated site. That feels... harder than I want to dig into right now, but I'll be looking for ideas.
