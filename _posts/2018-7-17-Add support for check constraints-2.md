---
layout: post
title: Add Support for CHECK Constraints, Lakshay Arora | GSoC 2018 with phpmyadmin
---

### [Add Support for CHECK Constraints](https://github.com/phpmyadmin/phpmyadmin/issues/13592)
#### Post 2
This feature request is divided in three parts - 
1. Implement an interface for interacting with these constraints
2. Update parser to understand this syntax
3. Update the export interface to allow including these in an export

Mysql does not provide any way to alter the definition of a constraint. The main idea is to add support for a constraint and additionally build a feature seperate from mysql to alter a constraint.

I've submitted the PR for the first part of the feature.
I'm currently working on the sql-parser.(The second part)
#### Work done - 
1. SQL parser now recognizes CHECK statements in alter table commands.

### Plans for this week-
1. Make sql parse fully aware of the CHECK statements.
2. Update the export interface to allow including these in an export.