Grunt Experiment #2
===================

In this experiment I want to move in the direction of a grunt and django integration. Sokanu's production project uses Django, and my primary interests are 1) using Grunt in my day-to-day work at the company, and 2) helping make other people's lives easier with Grunt.

## What Makes a Django Static Environment?

In Django's paradigm stylesheets, scripts, images and everything else that runs client-side is placed in a group called “static assets.” From what I understand, this is similar to other frameworks such as Ruby on Rails with it's “asset pipeline”. So, what constitutes a Django static environment? A few things:
- multiple static asset directories contained in separate apps
- all static directories are combined into one during any static file lookup
These are the technical factors that I want to integrate grunt with. There is another, less technical consideration: different apps are managed by different developers. Currently we have around ten applications with their own static files, and ownership is split between three developers. Using grunt in a particular way or at all is not required per each app.