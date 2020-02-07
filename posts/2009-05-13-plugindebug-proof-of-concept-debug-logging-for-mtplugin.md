date: 2009-05-13
slug: plugindebug-proof-of-concept-debug-logging-for-mtplugin
title: 'PluginDebug: proof-of-concept debug logging for MT::Plugin'
---
As a developer for [SixApart](http://sixapart.com) Services, one thing I do a lot of is put debug code in plugins I'm working on to output values to Movable Type's backend activity log. This can get messy, and I usually end up writing a one-off debuglog function for each plugin to make this more convenient.