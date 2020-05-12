date: 2020-02-13 03:09
mastodon_id: "103649339512365593"
mastodon_url: https://toot.cafe/@sivy/103649339512365593
slug: python-string-hexdigits
tags: python,programming
title: string.hexdigits
twitter_id: "1227792039011467264"
twitter_url: https://twitter.com/steveivy/status/1227792039011467264
---
I recently found the following in a bit of #python sample code:

```python
random_data = random.sample(string.hexdigits, 8)
```

Wait, `hexdigits`? I'd use `string.ascii_letters` and `string.ascii_lowercase` before, but this was the first time I'd seen `hexdigits`, which is exactly what you'd think:

> The string '0123456789abcdefABCDEF'.

That's useful.
