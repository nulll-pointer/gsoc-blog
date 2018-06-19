---
layout: post
title: Working on fourth feature, GSoC 2018 with phpmyadmin
---

### Working on fourth feature
I'm currently working on the fourth feature-
Before starting, I was thinking about showing a popup to add index when user tries to add AUTO_INCREMENT to an existing column. But in our conversations, Isaac and I decided to -
1. Automatically add PRIMARY KEY instead of showing a popup to add index.
2. Disable popup when user clicks on the A_I checkbox in column insert and new table page.

### Issues I'm currently working on-
1. [Fatal javascript error while adding index to a new column, #14402](https://github.com/phpmyadmin/phpmyadmin/issues/14402)