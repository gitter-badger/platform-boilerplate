# Platform boilerplate

### Idear
To have 1 boilerplate that can build your app and run it any ware possible. You should only need this boilerplate if you want to run a MEAN stack.

### Intro
Boilerplate for an app that can be exported to all major platforms available, native mobile, web, desktop behind that is a node server connected to a mongodb. All done via a MEAN stack.

### Tech spec
So this is the tech spec so far - please add some input in the <a href="https://github.com/sp90/full-platform-boilerplate/issues">issues</a> section

##### Basic (MEAN stack)

* Mongodb
* Node server
* Angular
* Sass
* Html

##### Tools

* <a href="https://github.com/nwjs/nw.js/">node-webkit</a> for compiling into native **desktop** application
* <a href="http://ionicframework.com/">ionic</a> for compiling into native **mobile** application
* <a href="http://gulpjs.com/">Gulp</a> as task runner

##### Further functionality

It would be nice to have following things aswell

* <a href="http://bower.io/">bower</a> for frontend dependencies management
* build-in support for authentication with facebook, twitter, github, google & linkin support (maybe utilize passportjs)
* CI could be <a href="https://jenkins-ci.org/">jenkins</a> or similar
* Javascript testing could be <a href="http://jasmine.github.io/2.0/introduction.html">Jasmine</a> or simliar
* In addition to javascript testing jshint would be nice
* ES6 support trough babel
* A yeoman generator to scaffold all of the code
* Deployment of some kind, i would love to use docker containers for this

### Deployment Setup 
I think this would be a nice setup please contribute in the issues section if you have suggestions - i would love to use docker containers for scalability.

* Docker(Container1)     
	* Mongodb      
* Docker(Container2) 
	* Node server
* Docker(Container3)
	* Frontend/Angular
* Ionic(Android/iOS/WindowsPhone)
	* Frontend/Angular
* NW(Windows/OS X/Linus)
	* Frontend/Angular
