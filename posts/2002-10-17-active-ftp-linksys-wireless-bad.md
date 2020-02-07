date: 2002-10-17
slug: active-ftp-linksys-wireless-bad
title: Active FTP + Linksys Wireless == Bad
---
I haven't tracked down why yet, but I think I've confirmed that software operating in active ftp mode (as opposed to passive ftp, in this case fink) is incompatible with the 802.11 implementation in the Linksysy WAP that I've got. Whenever I tried to download software with fink my wireless connection would start going up and down, then just down, until I reset the WAP. I reconfigured fink to use passive FTP and am now having no problems. I'm going to research this more a bit later and write it up here.