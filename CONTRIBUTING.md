Contributing to Platform Boilerplate
============

#### Contributing code?

1. [Fork Platform Boilerplate][1].
2. `git checkout -b descriptive-branch-name dev` and make your commits.
3. When you think your code is ready, create a pull request against the development branch. 
4. Please check [existing issues][2] when possible.

#### Have ideas would like to see implemented?
* You can [suggest features][2].
* You can [discuss a bug][2] or [report a bug][2]!


Branch structure
----------------

This repository is made up of two branches: master (stable app) and dev (unstable / development in progresss).

* **master** has the latest stable code.
* **dev** includes the latest unstable.


Code Style
----------------

#### Angular

This repository follows [johnpapa][3] guide lines and convention. Because this code styles are based on exprienced developers with angular.

## Table of Contents

  1. [Single Responsibility](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#single-responsibility)
  1. [IIFE](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#iife)
  1. [Modules](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#modules)
  1. [Controllers](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#controllers)
  1. [Services](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#services)
  1. [Factories](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#factories)
  1. [Data Services](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#data-services)
  1. [Directives](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#directives)
  1. [Resolving Promises for a Controller](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#resolving-promises-for-a-controller)
  1. [Manual Annotating for Dependency Injection](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#manual-annotating-for-dependency-injection)
  1. [Minification and Annotation](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#minification-and-annotation)
  1. [Exception Handling](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#exception-handling)
  1. [Naming](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#naming)
  1. [Application Structure LIFT Principle](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#application-structure-lift-principle)
  1. [Application Structure](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#application-structure)
  1. [Modularity](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#modularity)
  1. [Startup Logic](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#startup-logic)
  1. [Angular $ Wrapper Services](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#angular--wrapper-services)
  1. [Testing](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#testing)
  1. [Animations](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#animations)
  1. [Comments](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#comments)
  1. [JSHint](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#js-hint)
  1. [JSCS](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#jscs)
  1. [Constants](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#constants)
  1. [File Templates and Snippets](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#file-templates-and-snippets)
  1. [Yeoman Generator](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#yeoman-generator)
  1. [Routing](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#routing)
  1. [Task Automation](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#task-automation)
  1. [Filters](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#filters)
  1. [Angular Docs](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#angular-docs)
  1. [Contributing](https://github.com/johnpapa/angular-styleguide/blob/master/README.md#contributing)


#### SASS/CSS
This repository uses BEM syntax for all its css/sass naming for classes since it does provide trasnparency and useful meaning to other developers.

###### Naming convention
```
.site-search {}
.site-search__field {}
.site-search--full {}

```
- **.site** represents the higher level of an abstraction or component.
- **.site__element** represents a descendent of **.site** that helps form .site as a whole.
- **.site--modifier** represents a different state or version of **.site**.

The point of BEM is to tell developers more about what a piece of markup is doing from its name alone. For example:

```
.person {}
.person__hand {}
.person--female {}
.person--male {}
.person--female__hand {}
.person__hand--left {}

```
The top level block is a *person* which has elements such as *hand*. This person can has variations such *male/female*.
[learn more here][4]


#### Node.js
##### Basic rules of life
- No trailing whitespaces
- 80 characters per line
- Use 1 tab for indeting... DO NOT mix tab and spaces
- Use Semicolons

##### Rules with Example
###### Use single quotes
Always use single qoutes, unless is JSON ;) 

Right:

```
var foo = 'bar';

```
###### Braces go on the same line
Place opening braces always in the same line

```
if(you_are_amazing){
	console.log('yes you are!');
}

```

###### Method Chaining
One method per line while chaining methods please 

```
User
  .findOne({ name: 'foo' })
  .populate('bar')
  .exec(function(err, user) {
    return true;
  });

```
 
###### Declaring multiple
Always declare one variable per statement

```
var cph = ['foo', 'bar'];
var val = [22, 11];
var obj = {};

```
###### Use lowerCamelCase for var, properties and function names
Variables, properties and function names should use lowerCamelCase. They should be descriptive and try to avoid uncommon abbreviations. 

```
var superAdminUser = db.query(".... ");

```


###### Use UpperCamelCase for classes
Class names should use UpperCamelCase

```
function BankController(){
	
}
```

###### UPPERCASE for constants
Contants should always be Uppercase

```
var THIS_REPO_WILL_BE_GREAT = true;

```

###### Objects and Arrays
Use trailing commans and short declarations should be on a single line

```
var x = ['Hello', 'World'];
var y = {
	example: true,
	'general': true,
	'time' : '20151027'	
};

```
###### Use the right comparison operator
Use *===* to insure a strict equality

```
var x = 0;
if(x !== ''){
	console.log("game over");
}

```
###### Use descriptive conditions
Any non-trivial conditions should be assigned to a descriptively named variable

``` 
var isValidPassword = password.length >= 4 && /^(?=.*\d).{4,}$/.test(password);

if (isValidPassword) {
  console.log('valid password');
}

```

###### Commenting 
Use slashes for both single line and multi line comments. Try to write comments that exmplain or clarify difficult parts of your code.

```
// Get some really strong password
var matches = password.match(^(?=.*[A-Z].*[A-Z])(?=.*[!@#$&*])(?=.*[0-9].*[0-9])(?=.*[a-z].*[a-z].*[a-z]).{8}$);

// This function has a failure while
// handling some non exisitng user
function changeUserPassword(id, password){
	
}

``` 


Copyright
----------------

Copyright (c) 2015 [sp90](http://www.nomis.dk/)

###### (The MIT License)
Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.




 [1]: https://github.com/sp90/platform-boilerplate
 [2]: https://github.com/sp90/platform-boilerplate/issues
 [3]: https://github.com/johnpapa/angular-styleguide
 [4]: http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/
 [5]: http://stackoverflow.com/questions/523643/difference-between-and-in-javascript