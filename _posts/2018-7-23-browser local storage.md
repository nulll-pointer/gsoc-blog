---
layout: post
title: Integrate storing user preferences in browser local storage, Lakshay Arora | GSoC 2018 with phpmyadmin
---

### [Integrate storing user preferences in browser local storage](https://github.com/phpmyadmin/phpmyadmin/issues/13843)
#### Post 1
This is my favorite feature request because of its importance and the challanges it imposes.
The data about add on features is stored in the configuration storage, when it is not configured, the data doesn't persist over session. In those cases the data should be saved in browser local storage.
1. All this data(stored on client side) will be needed by the server, so we'll need to pass the data to the server during login.
2. Whenever user makes some changes in the data, after processing it on the server side, it can be passed on to the client using ajax request and updated in browser local storage.

### Plans for this week-
Automatically load settings from local storage at login time.