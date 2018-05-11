---
layout: post
title: GSoC progress in community bonding period.
---

### GSoC progress in community bonding period. 
#### Worked on some issues in the Issue Tracker
1.  There was a [bug](https://github.com/phpmyadmin/phpmyadmin/issues/14249) in the edit view feature, where the form submission button was missing. It was a small task to add the button. Currently, I am working on removing two buttons in create view form as discussed in the [issue page](https://github.com/phpmyadmin/phpmyadmin/issues/14249).

2. There is a [bug](https://github.com/phpmyadmin/phpmyadmin/issues/14229) in the recent tables list on the navigation panel which doesn't show the recently visited tables. I've submitted a PR which solves this issue.


#### Started working on the first enhancement
As I've stated in my proposal that I won't be able to give 5-6 hours from 28th May to 8th June. I've already started working on the first enhancement.
The aim is to append a modal on the page which would ask for login, instead of rendering the whole login page, which would preserve the information which user entered in the previous session.

##### Progress
I've made the modal which is correctly appended on the page when session times out and logs in the user.
###### Implementation in detail-
There is a function UpdateIdleTime() in functions.js which sends post request just a second before the session runs out. When it finds that the session has expired(according to server response, more on this below), it reloads the page.
I've changed it so that instead of reloadin the page, it appends the modal returned(more on this below).

When updateIdleTime() sends a request to the server and it detects session timeout, it sends with a success false response and updateIdleTime() reloads the page.
Instead of returning a false response, I've changed the file "libraries/classes/Auth/AuthenticationCookie.php" to return a modal.

When the user logs in again, a new session is started issuing a new session token, all the hidden form elements with the old session token are replaced with the new token.
If a new user logs in, it reloads the page.

###### Security Concerns
I'm currenty testing for security vulnerabilities and implementing security features to prevent unauthorized access.
1. Page is automatically reloaded if the modal is deleted explicilty.
2. All the page functionalities are disabled while the modal appears.
3. .....

See you next time. :)