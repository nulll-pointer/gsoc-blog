---
layout: post
title: Working on fifth feature, GSoC 2018 with phpmyadmin
---

### Working on fifth feature
I'm currently working on the [fifth feature](https://github.com/phpmyadmin/phpmyadmin/issues/13155)-
This is one of the most requested features in my [features' list](https://nulll-pointer.github.io/gsoc-blog/enhancements/)
Till now I've done the following-
1. Added a configuration directive in config.default.php as $cfg\['Import'\]\['enable_drag_drop_import'\]
2. Added a checkbox in the settings page to toggle this config on or off.
3. Disabled the handler at the server side if config is set to disabled.

TODO:
1. Test on multiple servers.
2. Disable drag drop handlers in javascript.