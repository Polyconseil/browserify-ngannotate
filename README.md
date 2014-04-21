# browserify-ngannotate

[![Build Status](https://travis-ci.org/omsmith/browserify-ngannotate.svg)](https://travis-ci.org/omsmith/browserify-ngannotate) [![Coverage Status](http://img.shields.io/coveralls/omsmith/browserify-ngannotate.svg)](https://coveralls.io/r/omsmith/browserify-ngannotate)

A [browserify](http://github.com/substack/node-browserify) transform that uses [ng-annotate](https://github.com/olov/ng-annotate) to add dependency injection annotations to your AngularJS source code, preparing it for minification.

# Usage
```
browserify -t browserify-ngannotate app.js > bundle.js
```

## Options
Provided options are passed through to ng-annotate. The `add` option defaults
to `true`.

For example, to remove annotations, one could use the following:

```
browserify -t [ browserify-ngannotate --no-add --remove ] app.js > bundle.js
```

# Install
```
npm install browserify-ngannotate --save
```

# License
MIT
