# gulp-gitmodified
[![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][depstat-image]][depstat-url]

> gitmodified plugin for [gulp](https://github.com/gulpjs/gulp)

## Usage

A plugin for Gulp to get an object stream of modified files on git.

**Note:** Highly experimental. There is no tests yet and it's in early alpha. Tests will come soon.

First, install `gulp-gitmodified` as a development dependency:

```shell
npm install --save-dev gulp-gitmodified
```

Then, add it to your `gulpfile.js`:

```javascript
var gitmodified = require("gulp-gitmodified");

var files = gulp.src("./src/*.ext")
	.pipe(gitmodified())

files.on('data', function (file) {
  console.log("Modified file:", file);
})
```

## API

### gitmodified()

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)

[npm-url]: https://npmjs.org/package/gulp-gitmodified
[npm-image]: https://badge.fury.io/js/gulp-gitmodified.png

[travis-url]: http://travis-ci.org/mikaelbr/gulp-gitmodified
[travis-image]: https://secure.travis-ci.org/mikaelbr/gulp-gitmodified.png?branch=master

[depstat-url]: https://david-dm.org/mikaelbr/gulp-gitmodified
[depstat-image]: https://david-dm.org/mikaelbr/gulp-gitmodified.png