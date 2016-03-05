bootstrap-csh
=============

CSS overrides for [Twitter Bootstrap](http://getbootstrap.com), for use in [Computer Science House](http://csh.rit.edu) websites. 

Includes two themes:

* `members` - The "PDP-11" theme (purple and pink), for internal CSH sites
* `members-flat` - The flat/material version of the pink and purple styles.


Minified and compiled files can be found in the `release` directory. Original development files can be found in the `dev` directory. Example pages using both themes can be found in the `test` directory.

Contributing
------------

To contribute to this project:
* Fork the repository.
* Make your changes in the "dev" directory.
* Compile and minify your changes (see "Using Grunt" below).
* Verify your changes on the test pages (`test/members/` or `test/members-flat/`).
* Push your changes and submit a pull request.

Using Grunt
-----------

Learn more about Grunt: http://gruntjs.com

First, install grunt-cli: `npm install -g grunt-cli`

Next, install dependencies: `npm install`

Recommended grunt workflow:
* In one terminal window, run `grunt dev` to automatically compile and minify LESS files whenever a change is made to either theme.
* In another terminal window, run `grunt test` to spin up a web server and view your changes at `http://localhost:9000/members/` or `http://localhost:9000/members-flat/`.

All available grunt tasks:

* `grunt` or `grunt default`: Compile LESS and minify CSS for both themes
* `grunt defaultMembers`: Compile LESS and minify CSS for the `members` theme only
* `grunt defaultMembersFlat`: Compile LESS and minify CSS for the `members-flat` theme only
* `grunt dev`: Compile LESS, minify CSS, and watch for changes in both themes
* `grunt devMembers` Compile LESS, minfiy CSS, and watch for changes in the `members` theme
*  `grunt devMembersFlat` Compile LESS, minfiy CSS, and watch for changes in the `members-flat` theme
* `grunt test`: Spin up a local web server at `http://localhost:9000` to view the test pages
* `grunt testMembers`: Spin up a local web server and open the `members` test page at `http://localhost:9000/members/` 
* `grunt testMembersFlat`: Spin up a local web server and open the `members` test page at `http://localhost:9000/members-flat/` 
