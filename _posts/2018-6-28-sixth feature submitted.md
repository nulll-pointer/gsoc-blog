---
layout: post
title: Sixth feature submitted, GSoC 2018 with phpmyadmin
---

### Sixth feature submitted
I've submitted a [PR](https://github.com/phpmyadmin/phpmyadmin/pull/14436) for the sixth feature.
Adds features discussed in [#13023](https://github.com/phpmyadmin/phpmyadmin/issues/13023)
1. Show ajax errors at the bottom of the page, instead of showing them in a popup.
2. Add copy query button for errors in processing sql queries.

### Plans for next week-
The next feature(#7) that I'll be working on is-
[Add warning for default user/password usage](https://github.com/phpmyadmin/phpmyadmin/issues/12603)
Don’t use the controluser ‘pma’ if it does not yet exist and don’t use ‘pmapass’ as password.
consider testing if pma:pmapass is used, and warn about it?