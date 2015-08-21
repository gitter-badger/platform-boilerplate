Platform Boilerplate
============


Ideal
------------

To have 1 boilerplate that can build your app and run it any ware possible. You should only need this boilerplate if you want to run a MEAN stack.

Intro
------------

Boilerplate for an app that can be exported to all major platforms available, native mobile, web, desktop behind that is a node server connected to a mongodb. All done via a MEAN stack.

Tech spec
------------

So this is the tech spec so far - please add some input in the [issues][1] section

Basic (MEAN stack)
------------

* Mongodb
* Node server
* Angular
* Sass
* Html

Tools
------------

* [node-webkit][2] for compiling into native **desktop** application
* [ionic][3] for compiling into native **mobile** application
* [Gulp][4] as task runner


Further functionality
------------

It would be nice to have following things aswell

* [bower][5] for frontend dependencies management
* build-in support for authentication with facebook, twitter, github, google & linkin support (maybe utilize passportjs)
* CI could be [jenkins][6] or similar
* Javascript testing could be [Jasmine][7] or simliar
* In addition to javascript testing jshint would be nice
* ES6 support trough babel
* A yeoman generator to scaffold all of the code
* Deployment of some kind, i would love to use docker containers for this


Contributing
------------

If you want to contribute to Platform Boilerplate's development. You can read about it in [CONTRIBUTING.md][8].


[1]: https://github.com/sp90/full-platform-boilerplate/issues
[2]: https://github.com/nwjs/nw.js/
[3]: http://ionicframework.com/
[4]: http://gulpjs.com/
[5]: http://bower.io/
[6]: https://jenkins-ci.org/
[7]: http://jasmine.github.io/2.0/introduction.html
[8]: https://github.com/sp90/platform-boilerplate/blob/master/CONTRIBUTING.md

