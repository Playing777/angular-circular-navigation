# angular-circular-navigation [![Build Status](https://travis-ci.org/maxklenk/angular-circular-navigation.svg?branch=master)](https://travis-ci.org/maxklenk/angular-circular-navigation) [![Coverage Status](https://coveralls.io/repos/maxklenk/angular-circular-navigation/badge.png?branch=master)](https://coveralls.io/r/maxklenk/angular-circular-navigation?branch=master) [![Dependency Status](https://gemnasium.com/maxklenk/angular-circular-navigation.svg)](https://gemnasium.com/maxklenk/angular-circular-navigation)

angular-circular-navigation is a [AngularJS](https://github.com/angular/angular.js) directive, which is build on top of the Tutorial [Building a circular navigation with css transform](http://tympanus.net/codrops/2013/08/09/building-a-circular-navigation-with-css-transforms/) by [Sara Soueidan](http://sarasoueidan.com/).


## Usage

You can get it from [Bower](http://bower.io/):
```sh
bower install angular-circular-navigation
```

Add everything to your index.html:
```html
<link rel="stylesheet" href="bower_components/angular-circular-navigation/angular-circular-navigation.css">

<script src="bower_components/angular/angular.js"></script>
<script src="bower_components/angular-circular-navigation/angular-circular-navigation.js"></script>
```

And specify the directive in your module dependencies:
```javascript
angular.module('myApp', ['angularCircularNavigation'])
```

Add the corresponding options in your controller:
```javascript
$scope.options = {
  content: 'Menu',
  isOpen: false,
  toggleOnClick: true,
  items: [
    {
      content: 'About',
      cssClass: '',
      onclick: function () {console.log('About');}
    }
  ]
};
```

Then you are ready to use the directive in your view:
```html
<div ng-controller="Controller">
  <circular
    options="options">
  </circular>
</div>
```

### Options

...


## Development

We use Karma and jshint to ensure the quality of the code. The easiest way to run these checks is to use grunt:
```sh
npm install -g bower grunt-cli
npm install
grunt
```


## Contributing

Please submit all pull requests the against develop branch. Make sure it passes the CI [![Build Status](https://travis-ci.org/maxklenk/angular-circular-navigation.svg?branch=develop)](https://travis-ci.org/maxklenk/angular-circular-navigation) and add tests to cover your code [![Coverage Status](https://coveralls.io/repos/maxklenk/angular-circular-navigation/badge.png?branch=develop)](https://coveralls.io/r/maxklenk/angular-circular-navigation?branch=develop). Thanks!

## Authors

**Max Klenk**

+ http://github.com/maxklenk



## Copyright and license

	The MIT License

	Copyright (c) 2014 Max Klenk

	Permission is hereby granted, free of charge, to any person obtaining a copy
	of this software and associated documentation files (the "Software"), to deal
	in the Software without restriction, including without limitation the rights
	to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
	copies of the Software, and to permit persons to whom the Software is
	furnished to do so, subject to the following conditions:

	The above copyright notice and this permission notice shall be included in
	all copies or substantial portions of the Software.

	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
	IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
	FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
	AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
	LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
	OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
	THE SOFTWARE.
