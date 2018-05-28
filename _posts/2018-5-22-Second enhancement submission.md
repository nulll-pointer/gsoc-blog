---
layout: post
title: Second enhancement, week 3, GSoC 2018 with phpmyadmin
---

### End of Week 3
I've submitted a PR for the second feature -
Following new features have been added to the csv import plugin- 

1. For a new import, user can now directly enter the table or database name at the time of import.
2. Partial import. User can enter how many rows they want to import.
3. Show table structure edit form when the import is successful(undecided).

I'm also working on some issues in the issue tracker.
1. (Issue in Changing theme)[https://github.com/phpmyadmin/phpmyadmin/issues/14295]
2. (preg_match error when clicking Insert or Search tabs)[https://github.com/phpmyadmin/phpmyadmin/issues/14315]

### Plans for next weak.
As stated in my proposal, my end sems have started and I won't be able to work for the next 10 days.
From 1st. I'll be working on the 3rd enhancement.

#### ​(Increase input field width for varchar(255))[https://github.com/phpmyadmin/phpmyadmin/issues/13627]
##### Enhancement-
In the insert row page, the dimensions of varchar textareas are small, which could be increased. As suggested in a ​comment​, the user appreciated presence of this feature in the earlier version and thus can be re-considered in the current version for a better user-experience.