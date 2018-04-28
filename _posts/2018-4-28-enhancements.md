---
layout: post
title: GSoC proposal. Enhancements I'll work on.
---

Following is the list of enhancements I'll work on this summer.
### [1. ​Add modal to login after session expired](https://github.com/phpmyadmin/phpmyadmin/issues/13654)

The default idle session timeout is 24 minutes, after which the session is destroyed and
the user has to login again to use the app. The problem is that the login page is
rendered over the current page leading to loss of all the information user was entering.
Login page overwrites the current page


##### Enhancement -

Append a modal on the page which would ask for login, instead of rendering the
whole login page, which would preserve information.

### 2. Importing table from a CSV file

When a table is imported from a CSV file, the default table name is Table ## and default
names for the columns are COL ##.
Default table and column names

##### Enhancement-

Set the imported table name to the name of the imported file and column names
to the titles of each column in the csv file OR ask the user to enter table and column
names.

### [3. ​Increase input field width for varchar(255)](https://github.com/phpmyadmin/phpmyadmin/issues/13627)

##### Enhancement-

In the insert row page, the dimensions of varchar textareas are small, which
could be increased. As suggested in a ​comment​, the user appreciated presence of this
feature in the earlier version and thus can be re-considered in the current version for a
better user-experience.



Default width of varchar textareas in insert page

### [4. ​Edit an existing row and setting auto increment should prompt to add index](https://github.com/phpmyadmin/phpmyadmin/issues/13235)

Making an existing int column ‘auto_increment’ shows the error message “#1075 -
Incorrect table definition; there can be only one auto column and it must be defined as a
key”.
Error message when trying to add auto increment on existing column


##### Enhancement-


Show a dialog to add an index to the column.

#### [5. ​Configuration option to disable drag drop files completely](https://github.com/phpmyadmin/phpmyadmin/issues/13155)

##### Enhancement-


Add a configuration option to disable drag and drop files support.

### [6.​ ​Error popup](https://github.com/phpmyadmin/phpmyadmin/issues/13023)

In the error popup, it is difficult to read the query when it overflows and it’s not possible
to copy the query as the popup closes when clicked.
Error popup

##### Enhancement-

1. Disable onclick close by default and add a close button at the top right corner.
2. Wrap the query if it overflows for better readability.
3. Add a ‘Copy Query’ button.


### [7.​ ​Add warning for default user/password usage](https://github.com/phpmyadmin/phpmyadmin/issues/12603)

##### Enhancement-

1. Don’t use the controluser ‘pma’ if it does not yet exist and don’t use ‘pmapass’ as
    password.

2. Test if pma:pmapass is used, and warn about it.

### [8. ​Order distinct values table by count](https://github.com/phpmyadmin/phpmyadmin/issues/13750)

The distinct values table is currently ordered by value.

##### Enhancement-


Order the distinct values by count in descending order.

### [9. ​Store user preferences in browser local storage](https://github.com/phpmyadmin/phpmyadmin/issues/13843)


All user configuration is stored in the user preferences. When the phpMyAdmin storage
configuration is not configured, these do not persist over session.

##### Enhancement-


Use browser local storage for storing user configuration.

### [10. ​Add support for CHECK constraints (feature request)](https://github.com/phpmyadmin/phpmyadmin/issues/13592)


MariaDB (MySQL-compatible) added support for CHECK constraints to version 10.2.
(stable=10.2.8). It would be very useful if PHPMyAdmin had a UI for adding and
managing these in tbl_create.php and tbl_structure.php.

##### Enhancement-


Implement a UI for adding and managing CHECK constraints in tbl_create.php
and tbl_structure.php.
