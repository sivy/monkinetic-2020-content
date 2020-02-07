date: 2003-07-17
slug: fixing-safaris-min-font-size
title: Fixing Safari's min font size
---
from [FreeForm Goodness](http://www.freeke.org/ffg) comes the fix for Safari's minimum font size, which changed in [Safari 1.0](http://www.apple.com/safari).
quoteHidden pref, your ass is mine.  

<code>defaults write com.apple.safari WebKitMinimumFontSize 9<br/>
defaults write com.apple.safari WebKitMinimumFixedFontSize 9</code>  

(you need to enter those two lines in the Terminal.)endquote