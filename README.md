About
=====

This module provides integration with [Rollbar](https://rollbar.com/). Rollbar provides a central
point for managing errors and warnings in your code. With Rollbar you can easlily track when errors begin to occur and how often.

This is not an official Rollbar module, this is currently also not on Drupal.org as I am unsure about the licensing of the third party code.

Sign up for an account at https://rollbar.com/


Features
========

This module currently only supports Drupal 7, with the following features. Over the next few weeks, I will be making some changes and hopefully getting this module listed on Drupal.org.

* Configurable PHP library path.
* Configurable access keys.
* Configurable environment (production, staging, development or custom).
* PHP Exception handler.
* PHP Error handler.
* Drupal Watchdog error handler.
* Ignore Drupal watchdog PHP errors. (Don't send these to Rollbar).
* Ability to turn off native PHP handlers and send all watchdog errors.
* JavaScript integration (send JS errors/exceptions to Rollbar.com).
* PHP/JavaScript integration are seperate use them both or only one of them.

Installation
============

1. Clone this repository. `git clone git@github.com:thepearson/drupal_rollbar.git`
2. Copy the rollbar directory to the modules folder in your installation.
3. Enable the module using Administer -> Modules (`admin/modules`)
4. Download rollbar.php from https://github.com/rollbar/rollbar-php and place it in `sites/all/libraries/rollbar/rollbar.php`


Configuration
=============

All configuration settings can be found under `admin/config/development/rollbar` once the module is enabled.


License
=======

The code in this module for the most part should be licensed under the GPLv2 however I am unsure about the licensing of the JavaScript snippet which is included and the official Rollbar library that is required to make the PHP support run. If any of the folks at Rollbar can let me know about the licensing. Untill I clear that up all Rollbar code and libraries are property of them.


