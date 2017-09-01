Btccore Build
======

A helper to add tasks to gulp.

## Attribution

This repository was created by copy forking [bitcore-build 6747a4a](https://github.com/bitpay/bitcore-build/commit/6747a4a15a0154de294d2591c5603969ad30eea1).

## Getting started

Install with:

```sh
npm install btccore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var btccoreTasks = require('btccore-build');

btccoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var btccoreTasks = require('btccore-build');
btccoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/owstack/btccore-lib) on the main btccore-lib repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/owstack/btccore-lib/blob/master/LICENSE).

Copyright 2017 Open Wallet Stack. Btccore is a trademark maintained by Open Wallet Stack.
