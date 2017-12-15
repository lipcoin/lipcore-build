# lipcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install lipcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var lipcoreTasks = require('lipcore-build');

lipcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var lipcoreTasks = require('lipcore-build');
lipcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/lipcoin/lipcore) on the main lipcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/lipcoin/lipcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2016 The Lipcoin Core Developers
Copyright 2017 The Lipcoin Core Developers