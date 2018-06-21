---
layout: post
title: Fourth feature submitted, GSoC 2018 with phpmyadmin
---

### Fourth feature submitted
I've submitted a PR for the fourth feature.
The following new functionalities have been added-
1. Automatically add PRIMARY KEY on column edit page when user tries to set AUTO INCREMENT.
2. Disable popup when user clicks on the A_I checkbox in column insert and new table page and automatically set default index to PRIMARY with defaults.

### Plans for next week-
The next feature(#5) that I'll be working on is-
[Add a configuration option to disable drag drop files completely](https://github.com/phpmyadmin/phpmyadmin/issues/13155)
This is one of the most requested features among the ones in my proposal.

1. I'll be adding a setting among other settings where user can disable the checkbox to disable drag/drop file functionality.
2. This setting will directly interact with the configuration file(just like how other configuration settings work).
There are some workarounds suggested by the users in the feature request page, I still have to figure out the safest and best among them, or, I'll be finding out a workaround of my own.