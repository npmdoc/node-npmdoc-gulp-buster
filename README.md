# api documentation for  [gulp-buster (v1.1.0)](https://github.com/UltCombo/gulp-buster)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-buster.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-buster) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-buster.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-buster)
#### Cache buster hashes generator for gulp. Blazing fast and fully configurable.

[![NPM](https://nodei.co/npm/gulp-buster.png?downloads=true)](https://www.npmjs.com/package/gulp-buster)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-buster/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-buster_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-buster/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-buster/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-buster/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ult Combo",
        "email": "ultcombo@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/UltCombo/gulp-buster/issues"
    },
    "dependencies": {
        "bluebird": "^3.3.5",
        "gulp-util": "^3.0.7",
        "lodash.defaults": "^4.0.1",
        "object-assign": "^4.0.1",
        "through": "^2.3.8"
    },
    "description": "Cache buster hashes generator for gulp. Blazing fast and fully configurable.",
    "devDependencies": {
        "istanbul": "^0.4.3",
        "mocha": "^2.4.5",
        "should": "^8.3.1"
    },
    "directories": {},
    "dist": {
        "shasum": "f58afae8051725fbe86792b2ff95637c38c7de1e",
        "tarball": "https://registry.npmjs.org/gulp-buster/-/gulp-buster-1.1.0.tgz"
    },
    "engines": {
        "node": ">= 0.10"
    },
    "gitHead": "86bd6b3340327f6eb19b0e25d7a01faa2dd9a99f",
    "homepage": "https://github.com/UltCombo/gulp-buster",
    "keywords": [
        "gulpplugin",
        "cachebuster",
        "cache buster",
        "cache",
        "fingerprint",
        "fingerprinting",
        "revision",
        "revisioning",
        "workflow",
        "webdev",
        "web development"
    ],
    "license": "WTFPL",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "ult_combo",
            "email": "ultcombo@gmail.com"
        }
    ],
    "name": "gulp-buster",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/UltCombo/gulp-buster.git"
    },
    "scripts": {
        "test": "mocha",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha -- -R dot",
        "test-travis": "istanbul cover node_modules/mocha/bin/_mocha --report lcovonly"
    },
    "version": "1.1.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-buster](#apidoc.module.gulp-buster)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise (executor)](#apidoc.element.gulp-buster._Promise)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.AggregateError (message)](#apidoc.element.gulp-buster._Promise.AggregateError)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.CancellationError (message)](#apidoc.element.gulp-buster._Promise.CancellationError)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.OperationalError (message)](#apidoc.element.gulp-buster._Promise.OperationalError)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.PromiseInspection (promise)](#apidoc.element.gulp-buster._Promise.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.TimeoutError (message)](#apidoc.element.gulp-buster._Promise.TimeoutError)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise._SomePromiseArray (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.coroutine (generatorFunction, options)](#apidoc.element.gulp-buster._Promise.coroutine)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_assignOptions (options)](#apidoc.element.gulp-buster._assignOptions)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_error (msg)](#apidoc.element.gulp-buster._error)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_getType (value)](#apidoc.element.gulp-buster._getType)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_hash (file, options)](#apidoc.element.gulp-buster._hash)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_relativePath (projectPath, relativePath, filePath)](#apidoc.element.gulp-buster._relativePath)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_reset ()](#apidoc.element.gulp-buster._reset)
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_DEFAULT_OPTIONS
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.AggregateError.prototype
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.CancellationError.prototype
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.OperationalError.prototype
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.PromiseInspection.prototype
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.TimeoutError.prototype
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_Promise._SomePromiseArray.prototype
1.  object <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.prototype

#### [module gulp-buster._DEFAULT_OPTIONS](#apidoc.module.gulp-buster._DEFAULT_OPTIONS)
1.  [function <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>formatter ()](#apidoc.element.gulp-buster._DEFAULT_OPTIONS.formatter)
1.  [function <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>transform ()](#apidoc.element.gulp-buster._DEFAULT_OPTIONS.transform)
1.  number <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>length
1.  string <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>algo
1.  string <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>fileName
1.  string <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>relativePath

#### [module gulp-buster._Promise](#apidoc.module.gulp-buster._Promise)
1.  [function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise (executor)](#apidoc.element.gulp-buster._Promise._Promise)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>AggregateError (message)](#apidoc.element.gulp-buster._Promise.AggregateError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>CancellationError (message)](#apidoc.element.gulp-buster._Promise.CancellationError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>OperationalError (message)](#apidoc.element.gulp-buster._Promise.OperationalError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>Promise (executor)](#apidoc.element.gulp-buster._Promise.Promise)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>PromiseInspection (promise)](#apidoc.element.gulp-buster._Promise.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>RangeError ()](#apidoc.element.gulp-buster._Promise.RangeError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>RejectionError (message)](#apidoc.element.gulp-buster._Promise.RejectionError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>TimeoutError (message)](#apidoc.element.gulp-buster._Promise.TimeoutError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>TypeError ()](#apidoc.element.gulp-buster._Promise.TypeError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>_SomePromiseArray (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>_peekContext ()](#apidoc.element.gulp-buster._Promise._peekContext)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>all (promises)](#apidoc.element.gulp-buster._Promise.all)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>any (promises)](#apidoc.element.gulp-buster._Promise.any)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>attempt (fn)](#apidoc.element.gulp-buster._Promise.attempt)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>bind (thisArg, value)](#apidoc.element.gulp-buster._Promise.bind)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>cast (obj)](#apidoc.element.gulp-buster._Promise.cast)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>config (opts)](#apidoc.element.gulp-buster._Promise.config)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>coroutine (generatorFunction, options)](#apidoc.element.gulp-buster._Promise.coroutine)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>defer ()](#apidoc.element.gulp-buster._Promise.defer)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>delay (ms, value)](#apidoc.element.gulp-buster._Promise.delay)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>each (promises, fn)](#apidoc.element.gulp-buster._Promise.each)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>filter (promises, fn, options)](#apidoc.element.gulp-buster._Promise.filter)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>fromCallback (fn)](#apidoc.element.gulp-buster._Promise.fromCallback)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>fromNode (fn)](#apidoc.element.gulp-buster._Promise.fromNode)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>fulfilled (obj)](#apidoc.element.gulp-buster._Promise.fulfilled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>getNewLibraryCopy ()](#apidoc.element.gulp-buster._Promise.getNewLibraryCopy)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>hasLongStackTraces ()](#apidoc.element.gulp-buster._Promise.hasLongStackTraces)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>is (val)](#apidoc.element.gulp-buster._Promise.is)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>join ()](#apidoc.element.gulp-buster._Promise.join)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>longStackTraces ()](#apidoc.element.gulp-buster._Promise.longStackTraces)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>map (promises, fn, options, _filter)](#apidoc.element.gulp-buster._Promise.map)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>mapSeries (promises, fn)](#apidoc.element.gulp-buster._Promise.mapSeries)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>method (fn)](#apidoc.element.gulp-buster._Promise.method)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>noConflict ()](#apidoc.element.gulp-buster._Promise.noConflict)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>onPossiblyUnhandledRejection (fn)](#apidoc.element.gulp-buster._Promise.onPossiblyUnhandledRejection)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>onUnhandledRejectionHandled (fn)](#apidoc.element.gulp-buster._Promise.onUnhandledRejectionHandled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>pending ()](#apidoc.element.gulp-buster._Promise.pending)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>promisify (fn, options)](#apidoc.element.gulp-buster._Promise.promisify)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>promisifyAll (target, options)](#apidoc.element.gulp-buster._Promise.promisifyAll)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>props (promises)](#apidoc.element.gulp-buster._Promise.props)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>race (promises)](#apidoc.element.gulp-buster._Promise.race)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>reduce (promises, fn, initialValue, _each)](#apidoc.element.gulp-buster._Promise.reduce)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>reject (reason)](#apidoc.element.gulp-buster._Promise.reject)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>rejected (reason)](#apidoc.element.gulp-buster._Promise.rejected)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>resolve (obj)](#apidoc.element.gulp-buster._Promise.resolve)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>setScheduler (fn)](#apidoc.element.gulp-buster._Promise.setScheduler)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>settle (promises)](#apidoc.element.gulp-buster._Promise.settle)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>some (promises, howMany)](#apidoc.element.gulp-buster._Promise.some)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>spawn (generatorFunction)](#apidoc.element.gulp-buster._Promise.spawn)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>try (fn)](#apidoc.element.gulp-buster._Promise.try)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>using ()](#apidoc.element.gulp-buster._Promise.using)
1.  string <span class="apidocSignatureSpan">gulp-buster._Promise.</span>version

#### [module gulp-buster._Promise.AggregateError](#apidoc.module.gulp-buster._Promise.AggregateError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>AggregateError (message)](#apidoc.element.gulp-buster._Promise.AggregateError.AggregateError)

#### [module gulp-buster._Promise.AggregateError.prototype](#apidoc.module.gulp-buster._Promise.AggregateError.prototype)
1.  boolean <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>isOperational
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>every ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.every)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>filter ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.filter)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>forEach ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>indexOf ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>join ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.join)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>lastIndexOf ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>map ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.map)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>pop ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.pop)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>push ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.push)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>reduce ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>reduceRight ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>reverse ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>shift ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.shift)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>slice ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.slice)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>some ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.some)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>sort ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.sort)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>toString ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.toString)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>unshift ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.unshift)
1.  number <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>length

#### [module gulp-buster._Promise.CancellationError](#apidoc.module.gulp-buster._Promise.CancellationError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>CancellationError (message)](#apidoc.element.gulp-buster._Promise.CancellationError.CancellationError)

#### [module gulp-buster._Promise.CancellationError.prototype](#apidoc.module.gulp-buster._Promise.CancellationError.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.CancellationError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.CancellationError.prototype.constructor)

#### [module gulp-buster._Promise.OperationalError](#apidoc.module.gulp-buster._Promise.OperationalError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>OperationalError (message)](#apidoc.element.gulp-buster._Promise.OperationalError.OperationalError)

#### [module gulp-buster._Promise.OperationalError.prototype](#apidoc.module.gulp-buster._Promise.OperationalError.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.OperationalError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.OperationalError.prototype.constructor)

#### [module gulp-buster._Promise.PromiseInspection](#apidoc.module.gulp-buster._Promise.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>PromiseInspection (promise)](#apidoc.element.gulp-buster._Promise.PromiseInspection.PromiseInspection)

#### [module gulp-buster._Promise.PromiseInspection.prototype](#apidoc.module.gulp-buster._Promise.PromiseInspection.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>_settledValue ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype._settledValue)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>error ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.error)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isCancelled ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isFulfilled ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isFulfilled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isPending ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isPending)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isRejected ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isRejected)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isResolved ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isResolved)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>reason ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.reason)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>value ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.value)

#### [module gulp-buster._Promise.TimeoutError](#apidoc.module.gulp-buster._Promise.TimeoutError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>TimeoutError (message)](#apidoc.element.gulp-buster._Promise.TimeoutError.TimeoutError)

#### [module gulp-buster._Promise.TimeoutError.prototype](#apidoc.module.gulp-buster._Promise.TimeoutError.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.TimeoutError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.TimeoutError.prototype.constructor)

#### [module gulp-buster._Promise._SomePromiseArray](#apidoc.module.gulp-buster._Promise._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>_SomePromiseArray (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray._SomePromiseArray)

#### [module gulp-buster._Promise._SomePromiseArray.prototype](#apidoc.module.gulp-buster._Promise._SomePromiseArray.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_addFulfilled (value)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._addFulfilled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_addRejected (reason)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._addRejected)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_canPossiblyFulfill ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._canPossiblyFulfill)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_checkOutcome ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._checkOutcome)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_fulfilled ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._fulfilled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_getRangeError (count)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._getRangeError)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_init ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._init)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_promiseCancelled ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_promiseFulfilled (value)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseFulfilled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_promiseRejected (reason)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseRejected)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_rejected ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._rejected)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_resolveEmptyArray ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._resolveEmptyArray)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>constructor (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>howMany ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.howMany)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>init ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.init)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>setHowMany (count)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.setHowMany)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>setUnwrap ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.setUnwrap)

#### [module gulp-buster._Promise.coroutine](#apidoc.module.gulp-buster._Promise.coroutine)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>coroutine (generatorFunction, options)](#apidoc.element.gulp-buster._Promise.coroutine.coroutine)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.coroutine.</span>addYieldHandler (fn)](#apidoc.element.gulp-buster._Promise.coroutine.addYieldHandler)

#### [module gulp-buster._Promise.prototype](#apidoc.module.gulp-buster._Promise.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>__isCancelled ()](#apidoc.element.gulp-buster._Promise.prototype.__isCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_addCallbacks ( fulfill, reject, promise, receiver, domain )](#apidoc.element.gulp-buster._Promise.prototype._addCallbacks)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_attachCancellationCallback (onCancel)](#apidoc.element.gulp-buster._Promise.prototype._attachCancellationCallback)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_attachExtraTrace ()](#apidoc.element.gulp-buster._Promise.prototype._attachExtraTrace)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_boundValue ()](#apidoc.element.gulp-buster._Promise.prototype._boundValue)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_branchHasCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._branchHasCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancel ()](#apidoc.element.gulp-buster._Promise.prototype._cancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancelBranched ()](#apidoc.element.gulp-buster._Promise.prototype._cancelBranched)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancelBy (canceller)](#apidoc.element.gulp-buster._Promise.prototype._cancelBy)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancelPromises ()](#apidoc.element.gulp-buster._Promise.prototype._cancelPromises)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_captureStackTrace ()](#apidoc.element.gulp-buster._Promise.prototype._captureStackTrace)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_clearCallbackDataAtIndex (index)](#apidoc.element.gulp-buster._Promise.prototype._clearCallbackDataAtIndex)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_clearCancellationData ()](#apidoc.element.gulp-buster._Promise.prototype._clearCancellationData)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_doInvokeOnCancel (onCancelCallback, internalOnly)](#apidoc.element.gulp-buster._Promise.prototype._doInvokeOnCancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_enoughBranchesHaveCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._enoughBranchesHaveCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_ensurePossibleRejectionHandled ()](#apidoc.element.gulp-buster._Promise.prototype._ensurePossibleRejectionHandled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_execute (executor, resolve, reject)](#apidoc.element.gulp-buster._Promise.prototype._execute)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fireEvent ()](#apidoc.element.gulp-buster._Promise.prototype._fireEvent)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_followee ()](#apidoc.element.gulp-buster._Promise.prototype._followee)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fulfill (value)](#apidoc.element.gulp-buster._Promise.prototype._fulfill)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fulfillPromises (len, value)](#apidoc.element.gulp-buster._Promise.prototype._fulfillPromises)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fulfillmentHandlerAt (index)](#apidoc.element.gulp-buster._Promise.prototype._fulfillmentHandlerAt)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_getDisposer ()](#apidoc.element.gulp-buster._Promise.prototype._getDisposer)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_invokeInternalOnCancel ()](#apidoc.element.gulp-buster._Promise.prototype._invokeInternalOnCancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_invokeOnCancel ()](#apidoc.element.gulp-buster._Promise.prototype._invokeOnCancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isBound ()](#apidoc.element.gulp-buster._Promise.prototype._isBound)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isCancellable ()](#apidoc.element.gulp-buster._Promise.prototype._isCancellable)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._isCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isDisposable ()](#apidoc.element.gulp-buster._Promise.prototype._isDisposable)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isFateSealed ()](#apidoc.element.gulp-buster._Promise.prototype._isFateSealed)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isFinal ()](#apidoc.element.gulp-buster._Promise.prototype._isFinal)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isFollowing ()](#apidoc.element.gulp-buster._Promise.prototype._isFollowing)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isRejectionUnhandled ()](#apidoc.element.gulp-buster._Promise.prototype._isRejectionUnhandled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isUnhandledRejectionNotified ()](#apidoc.element.gulp-buster._Promise.prototype._isUnhandledRejectionNotified)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_length ()](#apidoc.element.gulp-buster._Promise.prototype._length)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_migrateCallback0 (follower)](#apidoc.element.gulp-buster._Promise.prototype._migrateCallback0)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_migrateCallbackAt (follower, index)](#apidoc.element.gulp-buster._Promise.prototype._migrateCallbackAt)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_notifyUnhandledRejection ()](#apidoc.element.gulp-buster._Promise.prototype._notifyUnhandledRejection)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_notifyUnhandledRejectionIsHandled ()](#apidoc.element.gulp-buster._Promise.prototype._notifyUnhandledRejectionIsHandled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_onCancel ()](#apidoc.element.gulp-buster._Promise.prototype._onCancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_passThrough (handler, type, success, fail)](#apidoc.element.gulp-buster._Promise.prototype._passThrough)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_peekContext ()](#apidoc.element.gulp-buster._Promise.prototype._peekContext)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_popContext ()](#apidoc.element.gulp-buster._Promise.prototype._popContext)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_promiseAt (index)](#apidoc.element.gulp-buster._Promise.prototype._promiseAt)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_promiseCreated ()](#apidoc.element.gulp-buster._Promise.prototype._promiseCreated)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_propagateFrom (parent, flags)](#apidoc.element.gulp-buster._Promise.prototype._propagateFrom)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_proxy (proxyable, arg)](#apidoc.element.gulp-buster._Promise.prototype._proxy)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_pushContext ()](#apidoc.element.gulp-buster._Promise.prototype._pushContext)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_reason ()](#apidoc.element.gulp-buster._Promise.prototype._reason)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_receiverAt (index)](#apidoc.element.gulp-buster._Promise.prototype._receiverAt)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_reject (reason)](#apidoc.element.gulp-buster._Promise.prototype._reject)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_rejectCallback (reason, synchronous, ignoreNonErrorWarnings)](#apidoc.element.gulp-buster._Promise.prototype._rejectCallback)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_rejectPromises (len, reason)](#apidoc.element.gulp-buster._Promise.prototype._rejectPromises)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_rejectionHandlerAt (index)](#apidoc.element.gulp-buster._Promise.prototype._rejectionHandlerAt)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resolveCallback (value, shouldBind)](#apidoc.element.gulp-buster._Promise.prototype._resolveCallback)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resolveFromExecutor (executor)](#apidoc.element.gulp-buster._Promise.prototype._resolveFromExecutor)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resolveFromSyncValue (value)](#apidoc.element.gulp-buster._Promise.prototype._resolveFromSyncValue)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resultCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._resultCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_returnedNonUndefined ()](#apidoc.element.gulp-buster._Promise.prototype._returnedNonUndefined)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setAsyncGuaranteed ()](#apidoc.element.gulp-buster._Promise.prototype._setAsyncGuaranteed)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setBoundTo (obj)](#apidoc.element.gulp-buster._Promise.prototype._setBoundTo)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._setCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setDisposable (disposer)](#apidoc.element.gulp-buster._Promise.prototype._setDisposable)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setFollowee (promise)](#apidoc.element.gulp-buster._Promise.prototype._setFollowee)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setFollowing ()](#apidoc.element.gulp-buster._Promise.prototype._setFollowing)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setFulfilled ()](#apidoc.element.gulp-buster._Promise.prototype._setFulfilled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setIsFinal ()](#apidoc.element.gulp-buster._Promise.prototype._setIsFinal)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setLength (len)](#apidoc.element.gulp-buster._Promise.prototype._setLength)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setOnCancel (handler)](#apidoc.element.gulp-buster._Promise.prototype._setOnCancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setRejected ()](#apidoc.element.gulp-buster._Promise.prototype._setRejected)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setRejectionIsUnhandled ()](#apidoc.element.gulp-buster._Promise.prototype._setRejectionIsUnhandled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setReturnedNonUndefined ()](#apidoc.element.gulp-buster._Promise.prototype._setReturnedNonUndefined)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setUnhandledRejectionIsNotified ()](#apidoc.element.gulp-buster._Promise.prototype._setUnhandledRejectionIsNotified)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setWillBeCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._setWillBeCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromise (promise, handler, receiver, value)](#apidoc.element.gulp-buster._Promise.prototype._settlePromise)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromise0 (handler, value, bitField)](#apidoc.element.gulp-buster._Promise.prototype._settlePromise0)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromiseCtx (ctx)](#apidoc.element.gulp-buster._Promise.prototype._settlePromiseCtx)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromiseFromHandler ( handler, receiver, value, promise )](#apidoc.element.gulp-buster._Promise.prototype._settlePromiseFromHandler)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromiseLateCancellationObserver (ctx)](#apidoc.element.gulp-buster._Promise.prototype._settlePromiseLateCancellationObserver)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromises ()](#apidoc.element.gulp-buster._Promise.prototype._settlePromises)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settledValue ()](#apidoc.element.gulp-buster._Promise.prototype._settledValue)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_target ()](#apidoc.element.gulp-buster._Promise.prototype._target)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_then ( didFulfill, didReject, _, receiver, internalData )](#apidoc.element.gulp-buster._Promise.prototype._then)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._unsetCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetDisposable ()](#apidoc.element.gulp-buster._Promise.prototype._unsetDisposable)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetOnCancel ()](#apidoc.element.gulp-buster._Promise.prototype._unsetOnCancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetRejectionIsUnhandled ()](#apidoc.element.gulp-buster._Promise.prototype._unsetRejectionIsUnhandled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetUnhandledRejectionIsNotified ()](#apidoc.element.gulp-buster._Promise.prototype._unsetUnhandledRejectionIsNotified)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_value ()](#apidoc.element.gulp-buster._Promise.prototype._value)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_warn (message, shouldUseOwnTrace, promise)](#apidoc.element.gulp-buster._Promise.prototype._warn)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>all ()](#apidoc.element.gulp-buster._Promise.prototype.all)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>any ()](#apidoc.element.gulp-buster._Promise.prototype.any)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>asCallback (nodeback, options)](#apidoc.element.gulp-buster._Promise.prototype.asCallback)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>bind (thisArg)](#apidoc.element.gulp-buster._Promise.prototype.bind)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>break ()](#apidoc.element.gulp-buster._Promise.prototype.break)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>call (methodName)](#apidoc.element.gulp-buster._Promise.prototype.call)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>cancel ()](#apidoc.element.gulp-buster._Promise.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>catch (fn)](#apidoc.element.gulp-buster._Promise.prototype.catch)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>catchReturn (value)](#apidoc.element.gulp-buster._Promise.prototype.catchReturn)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>catchThrow (reason)](#apidoc.element.gulp-buster._Promise.prototype.catchThrow)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>caught (fn)](#apidoc.element.gulp-buster._Promise.prototype.caught)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>delay (ms)](#apidoc.element.gulp-buster._Promise.prototype.delay)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>disposer (fn)](#apidoc.element.gulp-buster._Promise.prototype.disposer)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>done (didFulfill, didReject)](#apidoc.element.gulp-buster._Promise.prototype.done)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>each (fn)](#apidoc.element.gulp-buster._Promise.prototype.each)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>error (fn)](#apidoc.element.gulp-buster._Promise.prototype.error)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>filter (fn, options)](#apidoc.element.gulp-buster._Promise.prototype.filter)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>finally (handler)](#apidoc.element.gulp-buster._Promise.prototype.finally)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>get (propertyName)](#apidoc.element.gulp-buster._Promise.prototype.get)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isCancellable ()](#apidoc.element.gulp-buster._Promise.prototype.isCancellable)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isCancelled ()](#apidoc.element.gulp-buster._Promise.prototype.isCancelled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isFulfilled ()](#apidoc.element.gulp-buster._Promise.prototype.isFulfilled)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isPending ()](#apidoc.element.gulp-buster._Promise.prototype.isPending)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isRejected ()](#apidoc.element.gulp-buster._Promise.prototype.isRejected)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isResolved ()](#apidoc.element.gulp-buster._Promise.prototype.isResolved)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>lastly (handler)](#apidoc.element.gulp-buster._Promise.prototype.lastly)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>map (fn, options)](#apidoc.element.gulp-buster._Promise.prototype.map)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>mapSeries (fn)](#apidoc.element.gulp-buster._Promise.prototype.mapSeries)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>nodeify (nodeback, options)](#apidoc.element.gulp-buster._Promise.prototype.nodeify)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>props ()](#apidoc.element.gulp-buster._Promise.prototype.props)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>race ()](#apidoc.element.gulp-buster._Promise.prototype.race)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>reason ()](#apidoc.element.gulp-buster._Promise.prototype.reason)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>reduce (fn, initialValue)](#apidoc.element.gulp-buster._Promise.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>reflect ()](#apidoc.element.gulp-buster._Promise.prototype.reflect)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>return (value)](#apidoc.element.gulp-buster._Promise.prototype.return)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>settle ()](#apidoc.element.gulp-buster._Promise.prototype.settle)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>some (howMany)](#apidoc.element.gulp-buster._Promise.prototype.some)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>spread (fn)](#apidoc.element.gulp-buster._Promise.prototype.spread)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>suppressUnhandledRejections ()](#apidoc.element.gulp-buster._Promise.prototype.suppressUnhandledRejections)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>tap (handler)](#apidoc.element.gulp-buster._Promise.prototype.tap)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>tapCatch (handlerOrPredicate)](#apidoc.element.gulp-buster._Promise.prototype.tapCatch)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>then (didFulfill, didReject)](#apidoc.element.gulp-buster._Promise.prototype.then)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>thenReturn (value)](#apidoc.element.gulp-buster._Promise.prototype.thenReturn)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>thenThrow (reason)](#apidoc.element.gulp-buster._Promise.prototype.thenThrow)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>throw (reason)](#apidoc.element.gulp-buster._Promise.prototype.throw)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>timeout (ms, message)](#apidoc.element.gulp-buster._Promise.prototype.timeout)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>toJSON ()](#apidoc.element.gulp-buster._Promise.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>toString ()](#apidoc.element.gulp-buster._Promise.prototype.toString)
1.  [function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>value ()](#apidoc.element.gulp-buster._Promise.prototype.value)



# <a name="apidoc.module.gulp-buster"></a>[module gulp-buster](#apidoc.module.gulp-buster)

#### <a name="apidoc.element.gulp-buster._Promise"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise (executor)](#apidoc.element.gulp-buster._Promise)
- description and source-code
```javascript
function Promise(executor) {
    if (executor !== INTERNAL) {
        check(this, executor);
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._resolveFromExecutor(executor);
    this._promiseCreated();
    this._fireEvent("promiseCreated", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.AggregateError (message)](#apidoc.element.gulp-buster._Promise.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.CancellationError"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.CancellationError (message)](#apidoc.element.gulp-buster._Promise.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.OperationalError"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.OperationalError (message)](#apidoc.element.gulp-buster._Promise.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.PromiseInspection (promise)](#apidoc.element.gulp-buster._Promise.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValueField = promise._isFateSealed()
            ? promise._settledValue() : undefined;
    }
    else {
        this._bitField = 0;
        this._settledValueField = undefined;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.TimeoutError"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.TimeoutError (message)](#apidoc.element.gulp-buster._Promise.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise._SomePromiseArray (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.coroutine"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise.coroutine (generatorFunction, options)](#apidoc.element.gulp-buster._Promise.coroutine)
- description and source-code
```javascript
_Promise.coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        var ret = spawn.promise();
        spawn._generator = generator;
        spawn._promiseFulfilled(undefined);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._assignOptions"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_assignOptions (options)](#apidoc.element.gulp-buster._assignOptions)
- description and source-code
```javascript
function assignOptions(options) {
	if (typeof options === 'string') options = { fileName: options };
	options = options || {};

	Object.keys(options).forEach(function(option) {
		if (!OPTION_TYPES.hasOwnProperty(option)) throw error('Unsupported option: ' + option);
		if (options[option] !== undefined && OPTION_TYPES[option].indexOf(getType(options[option])) === -1) throw error(''options.' +
option + '' must be of type ' + OPTION_TYPES[option].join(' or '));
	});

	return defaults({}, options, DEFAULT_OPTIONS);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._error"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_error (msg)](#apidoc.element.gulp-buster._error)
- description and source-code
```javascript
function error(msg) {
	return new gutil.PluginError('gulp-buster', msg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._getType"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_getType (value)](#apidoc.element.gulp-buster._getType)
- description and source-code
```javascript
function getType(value) {
	return {}.toString.call(value).slice(8, -1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._hash"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_hash (file, options)](#apidoc.element.gulp-buster._hash)
- description and source-code
```javascript
function hash(file, options) {
	return typeof options.algo === 'function'
		? options.algo.call(undefined, file)
		: crypto.createHash(options.algo).update(file.contents).digest('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._relativePath"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_relativePath (projectPath, relativePath, filePath)](#apidoc.element.gulp-buster._relativePath)
- description and source-code
```javascript
function relativePath(projectPath, relativePath, filePath) {
	return path.relative(path.join(projectPath, relativePath), filePath).replace(/\\/g, '/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._reset"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_reset ()](#apidoc.element.gulp-buster._reset)
- description and source-code
```javascript
_reset = function () {
		hashesStore = {};
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._DEFAULT_OPTIONS"></a>[module gulp-buster._DEFAULT_OPTIONS](#apidoc.module.gulp-buster._DEFAULT_OPTIONS)

#### <a name="apidoc.element.gulp-buster._DEFAULT_OPTIONS.formatter"></a>[function <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>formatter ()](#apidoc.element.gulp-buster._DEFAULT_OPTIONS.formatter)
- description and source-code
```javascript
function stringify() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._DEFAULT_OPTIONS.transform"></a>[function <span class="apidocSignatureSpan">gulp-buster._DEFAULT_OPTIONS.</span>transform ()](#apidoc.element.gulp-buster._DEFAULT_OPTIONS.transform)
- description and source-code
```javascript
function Object() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise"></a>[module gulp-buster._Promise](#apidoc.module.gulp-buster._Promise)

#### <a name="apidoc.element.gulp-buster._Promise._Promise"></a>[function <span class="apidocSignatureSpan">gulp-buster.</span>_Promise (executor)](#apidoc.element.gulp-buster._Promise._Promise)
- description and source-code
```javascript
function Promise(executor) {
    if (executor !== INTERNAL) {
        check(this, executor);
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._resolveFromExecutor(executor);
    this._promiseCreated();
    this._fireEvent("promiseCreated", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>AggregateError (message)](#apidoc.element.gulp-buster._Promise.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.CancellationError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>CancellationError (message)](#apidoc.element.gulp-buster._Promise.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.OperationalError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>OperationalError (message)](#apidoc.element.gulp-buster._Promise.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.Promise"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>Promise (executor)](#apidoc.element.gulp-buster._Promise.Promise)
- description and source-code
```javascript
function Promise(executor) {
    if (executor !== INTERNAL) {
        check(this, executor);
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._resolveFromExecutor(executor);
    this._promiseCreated();
    this._fireEvent("promiseCreated", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>PromiseInspection (promise)](#apidoc.element.gulp-buster._Promise.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValueField = promise._isFateSealed()
            ? promise._settledValue() : undefined;
    }
    else {
        this._bitField = 0;
        this._settledValueField = undefined;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.RangeError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>RangeError ()](#apidoc.element.gulp-buster._Promise.RangeError)
- description and source-code
```javascript
function RangeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.RejectionError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>RejectionError (message)](#apidoc.element.gulp-buster._Promise.RejectionError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.TimeoutError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>TimeoutError (message)](#apidoc.element.gulp-buster._Promise.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.TypeError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>TypeError ()](#apidoc.element.gulp-buster._Promise.TypeError)
- description and source-code
```javascript
function TypeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>_SomePromiseArray (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._peekContext"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>_peekContext ()](#apidoc.element.gulp-buster._Promise._peekContext)
- description and source-code
```javascript
_peekContext = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.all"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>all (promises)](#apidoc.element.gulp-buster._Promise.all)
- description and source-code
```javascript
all = function (promises) {
    return new PromiseArray(promises).promise();
}
```
- example usage
```shell
...
				if (typeof hashed !== 'string') throw error('Return/fulfill value of 'options.algo' must be a string');
				hashes[relativePath(file.cwd, options.relativePath, file.path)] = sliceHash(hashed, options);
			})
		);
	}

	function endStream() {
		Promise.all(hashingPromises).bind(this).then(function() {
			return options.transform.call(undefined, assign({}, hashes));
		}).then(function(transformed) {
			return options.formatter.call(undefined, transformed);
		}).then(function(formatted) {
			if (typeof formatted !== 'string') throw error('Return/fulfill value of 'options.formatter' must be a string');

			this.emit('data', new gutil.File({
...
```

#### <a name="apidoc.element.gulp-buster._Promise.any"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>any (promises)](#apidoc.element.gulp-buster._Promise.any)
- description and source-code
```javascript
any = function (promises) {
    return any(promises);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.attempt"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>attempt (fn)](#apidoc.element.gulp-buster._Promise.attempt)
- description and source-code
```javascript
attempt = function (fn) {
    if (typeof fn !== "function") {
        return apiRejection("expecting a function but got " + util.classString(fn));
    }
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._pushContext();
    var value;
    if (arguments.length > 1) {
        debug.deprecated("calling Promise.try with more than 1 argument");
        var arg = arguments[1];
        var ctx = arguments[2];
        value = util.isArray(arg) ? tryCatch(fn).apply(ctx, arg)
                                  : tryCatch(fn).call(ctx, arg);
    } else {
        value = tryCatch(fn)();
    }
    var promiseCreated = ret._popContext();
    debug.checkForgottenReturns(
        value, promiseCreated, "Promise.try", ret);
    ret._resolveFromSyncValue(value);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.bind"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>bind (thisArg, value)](#apidoc.element.gulp-buster._Promise.bind)
- description and source-code
```javascript
bind = function (thisArg, value) {
    return Promise.resolve(value).bind(thisArg);
}
```
- example usage
```shell
...

	function hashFile(file) {
		if (file.isNull()) return; // ignore
		if (file.isStream()) return this.emit('error', error('Streaming not supported'));

		// start hashing files as soon as they are received for maximum concurrency
		hashingPromises.push(
			Promise.try(hash.bind(undefined, file, options)).then(function(hashed) {
				if (typeof hashed !== 'string') throw error('Return/fulfill value of 'options.algo' must be a string');
				hashes[relativePath(file.cwd, options.relativePath, file.path)] = sliceHash(hashed, options);
			})
		);
	}

	function endStream() {
...
```

#### <a name="apidoc.element.gulp-buster._Promise.cast"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>cast (obj)](#apidoc.element.gulp-buster._Promise.cast)
- description and source-code
```javascript
cast = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._setFulfilled();
        ret._rejectionHandler0 = obj;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.config"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>config (opts)](#apidoc.element.gulp-buster._Promise.config)
- description and source-code
```javascript
config = function (opts) {
    opts = Object(opts);
    if ("longStackTraces" in opts) {
        if (opts.longStackTraces) {
            Promise.longStackTraces();
        } else if (!opts.longStackTraces && Promise.hasLongStackTraces()) {
            disableLongStackTraces();
        }
    }
    if ("warnings" in opts) {
        var warningsOption = opts.warnings;
        config.warnings = !!warningsOption;
        wForgottenReturn = config.warnings;

        if (util.isObject(warningsOption)) {
            if ("wForgottenReturn" in warningsOption) {
                wForgottenReturn = !!warningsOption.wForgottenReturn;
            }
        }
    }
    if ("cancellation" in opts && opts.cancellation && !config.cancellation) {
        if (async.haveItemsQueued()) {
            throw new Error(
                "cannot enable cancellation after promises are in use");
        }
        Promise.prototype._clearCancellationData =
            cancellationClearCancellationData;
        Promise.prototype._propagateFrom = cancellationPropagateFrom;
        Promise.prototype._onCancel = cancellationOnCancel;
        Promise.prototype._setOnCancel = cancellationSetOnCancel;
        Promise.prototype._attachCancellationCallback =
            cancellationAttachCancellationCallback;
        Promise.prototype._execute = cancellationExecute;
        propagateFromFunction = cancellationPropagateFrom;
        config.cancellation = true;
    }
    if ("monitoring" in opts) {
        if (opts.monitoring && !config.monitoring) {
            config.monitoring = true;
            Promise.prototype._fireEvent = activeFireEvent;
        } else if (!opts.monitoring && config.monitoring) {
            config.monitoring = false;
            Promise.prototype._fireEvent = defaultFireEvent;
        }
    }
    return Promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.coroutine"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>coroutine (generatorFunction, options)](#apidoc.element.gulp-buster._Promise.coroutine)
- description and source-code
```javascript
coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        var ret = spawn.promise();
        spawn._generator = generator;
        spawn._promiseFulfilled(undefined);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.defer"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>defer ()](#apidoc.element.gulp-buster._Promise.defer)
- description and source-code
```javascript
defer = function () {
    debug.deprecated("Promise.defer", "new Promise");
    var promise = new Promise(INTERNAL);
    return {
        promise: promise,
        resolve: deferResolve,
        reject: deferReject
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.delay"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>delay (ms, value)](#apidoc.element.gulp-buster._Promise.delay)
- description and source-code
```javascript
delay = function (ms, value) {
    var ret;
    var handle;
    if (value !== undefined) {
        ret = Promise.resolve(value)
                ._then(afterValue, null, null, ms, undefined);
        if (debug.cancellation() && value instanceof Promise) {
            ret._setOnCancel(value);
        }
    } else {
        ret = new Promise(INTERNAL);
        handle = setTimeout(function() { ret._fulfill(); }, +ms);
        if (debug.cancellation()) {
            ret._setOnCancel(new HandleWrapper(handle));
        }
        ret._captureStackTrace();
    }
    ret._setAsyncGuaranteed();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.each"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>each (promises, fn)](#apidoc.element.gulp-buster._Promise.each)
- description and source-code
```javascript
each = function (promises, fn) {
    return PromiseReduce(promises, fn, INTERNAL, 0)
              ._then(promiseAllThis, undefined, undefined, promises, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.filter"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>filter (promises, fn, options)](#apidoc.element.gulp-buster._Promise.filter)
- description and source-code
```javascript
filter = function (promises, fn, options) {
    return PromiseMap(promises, fn, options, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.fromCallback"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>fromCallback (fn)](#apidoc.element.gulp-buster._Promise.fromCallback)
- description and source-code
```javascript
fromCallback = function (fn) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    var multiArgs = arguments.length > 1 ? !!Object(arguments[1]).multiArgs
                                         : false;
    var result = tryCatch(fn)(nodebackForPromise(ret, multiArgs));
    if (result === errorObj) {
        ret._rejectCallback(result.e, true);
    }
    if (!ret._isFateSealed()) ret._setAsyncGuaranteed();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.fromNode"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>fromNode (fn)](#apidoc.element.gulp-buster._Promise.fromNode)
- description and source-code
```javascript
fromNode = function (fn) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    var multiArgs = arguments.length > 1 ? !!Object(arguments[1]).multiArgs
                                         : false;
    var result = tryCatch(fn)(nodebackForPromise(ret, multiArgs));
    if (result === errorObj) {
        ret._rejectCallback(result.e, true);
    }
    if (!ret._isFateSealed()) ret._setAsyncGuaranteed();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.fulfilled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>fulfilled (obj)](#apidoc.element.gulp-buster._Promise.fulfilled)
- description and source-code
```javascript
fulfilled = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._setFulfilled();
        ret._rejectionHandler0 = obj;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.getNewLibraryCopy"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>getNewLibraryCopy ()](#apidoc.element.gulp-buster._Promise.getNewLibraryCopy)
- description and source-code
```javascript
getNewLibraryCopy = function () {
var makeSelfResolutionError = function () {
    return new TypeError("circular promise resolution chain\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
};
var reflectHandler = function() {
    return new Promise.PromiseInspection(this._target());
};
var apiRejection = function(msg) {
    return Promise.reject(new TypeError(msg));
};
function Proxyable() {}
var UNDEFINED_BINDING = {};
var util = require("./util");

var getDomain;
if (util.isNode) {
    getDomain = function() {
        var ret = process.domain;
        if (ret === undefined) ret = null;
        return ret;
    };
} else {
    getDomain = function() {
        return null;
    };
}
util.notEnumerableProp(Promise, "_getDomain", getDomain);

var es5 = require("./es5");
var Async = require("./async");
var async = new Async();
es5.defineProperty(Promise, "_async", {value: async});
var errors = require("./errors");
var TypeError = Promise.TypeError = errors.TypeError;
Promise.RangeError = errors.RangeError;
var CancellationError = Promise.CancellationError = errors.CancellationError;
Promise.TimeoutError = errors.TimeoutError;
Promise.OperationalError = errors.OperationalError;
Promise.RejectionError = errors.OperationalError;
Promise.AggregateError = errors.AggregateError;
var INTERNAL = function(){};
var APPLY = {};
var NEXT_FILTER = {};
var tryConvertToPromise = require("./thenables")(Promise, INTERNAL);
var PromiseArray =
    require("./promise_array")(Promise, INTERNAL,
                               tryConvertToPromise, apiRejection, Proxyable);
var Context = require("./context")(Promise);
<span class="apidocCodeCommentSpan"> /*jshint unused:false*/
</span>var createContext = Context.create;
var debug = require("./debuggability")(Promise, Context);
var CapturedTrace = debug.CapturedTrace;
var PassThroughHandlerContext =
    require("./finally")(Promise, tryConvertToPromise, NEXT_FILTER);
var catchFilter = require("./catch_filter")(NEXT_FILTER);
var nodebackForPromise = require("./nodeback");
var errorObj = util.errorObj;
var tryCatch = util.tryCatch;
function check(self, executor) {
    if (self == null || self.constructor !== Promise) {
        throw new TypeError("the promise constructor cannot be invoked directly\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    if (typeof executor !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(executor));
    }

}

function Promise(executor) {
    if (executor !== INTERNAL) {
        check(this, executor);
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._resolveFromExecutor(executor);
    this._promiseCreated();
    this._fireEvent("promiseCreated", this);
}

Promise.prototype.toString = function () {
    return "[object Promise]";
};

Promise.prototype.caught = Promise.prototype["catch"] = function (fn) {
    var len = arguments.length;
    if (len > 1) {
        var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (util.isObject(item)) {
                catchInstances[j++] = item;
            } else {
                return apiRejection("Catch statement predicate: " +
                    "expecting an object but got " + util.classString(item));
            }
        }
        catchInstances.length = j;
        fn = arguments[i];
        return this.then(undefined, catchFilter(catchInstances, fn, this));
    }
    return this.then(undefined, fn);
};

Promise.prototype.reflect = function () {
    return this._then(reflectHandler,
        reflectHandler, undefined, this, undefined);
};

Promise.prototype.then = function (didFulfill, didReject) {
    if (debug.warnings() && arguments.length > 0 &&
        typeof didFulfill !== "function" &&
        typeof didReject !== "function") {
        var msg = ".then() only accepts functions but was passed: " +
                util.classString(didFulfill);
        if (arguments.length > 1) {
            msg += ", ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.hasLongStackTraces"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>hasLongStackTraces ()](#apidoc.element.gulp-buster._Promise.hasLongStackTraces)
- description and source-code
```javascript
hasLongStackTraces = function () {
    return config.longStackTraces && longStackTracesIsSupported();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.is"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>is (val)](#apidoc.element.gulp-buster._Promise.is)
- description and source-code
```javascript
is = function (val) {
    return val instanceof Promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.join"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>join ()](#apidoc.element.gulp-buster._Promise.join)
- description and source-code
```javascript
join = function () {
    var last = arguments.length - 1;
    var fn;
    if (last > 0 && typeof arguments[last] === "function") {
        fn = arguments[last];
        if (!false) {
            if (last <= 8 && canEvaluate) {
                var ret = new Promise(INTERNAL);
                ret._captureStackTrace();
                var HolderClass = holderClasses[last - 1];
                var holder = new HolderClass(fn);
                var callbacks = thenCallbacks;

                for (var i = 0; i < last; ++i) {
                    var maybePromise = tryConvertToPromise(arguments[i], ret);
                    if (maybePromise instanceof Promise) {
                        maybePromise = maybePromise._target();
                        var bitField = maybePromise._bitField;
                        ;
                        if (((bitField & 50397184) === 0)) {
                            maybePromise._then(callbacks[i], reject,
                                               undefined, ret, holder);
                            promiseSetters[i](maybePromise, holder);
                            holder.asyncNeeded = false;
                        } else if (((bitField & 33554432) !== 0)) {
                            callbacks[i].call(ret,
                                              maybePromise._value(), holder);
                        } else if (((bitField & 16777216) !== 0)) {
                            ret._reject(maybePromise._reason());
                        } else {
                            ret._cancel();
                        }
                    } else {
                        callbacks[i].call(ret, maybePromise, holder);
                    }
                }

                if (!ret._isFateSealed()) {
                    if (holder.asyncNeeded) {
                        var domain = getDomain();
                        if (domain !== null) {
                            holder.fn = util.domainBind(domain, holder.fn);
                        }
                    }
                    ret._setAsyncGuaranteed();
                    ret._setOnCancel(holder);
                }
                return ret;
            }
        }
    }
    var $_len = arguments.length;var args = new Array($_len); for(var $_i = 0; $_i < $_len; ++$_i) {args[$_i] = arguments[$_i];};
    if (fn) args.pop();
    var ret = new PromiseArray(args).promise();
    return fn !== undefined ? ret.spread(fn) : ret;
}
```
- example usage
```shell
...
		? options.length > 0
			? hash.slice(0, options.length)
			: hash.slice(options.length)
		: hash;
}

function relativePath(projectPath, relativePath, filePath) {
	return path.relative(path.join(projectPath, relativePath), filePath).replace(/\\/g, '/');
}

function getType(value) {
	return {}.toString.call(value).slice(8, -1);
}

function assignOptions(options) {
...
```

#### <a name="apidoc.element.gulp-buster._Promise.longStackTraces"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>longStackTraces ()](#apidoc.element.gulp-buster._Promise.longStackTraces)
- description and source-code
```javascript
longStackTraces = function () {
    if (async.haveItemsQueued() && !config.longStackTraces) {
        throw new Error("cannot enable long stack traces after promises have been created\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    if (!config.longStackTraces && longStackTracesIsSupported()) {
        var Promise_captureStackTrace = Promise.prototype._captureStackTrace;
        var Promise_attachExtraTrace = Promise.prototype._attachExtraTrace;
        config.longStackTraces = true;
        disableLongStackTraces = function() {
            if (async.haveItemsQueued() && !config.longStackTraces) {
                throw new Error("cannot enable long stack traces after promises have been created\u000a\u000a    See http://goo.
gl/MqrFmX\u000a");
            }
            Promise.prototype._captureStackTrace = Promise_captureStackTrace;
            Promise.prototype._attachExtraTrace = Promise_attachExtraTrace;
            Context.deactivateLongStackTraces();
            async.enableTrampoline();
            config.longStackTraces = false;
        };
        Promise.prototype._captureStackTrace = longStackTracesCaptureStackTrace;
        Promise.prototype._attachExtraTrace = longStackTracesAttachExtraTrace;
        Context.activateLongStackTraces();
        async.disableTrampolineIfNecessary();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.map"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>map (promises, fn, options, _filter)](#apidoc.element.gulp-buster._Promise.map)
- description and source-code
```javascript
map = function (promises, fn, options, _filter) {
    return map(promises, fn, options, _filter);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.mapSeries"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>mapSeries (promises, fn)](#apidoc.element.gulp-buster._Promise.mapSeries)
- description and source-code
```javascript
function PromiseMapSeries(promises, fn) {
    return PromiseReduce(promises, fn, INTERNAL, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.method"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>method (fn)](#apidoc.element.gulp-buster._Promise.method)
- description and source-code
```javascript
method = function (fn) {
    if (typeof fn !== "function") {
        throw new Promise.TypeError("expecting a function but got " + util.classString(fn));
    }
    return function () {
        var ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._pushContext();
        var value = tryCatch(fn).apply(this, arguments);
        var promiseCreated = ret._popContext();
        debug.checkForgottenReturns(
            value, promiseCreated, "Promise.method", ret);
        ret._resolveFromSyncValue(value);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.noConflict"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>noConflict ()](#apidoc.element.gulp-buster._Promise.noConflict)
- description and source-code
```javascript
function noConflict() {
    try { if (Promise === bluebird) Promise = old; }
    catch (e) {}
    return bluebird;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.onPossiblyUnhandledRejection"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>onPossiblyUnhandledRejection (fn)](#apidoc.element.gulp-buster._Promise.onPossiblyUnhandledRejection)
- description and source-code
```javascript
onPossiblyUnhandledRejection = function (fn) {
    var domain = getDomain();
    possiblyUnhandledRejection =
        typeof fn === "function" ? (domain === null ?
                                            fn : util.domainBind(domain, fn))
                                 : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.onUnhandledRejectionHandled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>onUnhandledRejectionHandled (fn)](#apidoc.element.gulp-buster._Promise.onUnhandledRejectionHandled)
- description and source-code
```javascript
onUnhandledRejectionHandled = function (fn) {
    var domain = getDomain();
    unhandledRejectionHandled =
        typeof fn === "function" ? (domain === null ?
                                            fn : util.domainBind(domain, fn))
                                 : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.pending"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>pending ()](#apidoc.element.gulp-buster._Promise.pending)
- description and source-code
```javascript
pending = function () {
    debug.deprecated("Promise.defer", "new Promise");
    var promise = new Promise(INTERNAL);
    return {
        promise: promise,
        resolve: deferResolve,
        reject: deferReject
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.promisify"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>promisify (fn, options)](#apidoc.element.gulp-buster._Promise.promisify)
- description and source-code
```javascript
promisify = function (fn, options) {
    if (typeof fn !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(fn));
    }
    if (isPromisified(fn)) {
        return fn;
    }
    options = Object(options);
    var receiver = options.context === undefined ? THIS : options.context;
    var multiArgs = !!options.multiArgs;
    var ret = promisify(fn, receiver, multiArgs);
    util.copyDescriptors(fn, ret, propsFilter);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.promisifyAll"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>promisifyAll (target, options)](#apidoc.element.gulp-buster._Promise.promisifyAll)
- description and source-code
```javascript
promisifyAll = function (target, options) {
    if (typeof target !== "function" && typeof target !== "object") {
        throw new TypeError("the target of promisifyAll must be an object or a function\u000a\u000a    See http://goo.gl/MqrFmX\
u000a");
    }
    options = Object(options);
    var multiArgs = !!options.multiArgs;
    var suffix = options.suffix;
    if (typeof suffix !== "string") suffix = defaultSuffix;
    var filter = options.filter;
    if (typeof filter !== "function") filter = defaultFilter;
    var promisifier = options.promisifier;
    if (typeof promisifier !== "function") promisifier = makeNodePromisified;

    if (!util.isIdentifier(suffix)) {
        throw new RangeError("suffix must be a valid identifier\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }

    var keys = util.inheritedDataKeys(target);
    for (var i = 0; i < keys.length; ++i) {
        var value = target[keys[i]];
        if (keys[i] !== "constructor" &&
            util.isClass(value)) {
            promisifyAll(value.prototype, suffix, filter, promisifier,
                multiArgs);
            promisifyAll(value, suffix, filter, promisifier, multiArgs);
        }
    }

    return promisifyAll(target, suffix, filter, promisifier, multiArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.props"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>props (promises)](#apidoc.element.gulp-buster._Promise.props)
- description and source-code
```javascript
props = function (promises) {
    return props(promises);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.race"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>race (promises)](#apidoc.element.gulp-buster._Promise.race)
- description and source-code
```javascript
race = function (promises) {
    return race(promises, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.reduce"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>reduce (promises, fn, initialValue, _each)](#apidoc.element.gulp-buster._Promise.reduce)
- description and source-code
```javascript
reduce = function (promises, fn, initialValue, _each) {
    return reduce(promises, fn, initialValue, _each);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.reject"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>reject (reason)](#apidoc.element.gulp-buster._Promise.reject)
- description and source-code
```javascript
reject = function (reason) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._rejectCallback(reason, true);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.rejected"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>rejected (reason)](#apidoc.element.gulp-buster._Promise.rejected)
- description and source-code
```javascript
rejected = function (reason) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._rejectCallback(reason, true);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.resolve"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>resolve (obj)](#apidoc.element.gulp-buster._Promise.resolve)
- description and source-code
```javascript
resolve = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._setFulfilled();
        ret._rejectionHandler0 = obj;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.setScheduler"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>setScheduler (fn)](#apidoc.element.gulp-buster._Promise.setScheduler)
- description and source-code
```javascript
setScheduler = function (fn) {
    if (typeof fn !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(fn));
    }
    return async.setScheduler(fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.settle"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>settle (promises)](#apidoc.element.gulp-buster._Promise.settle)
- description and source-code
```javascript
settle = function (promises) {
    debug.deprecated(".settle()", ".reflect()");
    return new SettledPromiseArray(promises).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.some"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>some (promises, howMany)](#apidoc.element.gulp-buster._Promise.some)
- description and source-code
```javascript
some = function (promises, howMany) {
    return some(promises, howMany);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.spawn"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>spawn (generatorFunction)](#apidoc.element.gulp-buster._Promise.spawn)
- description and source-code
```javascript
spawn = function (generatorFunction) {
    debug.deprecated("Promise.spawn()", "Promise.coroutine()");
    if (typeof generatorFunction !== "function") {
        return apiRejection("generatorFunction must be a function\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    var spawn = new PromiseSpawn(generatorFunction, this);
    var ret = spawn.promise();
    spawn._run(Promise.spawn);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.try"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>try (fn)](#apidoc.element.gulp-buster._Promise.try)
- description and source-code
```javascript
try = function (fn) {
    if (typeof fn !== "function") {
        return apiRejection("expecting a function but got " + util.classString(fn));
    }
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._pushContext();
    var value;
    if (arguments.length > 1) {
        debug.deprecated("calling Promise.try with more than 1 argument");
        var arg = arguments[1];
        var ctx = arguments[2];
        value = util.isArray(arg) ? tryCatch(fn).apply(ctx, arg)
                                  : tryCatch(fn).call(ctx, arg);
    } else {
        value = tryCatch(fn)();
    }
    var promiseCreated = ret._popContext();
    debug.checkForgottenReturns(
        value, promiseCreated, "Promise.try", ret);
    ret._resolveFromSyncValue(value);
    return ret;
}
```
- example usage
```shell
...

	function hashFile(file) {
		if (file.isNull()) return; // ignore
		if (file.isStream()) return this.emit('error', error('Streaming not supported'));

		// start hashing files as soon as they are received for maximum concurrency
		hashingPromises.push(
			Promise.try(hash.bind(undefined, file, options)).then(function(hashed) {
				if (typeof hashed !== 'string') throw error('Return/fulfill value of 'options.algo' must be a string');
				hashes[relativePath(file.cwd, options.relativePath, file.path)] = sliceHash(hashed, options);
			})
		);
	}

	function endStream() {
...
```

#### <a name="apidoc.element.gulp-buster._Promise.using"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>using ()](#apidoc.element.gulp-buster._Promise.using)
- description and source-code
```javascript
using = function () {
    var len = arguments.length;
    if (len < 2) return apiRejection(
                    "you must pass at least 2 arguments to Promise.using");
    var fn = arguments[len - 1];
    if (typeof fn !== "function") {
        return apiRejection("expecting a function but got " + util.classString(fn));
    }
    var input;
    var spreadArgs = true;
    if (len === 2 && Array.isArray(arguments[0])) {
        input = arguments[0];
        len = input.length;
        spreadArgs = false;
    } else {
        input = arguments;
        len--;
    }
    var resources = new ResourceList(len);
    for (var i = 0; i < len; ++i) {
        var resource = input[i];
        if (Disposer.isDisposer(resource)) {
            var disposer = resource;
            resource = resource.promise();
            resource._setDisposable(disposer);
        } else {
            var maybePromise = tryConvertToPromise(resource);
            if (maybePromise instanceof Promise) {
                resource =
                    maybePromise._then(maybeUnwrapDisposer, null, null, {
                        resources: resources,
                        index: i
                }, undefined);
            }
        }
        resources[i] = resource;
    }

    var reflectedResources = new Array(resources.length);
    for (var i = 0; i < reflectedResources.length; ++i) {
        reflectedResources[i] = Promise.resolve(resources[i]).reflect();
    }

    var resultPromise = Promise.all(reflectedResources)
        .then(function(inspections) {
            for (var i = 0; i < inspections.length; ++i) {
                var inspection = inspections[i];
                if (inspection.isRejected()) {
                    errorObj.e = inspection.error();
                    return errorObj;
                } else if (!inspection.isFulfilled()) {
                    resultPromise.cancel();
                    return;
                }
                inspections[i] = inspection.value();
            }
            promise._pushContext();

            fn = tryCatch(fn);
            var ret = spreadArgs
                ? fn.apply(undefined, inspections) : fn(inspections);
            var promiseCreated = promise._popContext();
            debug.checkForgottenReturns(
                ret, promiseCreated, "Promise.using", promise);
            return ret;
        });

    var promise = resultPromise.lastly(function() {
        var inspection = new Promise.PromiseInspection(resultPromise);
        return dispose(resources, inspection);
    });
    resources.promise = promise;
    promise._setOnCancel(resources);
    return promise;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.AggregateError"></a>[module gulp-buster._Promise.AggregateError](#apidoc.module.gulp-buster._Promise.AggregateError)

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.AggregateError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>AggregateError (message)](#apidoc.element.gulp-buster._Promise.AggregateError.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.AggregateError.prototype"></a>[module gulp-buster._Promise.AggregateError.prototype](#apidoc.module.gulp-buster._Promise.AggregateError.prototype)

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.every"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>every ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.every)
- description and source-code
```javascript
function every() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.filter"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>filter ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.filter)
- description and source-code
```javascript
function filter() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.forEach"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>forEach ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.forEach)
- description and source-code
```javascript
function forEach() { [native code] }
```
- example usage
```shell
...
	return {}.toString.call(value).slice(8, -1);
}

function assignOptions(options) {
	if (typeof options === 'string') options = { fileName: options };
	options = options || {};

	Object.keys(options).forEach(function(option) {
		if (!OPTION_TYPES.hasOwnProperty(option)) throw error('Unsupported option: ' + option);
		if (options[option] !== undefined && OPTION_TYPES[option].indexOf(getType(options[option])) === -1) throw error(''options.' +
option + '' must be of type ' + OPTION_TYPES[option].join(' or '));
	});

	return defaults({}, options, DEFAULT_OPTIONS);
}
...
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>indexOf ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.indexOf)
- description and source-code
```javascript
function indexOf() { [native code] }
```
- example usage
```shell
...

function assignOptions(options) {
	if (typeof options === 'string') options = { fileName: options };
	options = options || {};

	Object.keys(options).forEach(function(option) {
		if (!OPTION_TYPES.hasOwnProperty(option)) throw error('Unsupported option: ' + option);
		if (options[option] !== undefined && OPTION_TYPES[option].indexOf(getType(options[option])) === -1) throw error(''options.' +
option + '' must be of type ' + OPTION_TYPES[option].join(' or '));
	});

	return defaults({}, options, DEFAULT_OPTIONS);
}

module.exports = exports = function(options) {
	options = assignOptions(options);
...
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.join"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>join ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.join)
- description and source-code
```javascript
function join() { [native code] }
```
- example usage
```shell
...
		? options.length > 0
			? hash.slice(0, options.length)
			: hash.slice(options.length)
		: hash;
}

function relativePath(projectPath, relativePath, filePath) {
	return path.relative(path.join(projectPath, relativePath), filePath).replace(/\\/g, '/');
}

function getType(value) {
	return {}.toString.call(value).slice(8, -1);
}

function assignOptions(options) {
...
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>lastIndexOf ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.map"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>map ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.map)
- description and source-code
```javascript
function map() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.pop"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>pop ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.pop)
- description and source-code
```javascript
function pop() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.push"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>push ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.push)
- description and source-code
```javascript
function push() { [native code] }
```
- example usage
```shell
...
		hashingPromises = [];

	function hashFile(file) {
		if (file.isNull()) return; // ignore
		if (file.isStream()) return this.emit('error', error('Streaming not supported'));

		// start hashing files as soon as they are received for maximum concurrency
		hashingPromises.push(
			Promise.try(hash.bind(undefined, file, options)).then(function(hashed) {
				if (typeof hashed !== 'string') throw error('Return/fulfill value of 'options.algo' must be a string');
				hashes[relativePath(file.cwd, options.relativePath, file.path)] = sliceHash(hashed, options);
			})
		);
	}
...
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.reduce"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>reduce ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.reduce)
- description and source-code
```javascript
function reduce() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>reduceRight ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.reduceRight)
- description and source-code
```javascript
function reduceRight() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.reverse"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>reverse ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.reverse)
- description and source-code
```javascript
function reverse() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.shift"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>shift ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.shift)
- description and source-code
```javascript
function shift() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.slice"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>slice ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.slice)
- description and source-code
```javascript
function slice() { [native code] }
```
- example usage
```shell
...
		: crypto.createHash(options.algo).update(file.contents).digest('hex');
}

function sliceHash(hash, options) {
	// positive length = leading characters; negative = trailing
	return options.length
		? options.length > 0
			? hash.slice(0, options.length)
			: hash.slice(options.length)
		: hash;
}

function relativePath(projectPath, relativePath, filePath) {
	return path.relative(path.join(projectPath, relativePath), filePath).replace(/\\/g, '/');
}
...
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.some"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>some ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.some)
- description and source-code
```javascript
function some() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.sort"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>sort ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.sort)
- description and source-code
```javascript
function sort() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.toString"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>toString ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.toString)
- description and source-code
```javascript
toString = function () {
    var indent = Array(level * 4 + 1).join(" ");
    var ret = "\n" + indent + "AggregateError of:" + "\n";
    level++;
    indent = Array(level * 4 + 1).join(" ");
    for (var i = 0; i < this.length; ++i) {
        var str = this[i] === this ? "[Circular AggregateError]" : this[i] + "";
        var lines = str.split("\n");
        for (var j = 0; j < lines.length; ++j) {
            lines[j] = indent + lines[j];
        }
        str = lines.join("\n");
        ret += str + "\n";
    }
    level--;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.AggregateError.prototype.unshift"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.AggregateError.prototype.</span>unshift ()](#apidoc.element.gulp-buster._Promise.AggregateError.prototype.unshift)
- description and source-code
```javascript
function unshift() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.CancellationError"></a>[module gulp-buster._Promise.CancellationError](#apidoc.module.gulp-buster._Promise.CancellationError)

#### <a name="apidoc.element.gulp-buster._Promise.CancellationError.CancellationError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>CancellationError (message)](#apidoc.element.gulp-buster._Promise.CancellationError.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.CancellationError.prototype"></a>[module gulp-buster._Promise.CancellationError.prototype](#apidoc.module.gulp-buster._Promise.CancellationError.prototype)

#### <a name="apidoc.element.gulp-buster._Promise.CancellationError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.CancellationError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.CancellationError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.OperationalError"></a>[module gulp-buster._Promise.OperationalError](#apidoc.module.gulp-buster._Promise.OperationalError)

#### <a name="apidoc.element.gulp-buster._Promise.OperationalError.OperationalError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>OperationalError (message)](#apidoc.element.gulp-buster._Promise.OperationalError.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.OperationalError.prototype"></a>[module gulp-buster._Promise.OperationalError.prototype](#apidoc.module.gulp-buster._Promise.OperationalError.prototype)

#### <a name="apidoc.element.gulp-buster._Promise.OperationalError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.OperationalError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.OperationalError.prototype.constructor)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.PromiseInspection"></a>[module gulp-buster._Promise.PromiseInspection](#apidoc.module.gulp-buster._Promise.PromiseInspection)

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.PromiseInspection"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>PromiseInspection (promise)](#apidoc.element.gulp-buster._Promise.PromiseInspection.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValueField = promise._isFateSealed()
            ? promise._settledValue() : undefined;
    }
    else {
        this._bitField = 0;
        this._settledValueField = undefined;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.PromiseInspection.prototype"></a>[module gulp-buster._Promise.PromiseInspection.prototype](#apidoc.module.gulp-buster._Promise.PromiseInspection.prototype)

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype._settledValue"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>_settledValue ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype._settledValue)
- description and source-code
```javascript
_settledValue = function () {
    return this._settledValueField;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.error"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>error ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.error)
- description and source-code
```javascript
error = function () {
    if (!this.isRejected()) {
        throw new TypeError("cannot get rejection reason of a non-rejected promise\u000a\u000a    See http://goo.gl/MqrFmX\u000a
");
    }
    return this._settledValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isCancelled ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isCancelled)
- description and source-code
```javascript
isCancelled = function () {
    return (this._bitField & 8454144) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isFulfilled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isFulfilled ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isFulfilled)
- description and source-code
```javascript
isFulfilled = function () {
    return (this._bitField & 33554432) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isPending"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isPending ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isPending)
- description and source-code
```javascript
isPending = function () {
    return (this._bitField & 50397184) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isRejected"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isRejected ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isRejected)
- description and source-code
```javascript
isRejected = function () {
    return (this._bitField & 16777216) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isResolved"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>isResolved ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.isResolved)
- description and source-code
```javascript
isResolved = function () {
    return (this._bitField & 50331648) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.reason"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>reason ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.reason)
- description and source-code
```javascript
reason = function () {
    if (!this.isRejected()) {
        throw new TypeError("cannot get rejection reason of a non-rejected promise\u000a\u000a    See http://goo.gl/MqrFmX\u000a
");
    }
    return this._settledValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.value"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.PromiseInspection.prototype.</span>value ()](#apidoc.element.gulp-buster._Promise.PromiseInspection.prototype.value)
- description and source-code
```javascript
value = function () {
    if (!this.isFulfilled()) {
        throw new TypeError("cannot get fulfillment value of a non-fulfilled promise\u000a\u000a    See http://goo.gl/MqrFmX\u000a
");
    }
    return this._settledValue();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.TimeoutError"></a>[module gulp-buster._Promise.TimeoutError](#apidoc.module.gulp-buster._Promise.TimeoutError)

#### <a name="apidoc.element.gulp-buster._Promise.TimeoutError.TimeoutError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>TimeoutError (message)](#apidoc.element.gulp-buster._Promise.TimeoutError.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.TimeoutError.prototype"></a>[module gulp-buster._Promise.TimeoutError.prototype](#apidoc.module.gulp-buster._Promise.TimeoutError.prototype)

#### <a name="apidoc.element.gulp-buster._Promise.TimeoutError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.TimeoutError.prototype.</span>constructor (message)](#apidoc.element.gulp-buster._Promise.TimeoutError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise._SomePromiseArray"></a>[module gulp-buster._Promise._SomePromiseArray](#apidoc.module.gulp-buster._Promise._SomePromiseArray)

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>_SomePromiseArray (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise._SomePromiseArray.prototype"></a>[module gulp-buster._Promise._SomePromiseArray.prototype](#apidoc.module.gulp-buster._Promise._SomePromiseArray.prototype)

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._addFulfilled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_addFulfilled (value)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._addFulfilled)
- description and source-code
```javascript
_addFulfilled = function (value) {
    this._values[this._totalResolved++] = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._addRejected"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_addRejected (reason)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._addRejected)
- description and source-code
```javascript
_addRejected = function (reason) {
    this._values.push(reason);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._canPossiblyFulfill"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_canPossiblyFulfill ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._canPossiblyFulfill)
- description and source-code
```javascript
_canPossiblyFulfill = function () {
    return this.length() - this._rejected();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._checkOutcome"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_checkOutcome ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._checkOutcome)
- description and source-code
```javascript
_checkOutcome = function () {
    if (this.howMany() > this._canPossiblyFulfill()) {
        var e = new AggregateError();
        for (var i = this.length(); i < this._values.length; ++i) {
            if (this._values[i] !== CANCELLATION) {
                e.push(this._values[i]);
            }
        }
        if (e.length > 0) {
            this._reject(e);
        } else {
            this._cancel();
        }
        return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._fulfilled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_fulfilled ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._fulfilled)
- description and source-code
```javascript
_fulfilled = function () {
    return this._totalResolved;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._getRangeError"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_getRangeError (count)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._getRangeError)
- description and source-code
```javascript
_getRangeError = function (count) {
    var message = "Input array must contain at least " +
            this._howMany + " items but contains only " + count + " items";
    return new RangeError(message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._init"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_init ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._init)
- description and source-code
```javascript
_init = function () {
    if (!this._initialized) {
        return;
    }
    if (this._howMany === 0) {
        this._resolve([]);
        return;
    }
    this._init$(undefined, -5);
    var isArrayResolved = isArray(this._values);
    if (!this._isResolved() &&
        isArrayResolved &&
        this._howMany > this._canPossiblyFulfill()) {
        this._reject(this._getRangeError(this.length()));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_promiseCancelled ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseCancelled)
- description and source-code
```javascript
_promiseCancelled = function () {
    if (this._values instanceof Promise || this._values == null) {
        return this._cancel();
    }
    this._addRejected(CANCELLATION);
    return this._checkOutcome();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseFulfilled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_promiseFulfilled (value)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseFulfilled)
- description and source-code
```javascript
_promiseFulfilled = function (value) {
    this._addFulfilled(value);
    if (this._fulfilled() === this.howMany()) {
        this._values.length = this.howMany();
        if (this.howMany() === 1 && this._unwrap) {
            this._resolve(this._values[0]);
        } else {
            this._resolve(this._values);
        }
        return true;
    }
    return false;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseRejected"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_promiseRejected (reason)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._promiseRejected)
- description and source-code
```javascript
_promiseRejected = function (reason) {
    this._addRejected(reason);
    return this._checkOutcome();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._rejected"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_rejected ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._rejected)
- description and source-code
```javascript
_rejected = function () {
    return this._values.length - this.length();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._resolveEmptyArray"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>_resolveEmptyArray ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype._resolveEmptyArray)
- description and source-code
```javascript
_resolveEmptyArray = function () {
    this._reject(this._getRangeError(0));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.constructor"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>constructor (values)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.constructor)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.howMany"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>howMany ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.howMany)
- description and source-code
```javascript
howMany = function () {
    return this._howMany;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.init"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>init ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.init)
- description and source-code
```javascript
init = function () {
    this._initialized = true;
    this._init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.setHowMany"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>setHowMany (count)](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.setHowMany)
- description and source-code
```javascript
setHowMany = function (count) {
    this._howMany = count;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.setUnwrap"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise._SomePromiseArray.prototype.</span>setUnwrap ()](#apidoc.element.gulp-buster._Promise._SomePromiseArray.prototype.setUnwrap)
- description and source-code
```javascript
setUnwrap = function () {
    this._unwrap = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.coroutine"></a>[module gulp-buster._Promise.coroutine](#apidoc.module.gulp-buster._Promise.coroutine)

#### <a name="apidoc.element.gulp-buster._Promise.coroutine.coroutine"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.</span>coroutine (generatorFunction, options)](#apidoc.element.gulp-buster._Promise.coroutine.coroutine)
- description and source-code
```javascript
coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        var ret = spawn.promise();
        spawn._generator = generator;
        spawn._promiseFulfilled(undefined);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.coroutine.addYieldHandler"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.coroutine.</span>addYieldHandler (fn)](#apidoc.element.gulp-buster._Promise.coroutine.addYieldHandler)
- description and source-code
```javascript
addYieldHandler = function (fn) {
    if (typeof fn !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(fn));
    }
    yieldHandlers.push(fn);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-buster._Promise.prototype"></a>[module gulp-buster._Promise.prototype](#apidoc.module.gulp-buster._Promise.prototype)

#### <a name="apidoc.element.gulp-buster._Promise.prototype.__isCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>__isCancelled ()](#apidoc.element.gulp-buster._Promise.prototype.__isCancelled)
- description and source-code
```javascript
__isCancelled = function () {
    return (this._bitField & 65536) === 65536;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._addCallbacks"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_addCallbacks ( fulfill, reject, promise, receiver, domain )](#apidoc.element.gulp-buster._Promise.prototype._addCallbacks)
- description and source-code
```javascript
_addCallbacks = function ( fulfill, reject, promise, receiver, domain ) {
    var index = this._length();

    if (index >= 65535 - 4) {
        index = 0;
        this._setLength(0);
    }

    if (index === 0) {
        this._promise0 = promise;
        this._receiver0 = receiver;
        if (typeof fulfill === "function") {
            this._fulfillmentHandler0 =
                domain === null ? fulfill : util.domainBind(domain, fulfill);
        }
        if (typeof reject === "function") {
            this._rejectionHandler0 =
                domain === null ? reject : util.domainBind(domain, reject);
        }
    } else {
        var base = index * 4 - 4;
        this[base + 2] = promise;
        this[base + 3] = receiver;
        if (typeof fulfill === "function") {
            this[base + 0] =
                domain === null ? fulfill : util.domainBind(domain, fulfill);
        }
        if (typeof reject === "function") {
            this[base + 1] =
                domain === null ? reject : util.domainBind(domain, reject);
        }
    }
    this._setLength(index + 1);
    return index;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._attachCancellationCallback"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_attachCancellationCallback (onCancel)](#apidoc.element.gulp-buster._Promise.prototype._attachCancellationCallback)
- description and source-code
```javascript
_attachCancellationCallback = function (onCancel) {
    ;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._attachExtraTrace"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_attachExtraTrace ()](#apidoc.element.gulp-buster._Promise.prototype._attachExtraTrace)
- description and source-code
```javascript
_attachExtraTrace = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._boundValue"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_boundValue ()](#apidoc.element.gulp-buster._Promise.prototype._boundValue)
- description and source-code
```javascript
_boundValue = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._branchHasCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_branchHasCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._branchHasCancelled)
- description and source-code
```javascript
_branchHasCancelled = function () {
    this._branchesRemainingToCancel--;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._cancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancel ()](#apidoc.element.gulp-buster._Promise.prototype._cancel)
- description and source-code
```javascript
_cancel = function () {
    if (!this._isCancellable()) return;
    this._setCancelled();
    async.invoke(this._cancelPromises, this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._cancelBranched"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancelBranched ()](#apidoc.element.gulp-buster._Promise.prototype._cancelBranched)
- description and source-code
```javascript
_cancelBranched = function () {
    if (this._enoughBranchesHaveCancelled()) {
        this._cancel();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._cancelBy"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancelBy (canceller)](#apidoc.element.gulp-buster._Promise.prototype._cancelBy)
- description and source-code
```javascript
_cancelBy = function (canceller) {
    if (canceller === this) {
        this._branchesRemainingToCancel = 0;
        this._invokeOnCancel();
        return true;
    } else {
        this._branchHasCancelled();
        if (this._enoughBranchesHaveCancelled()) {
            this._invokeOnCancel();
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._cancelPromises"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_cancelPromises ()](#apidoc.element.gulp-buster._Promise.prototype._cancelPromises)
- description and source-code
```javascript
_cancelPromises = function () {
    if (this._length() > 0) this._settlePromises();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._captureStackTrace"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_captureStackTrace ()](#apidoc.element.gulp-buster._Promise.prototype._captureStackTrace)
- description and source-code
```javascript
_captureStackTrace = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._clearCallbackDataAtIndex"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_clearCallbackDataAtIndex (index)](#apidoc.element.gulp-buster._Promise.prototype._clearCallbackDataAtIndex)
- description and source-code
```javascript
_clearCallbackDataAtIndex = function (index) {
    var base = index * 4 - 4;
    this[base + 2] =
    this[base + 3] =
    this[base + 0] =
    this[base + 1] = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._clearCancellationData"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_clearCancellationData ()](#apidoc.element.gulp-buster._Promise.prototype._clearCancellationData)
- description and source-code
```javascript
_clearCancellationData = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._doInvokeOnCancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_doInvokeOnCancel (onCancelCallback, internalOnly)](#apidoc.element.gulp-buster._Promise.prototype._doInvokeOnCancel)
- description and source-code
```javascript
_doInvokeOnCancel = function (onCancelCallback, internalOnly) {
    if (util.isArray(onCancelCallback)) {
        for (var i = 0; i < onCancelCallback.length; ++i) {
            this._doInvokeOnCancel(onCancelCallback[i], internalOnly);
        }
    } else if (onCancelCallback !== undefined) {
        if (typeof onCancelCallback === "function") {
            if (!internalOnly) {
                var e = tryCatch(onCancelCallback).call(this._boundValue());
                if (e === errorObj) {
                    this._attachExtraTrace(e.e);
                    async.throwLater(e.e);
                }
            }
        } else {
            onCancelCallback._resultCancelled(this);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._enoughBranchesHaveCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_enoughBranchesHaveCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._enoughBranchesHaveCancelled)
- description and source-code
```javascript
_enoughBranchesHaveCancelled = function () {
    return this._branchesRemainingToCancel === undefined ||
           this._branchesRemainingToCancel <= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._ensurePossibleRejectionHandled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_ensurePossibleRejectionHandled ()](#apidoc.element.gulp-buster._Promise.prototype._ensurePossibleRejectionHandled)
- description and source-code
```javascript
_ensurePossibleRejectionHandled = function () {
    if ((this._bitField & 524288) !== 0) return;
    this._setRejectionIsUnhandled();
    async.invokeLater(this._notifyUnhandledRejection, this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._execute"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_execute (executor, resolve, reject)](#apidoc.element.gulp-buster._Promise.prototype._execute)
- description and source-code
```javascript
_execute = function (executor, resolve, reject) {
    try {
        executor(resolve, reject);
    } catch (e) {
        return e;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._fireEvent"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fireEvent ()](#apidoc.element.gulp-buster._Promise.prototype._fireEvent)
- description and source-code
```javascript
function defaultFireEvent() { return false; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._followee"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_followee ()](#apidoc.element.gulp-buster._Promise.prototype._followee)
- description and source-code
```javascript
_followee = function () {
    return this._rejectionHandler0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._fulfill"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fulfill (value)](#apidoc.element.gulp-buster._Promise.prototype._fulfill)
- description and source-code
```javascript
_fulfill = function (value) {
    var bitField = this._bitField;
    if (((bitField & 117506048) >>> 16)) return;
    if (value === this) {
        var err = makeSelfResolutionError();
        this._attachExtraTrace(err);
        return this._reject(err);
    }
    this._setFulfilled();
    this._rejectionHandler0 = value;

    if ((bitField & 65535) > 0) {
        if (((bitField & 134217728) !== 0)) {
            this._settlePromises();
        } else {
            async.settlePromises(this);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._fulfillPromises"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fulfillPromises (len, value)](#apidoc.element.gulp-buster._Promise.prototype._fulfillPromises)
- description and source-code
```javascript
_fulfillPromises = function (len, value) {
    for (var i = 1; i < len; i++) {
        var handler = this._fulfillmentHandlerAt(i);
        var promise = this._promiseAt(i);
        var receiver = this._receiverAt(i);
        this._clearCallbackDataAtIndex(i);
        this._settlePromise(promise, handler, receiver, value);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._fulfillmentHandlerAt"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_fulfillmentHandlerAt (index)](#apidoc.element.gulp-buster._Promise.prototype._fulfillmentHandlerAt)
- description and source-code
```javascript
_fulfillmentHandlerAt = function (index) {
    return this[
            index * 4 - 4 + 0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._getDisposer"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_getDisposer ()](#apidoc.element.gulp-buster._Promise.prototype._getDisposer)
- description and source-code
```javascript
_getDisposer = function () {
    return this._disposer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._invokeInternalOnCancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_invokeInternalOnCancel ()](#apidoc.element.gulp-buster._Promise.prototype._invokeInternalOnCancel)
- description and source-code
```javascript
_invokeInternalOnCancel = function () {
    if (this._isCancellable()) {
        this._doInvokeOnCancel(this._onCancel(), true);
        this._unsetOnCancel();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._invokeOnCancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_invokeOnCancel ()](#apidoc.element.gulp-buster._Promise.prototype._invokeOnCancel)
- description and source-code
```javascript
_invokeOnCancel = function () {
    var onCancelCallback = this._onCancel();
    this._unsetOnCancel();
    async.invoke(this._doInvokeOnCancel, this, onCancelCallback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isBound"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isBound ()](#apidoc.element.gulp-buster._Promise.prototype._isBound)
- description and source-code
```javascript
_isBound = function () {
    return (this._bitField & 2097152) === 2097152;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isCancellable"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isCancellable ()](#apidoc.element.gulp-buster._Promise.prototype._isCancellable)
- description and source-code
```javascript
_isCancellable = function () {
    return this.isPending() && !this._isCancelled();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._isCancelled)
- description and source-code
```javascript
_isCancelled = function () {
    return this._target().__isCancelled();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isDisposable"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isDisposable ()](#apidoc.element.gulp-buster._Promise.prototype._isDisposable)
- description and source-code
```javascript
_isDisposable = function () {
    return (this._bitField & 131072) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isFateSealed"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isFateSealed ()](#apidoc.element.gulp-buster._Promise.prototype._isFateSealed)
- description and source-code
```javascript
_isFateSealed = function () {
    return (this._bitField & 117506048) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isFinal"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isFinal ()](#apidoc.element.gulp-buster._Promise.prototype._isFinal)
- description and source-code
```javascript
_isFinal = function () {
    return (this._bitField & 4194304) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isFollowing"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isFollowing ()](#apidoc.element.gulp-buster._Promise.prototype._isFollowing)
- description and source-code
```javascript
_isFollowing = function () {
    return (this._bitField & 67108864) === 67108864;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isRejectionUnhandled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isRejectionUnhandled ()](#apidoc.element.gulp-buster._Promise.prototype._isRejectionUnhandled)
- description and source-code
```javascript
_isRejectionUnhandled = function () {
    return (this._bitField & 1048576) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._isUnhandledRejectionNotified"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_isUnhandledRejectionNotified ()](#apidoc.element.gulp-buster._Promise.prototype._isUnhandledRejectionNotified)
- description and source-code
```javascript
_isUnhandledRejectionNotified = function () {
    return (this._bitField & 262144) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._length"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_length ()](#apidoc.element.gulp-buster._Promise.prototype._length)
- description and source-code
```javascript
_length = function () {
    return this._bitField & 65535;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._migrateCallback0"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_migrateCallback0 (follower)](#apidoc.element.gulp-buster._Promise.prototype._migrateCallback0)
- description and source-code
```javascript
_migrateCallback0 = function (follower) {
    var bitField = follower._bitField;
    var fulfill = follower._fulfillmentHandler0;
    var reject = follower._rejectionHandler0;
    var promise = follower._promise0;
    var receiver = follower._receiverAt(0);
    if (receiver === undefined) receiver = UNDEFINED_BINDING;
    this._addCallbacks(fulfill, reject, promise, receiver, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._migrateCallbackAt"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_migrateCallbackAt (follower, index)](#apidoc.element.gulp-buster._Promise.prototype._migrateCallbackAt)
- description and source-code
```javascript
_migrateCallbackAt = function (follower, index) {
    var fulfill = follower._fulfillmentHandlerAt(index);
    var reject = follower._rejectionHandlerAt(index);
    var promise = follower._promiseAt(index);
    var receiver = follower._receiverAt(index);
    if (receiver === undefined) receiver = UNDEFINED_BINDING;
    this._addCallbacks(fulfill, reject, promise, receiver, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._notifyUnhandledRejection"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_notifyUnhandledRejection ()](#apidoc.element.gulp-buster._Promise.prototype._notifyUnhandledRejection)
- description and source-code
```javascript
_notifyUnhandledRejection = function () {
    if (this._isRejectionUnhandled()) {
        var reason = this._settledValue();
        this._setUnhandledRejectionIsNotified();
        fireRejectionEvent("unhandledRejection",
                                      possiblyUnhandledRejection, reason, this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._notifyUnhandledRejectionIsHandled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_notifyUnhandledRejectionIsHandled ()](#apidoc.element.gulp-buster._Promise.prototype._notifyUnhandledRejectionIsHandled)
- description and source-code
```javascript
_notifyUnhandledRejectionIsHandled = function () {
    fireRejectionEvent("rejectionHandled",
                                  unhandledRejectionHandled, undefined, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._onCancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_onCancel ()](#apidoc.element.gulp-buster._Promise.prototype._onCancel)
- description and source-code
```javascript
_onCancel = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._passThrough"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_passThrough (handler, type, success, fail)](#apidoc.element.gulp-buster._Promise.prototype._passThrough)
- description and source-code
```javascript
_passThrough = function (handler, type, success, fail) {
    if (typeof handler !== "function") return this.then();
    return this._then(success,
                      fail,
                      undefined,
                      new PassThroughHandlerContext(this, type, handler),
                      undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._peekContext"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_peekContext ()](#apidoc.element.gulp-buster._Promise.prototype._peekContext)
- description and source-code
```javascript
_peekContext = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._popContext"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_popContext ()](#apidoc.element.gulp-buster._Promise.prototype._popContext)
- description and source-code
```javascript
_popContext = function () {return null;}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._promiseAt"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_promiseAt (index)](#apidoc.element.gulp-buster._Promise.prototype._promiseAt)
- description and source-code
```javascript
_promiseAt = function (index) {
    return this[
            index * 4 - 4 + 2];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._promiseCreated"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_promiseCreated ()](#apidoc.element.gulp-buster._Promise.prototype._promiseCreated)
- description and source-code
```javascript
_promiseCreated = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._propagateFrom"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_propagateFrom (parent, flags)](#apidoc.element.gulp-buster._Promise.prototype._propagateFrom)
- description and source-code
```javascript
_propagateFrom = function (parent, flags) {
    ;
    ;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._proxy"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_proxy (proxyable, arg)](#apidoc.element.gulp-buster._Promise.prototype._proxy)
- description and source-code
```javascript
_proxy = function (proxyable, arg) {
    this._addCallbacks(undefined, undefined, arg, proxyable, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._pushContext"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_pushContext ()](#apidoc.element.gulp-buster._Promise.prototype._pushContext)
- description and source-code
```javascript
_pushContext = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._reason"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_reason ()](#apidoc.element.gulp-buster._Promise.prototype._reason)
- description and source-code
```javascript
_reason = function () {
    this._unsetRejectionIsUnhandled();
    return this._settledValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._receiverAt"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_receiverAt (index)](#apidoc.element.gulp-buster._Promise.prototype._receiverAt)
- description and source-code
```javascript
_receiverAt = function (index) {
    var ret = index === 0 ? this._receiver0 : this[
            index * 4 - 4 + 3];
    if (ret === UNDEFINED_BINDING) {
        return undefined;
    } else if (ret === undefined && this._isBound()) {
        return this._boundValue();
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._reject"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_reject (reason)](#apidoc.element.gulp-buster._Promise.prototype._reject)
- description and source-code
```javascript
_reject = function (reason) {
    var bitField = this._bitField;
    if (((bitField & 117506048) >>> 16)) return;
    this._setRejected();
    this._fulfillmentHandler0 = reason;

    if (this._isFinal()) {
        return async.fatalError(reason, util.isNode);
    }

    if ((bitField & 65535) > 0) {
        async.settlePromises(this);
    } else {
        this._ensurePossibleRejectionHandled();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._rejectCallback"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_rejectCallback (reason, synchronous, ignoreNonErrorWarnings)](#apidoc.element.gulp-buster._Promise.prototype._rejectCallback)
- description and source-code
```javascript
_rejectCallback = function (reason, synchronous, ignoreNonErrorWarnings) {
    var trace = util.ensureErrorObject(reason);
    var hasStack = trace === reason;
    if (!hasStack && !ignoreNonErrorWarnings && debug.warnings()) {
        var message = "a promise was rejected with a non-error: " +
            util.classString(reason);
        this._warn(message, true);
    }
    this._attachExtraTrace(trace, synchronous ? hasStack : false);
    this._reject(reason);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._rejectPromises"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_rejectPromises (len, reason)](#apidoc.element.gulp-buster._Promise.prototype._rejectPromises)
- description and source-code
```javascript
_rejectPromises = function (len, reason) {
    for (var i = 1; i < len; i++) {
        var handler = this._rejectionHandlerAt(i);
        var promise = this._promiseAt(i);
        var receiver = this._receiverAt(i);
        this._clearCallbackDataAtIndex(i);
        this._settlePromise(promise, handler, receiver, reason);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._rejectionHandlerAt"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_rejectionHandlerAt (index)](#apidoc.element.gulp-buster._Promise.prototype._rejectionHandlerAt)
- description and source-code
```javascript
_rejectionHandlerAt = function (index) {
    return this[
            index * 4 - 4 + 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._resolveCallback"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resolveCallback (value, shouldBind)](#apidoc.element.gulp-buster._Promise.prototype._resolveCallback)
- description and source-code
```javascript
_resolveCallback = function (value, shouldBind) {
    if (((this._bitField & 117506048) !== 0)) return;
    if (value === this)
        return this._rejectCallback(makeSelfResolutionError(), false);
    var maybePromise = tryConvertToPromise(value, this);
    if (!(maybePromise instanceof Promise)) return this._fulfill(value);

    if (shouldBind) this._propagateFrom(maybePromise, 2);

    var promise = maybePromise._target();

    if (promise === this) {
        this._reject(makeSelfResolutionError());
        return;
    }

    var bitField = promise._bitField;
    if (((bitField & 50397184) === 0)) {
        var len = this._length();
        if (len > 0) promise._migrateCallback0(this);
        for (var i = 1; i < len; ++i) {
            promise._migrateCallbackAt(this, i);
        }
        this._setFollowing();
        this._setLength(0);
        this._setFollowee(promise);
    } else if (((bitField & 33554432) !== 0)) {
        this._fulfill(promise._value());
    } else if (((bitField & 16777216) !== 0)) {
        this._reject(promise._reason());
    } else {
        var reason = new CancellationError("late cancellation observer");
        promise._attachExtraTrace(reason);
        this._reject(reason);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._resolveFromExecutor"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resolveFromExecutor (executor)](#apidoc.element.gulp-buster._Promise.prototype._resolveFromExecutor)
- description and source-code
```javascript
_resolveFromExecutor = function (executor) {
    if (executor === INTERNAL) return;
    var promise = this;
    this._captureStackTrace();
    this._pushContext();
    var synchronous = true;
    var r = this._execute(executor, function(value) {
        promise._resolveCallback(value);
    }, function (reason) {
        promise._rejectCallback(reason, synchronous);
    });
    synchronous = false;
    this._popContext();

    if (r !== undefined) {
        promise._rejectCallback(r, true);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._resolveFromSyncValue"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resolveFromSyncValue (value)](#apidoc.element.gulp-buster._Promise.prototype._resolveFromSyncValue)
- description and source-code
```javascript
_resolveFromSyncValue = function (value) {
    if (value === util.errorObj) {
        this._rejectCallback(value.e, false);
    } else {
        this._resolveCallback(value, true);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._resultCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_resultCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._resultCancelled)
- description and source-code
```javascript
_resultCancelled = function () {
    this.cancel();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._returnedNonUndefined"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_returnedNonUndefined ()](#apidoc.element.gulp-buster._Promise.prototype._returnedNonUndefined)
- description and source-code
```javascript
_returnedNonUndefined = function () {
    return (this._bitField & 268435456) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setAsyncGuaranteed"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setAsyncGuaranteed ()](#apidoc.element.gulp-buster._Promise.prototype._setAsyncGuaranteed)
- description and source-code
```javascript
_setAsyncGuaranteed = function () {
    if (async.hasCustomScheduler()) return;
    this._bitField = this._bitField | 134217728;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setBoundTo"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setBoundTo (obj)](#apidoc.element.gulp-buster._Promise.prototype._setBoundTo)
- description and source-code
```javascript
_setBoundTo = function (obj) {
    if (obj !== undefined) {
        this._bitField = this._bitField | 2097152;
        this._boundTo = obj;
    } else {
        this._bitField = this._bitField & (~2097152);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._setCancelled)
- description and source-code
```javascript
_setCancelled = function () {
    this._bitField = this._bitField | 65536;
    this._fireEvent("promiseCancelled", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setDisposable"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setDisposable (disposer)](#apidoc.element.gulp-buster._Promise.prototype._setDisposable)
- description and source-code
```javascript
_setDisposable = function (disposer) {
    this._bitField = this._bitField | 131072;
    this._disposer = disposer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setFollowee"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setFollowee (promise)](#apidoc.element.gulp-buster._Promise.prototype._setFollowee)
- description and source-code
```javascript
_setFollowee = function (promise) {
    this._rejectionHandler0 = promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setFollowing"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setFollowing ()](#apidoc.element.gulp-buster._Promise.prototype._setFollowing)
- description and source-code
```javascript
_setFollowing = function () {
    this._bitField = this._bitField | 67108864;
    this._fireEvent("promiseResolved", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setFulfilled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setFulfilled ()](#apidoc.element.gulp-buster._Promise.prototype._setFulfilled)
- description and source-code
```javascript
_setFulfilled = function () {
    this._bitField = this._bitField | 33554432;
    this._fireEvent("promiseFulfilled", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setIsFinal"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setIsFinal ()](#apidoc.element.gulp-buster._Promise.prototype._setIsFinal)
- description and source-code
```javascript
_setIsFinal = function () {
    this._bitField = this._bitField | 4194304;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setLength"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setLength (len)](#apidoc.element.gulp-buster._Promise.prototype._setLength)
- description and source-code
```javascript
_setLength = function (len) {
    this._bitField = (this._bitField & -65536) |
        (len & 65535);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setOnCancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setOnCancel (handler)](#apidoc.element.gulp-buster._Promise.prototype._setOnCancel)
- description and source-code
```javascript
_setOnCancel = function (handler) { ; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setRejected"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setRejected ()](#apidoc.element.gulp-buster._Promise.prototype._setRejected)
- description and source-code
```javascript
_setRejected = function () {
    this._bitField = this._bitField | 16777216;
    this._fireEvent("promiseRejected", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setRejectionIsUnhandled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setRejectionIsUnhandled ()](#apidoc.element.gulp-buster._Promise.prototype._setRejectionIsUnhandled)
- description and source-code
```javascript
_setRejectionIsUnhandled = function () {
    this._bitField = this._bitField | 1048576;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setReturnedNonUndefined"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setReturnedNonUndefined ()](#apidoc.element.gulp-buster._Promise.prototype._setReturnedNonUndefined)
- description and source-code
```javascript
_setReturnedNonUndefined = function () {
    this._bitField = this._bitField | 268435456;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setUnhandledRejectionIsNotified"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setUnhandledRejectionIsNotified ()](#apidoc.element.gulp-buster._Promise.prototype._setUnhandledRejectionIsNotified)
- description and source-code
```javascript
_setUnhandledRejectionIsNotified = function () {
    this._bitField = this._bitField | 262144;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._setWillBeCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_setWillBeCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._setWillBeCancelled)
- description and source-code
```javascript
_setWillBeCancelled = function () {
    this._bitField = this._bitField | 8388608;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._settlePromise"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromise (promise, handler, receiver, value)](#apidoc.element.gulp-buster._Promise.prototype._settlePromise)
- description and source-code
```javascript
_settlePromise = function (promise, handler, receiver, value) {
    var isPromise = promise instanceof Promise;
    var bitField = this._bitField;
    var asyncGuaranteed = ((bitField & 134217728) !== 0);
    if (((bitField & 65536) !== 0)) {
        if (isPromise) promise._invokeInternalOnCancel();

        if (receiver instanceof PassThroughHandlerContext &&
            receiver.isFinallyHandler()) {
            receiver.cancelPromise = promise;
            if (tryCatch(handler).call(receiver, value) === errorObj) {
                promise._reject(errorObj.e);
            }
        } else if (handler === reflectHandler) {
            promise._fulfill(reflectHandler.call(receiver));
        } else if (receiver instanceof Proxyable) {
            receiver._promiseCancelled(promise);
        } else if (isPromise || promise instanceof PromiseArray) {
            promise._cancel();
        } else {
            receiver.cancel();
        }
    } else if (typeof handler === "function") {
        if (!isPromise) {
            handler.call(receiver, value, promise);
        } else {
            if (asyncGuaranteed) promise._setAsyncGuaranteed();
            this._settlePromiseFromHandler(handler, receiver, value, promise);
        }
    } else if (receiver instanceof Proxyable) {
        if (!receiver._isResolved()) {
            if (((bitField & 33554432) !== 0)) {
                receiver._promiseFulfilled(value, promise);
            } else {
                receiver._promiseRejected(value, promise);
            }
        }
    } else if (isPromise) {
        if (asyncGuaranteed) promise._setAsyncGuaranteed();
        if (((bitField & 33554432) !== 0)) {
            promise._fulfill(value);
        } else {
            promise._reject(value);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._settlePromise0"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromise0 (handler, value, bitField)](#apidoc.element.gulp-buster._Promise.prototype._settlePromise0)
- description and source-code
```javascript
_settlePromise0 = function (handler, value, bitField) {
    var promise = this._promise0;
    var receiver = this._receiverAt(0);
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._settlePromise(promise, handler, receiver, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._settlePromiseCtx"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromiseCtx (ctx)](#apidoc.element.gulp-buster._Promise.prototype._settlePromiseCtx)
- description and source-code
```javascript
_settlePromiseCtx = function (ctx) {
    this._settlePromise(ctx.promise, ctx.handler, ctx.receiver, ctx.value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._settlePromiseFromHandler"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromiseFromHandler ( handler, receiver, value, promise )](#apidoc.element.gulp-buster._Promise.prototype._settlePromiseFromHandler)
- description and source-code
```javascript
_settlePromiseFromHandler = function ( handler, receiver, value, promise ) {
    var bitField = promise._bitField;
    if (((bitField & 65536) !== 0)) return;
    promise._pushContext();
    var x;
    if (receiver === APPLY) {
        if (!value || typeof value.length !== "number") {
            x = errorObj;
            x.e = new TypeError("cannot .spread() a non-array: " +
                                    util.classString(value));
        } else {
            x = tryCatch(handler).apply(this._boundValue(), value);
        }
    } else {
        x = tryCatch(handler).call(receiver, value);
    }
    var promiseCreated = promise._popContext();
    bitField = promise._bitField;
    if (((bitField & 65536) !== 0)) return;

    if (x === NEXT_FILTER) {
        promise._reject(value);
    } else if (x === errorObj) {
        promise._rejectCallback(x.e, false);
    } else {
        debug.checkForgottenReturns(x, promiseCreated, "",  promise, this);
        promise._resolveCallback(x);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._settlePromiseLateCancellationObserver"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromiseLateCancellationObserver (ctx)](#apidoc.element.gulp-buster._Promise.prototype._settlePromiseLateCancellationObserver)
- description and source-code
```javascript
_settlePromiseLateCancellationObserver = function (ctx) {
    var handler = ctx.handler;
    var promise = ctx.promise;
    var receiver = ctx.receiver;
    var value = ctx.value;
    if (typeof handler === "function") {
        if (!(promise instanceof Promise)) {
            handler.call(receiver, value, promise);
        } else {
            this._settlePromiseFromHandler(handler, receiver, value, promise);
        }
    } else if (promise instanceof Promise) {
        promise._reject(value);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._settlePromises"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settlePromises ()](#apidoc.element.gulp-buster._Promise.prototype._settlePromises)
- description and source-code
```javascript
_settlePromises = function () {
    var bitField = this._bitField;
    var len = (bitField & 65535);

    if (len > 0) {
        if (((bitField & 16842752) !== 0)) {
            var reason = this._fulfillmentHandler0;
            this._settlePromise0(this._rejectionHandler0, reason, bitField);
            this._rejectPromises(len, reason);
        } else {
            var value = this._rejectionHandler0;
            this._settlePromise0(this._fulfillmentHandler0, value, bitField);
            this._fulfillPromises(len, value);
        }
        this._setLength(0);
    }
    this._clearCancellationData();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._settledValue"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_settledValue ()](#apidoc.element.gulp-buster._Promise.prototype._settledValue)
- description and source-code
```javascript
_settledValue = function () {
    var bitField = this._bitField;
    if (((bitField & 33554432) !== 0)) {
        return this._rejectionHandler0;
    } else if (((bitField & 16777216) !== 0)) {
        return this._fulfillmentHandler0;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._target"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_target ()](#apidoc.element.gulp-buster._Promise.prototype._target)
- description and source-code
```javascript
_target = function () {
    var ret = this;
    while (ret._isFollowing()) ret = ret._followee();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._then"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_then ( didFulfill, didReject, _, receiver, internalData )](#apidoc.element.gulp-buster._Promise.prototype._then)
- description and source-code
```javascript
_then = function ( didFulfill, didReject, _, receiver, internalData ) {
    var haveInternalData = internalData !== undefined;
    var promise = haveInternalData ? internalData : new Promise(INTERNAL);
    var target = this._target();
    var bitField = target._bitField;

    if (!haveInternalData) {
        promise._propagateFrom(this, 3);
        promise._captureStackTrace();
        if (receiver === undefined &&
            ((this._bitField & 2097152) !== 0)) {
            if (!((bitField & 50397184) === 0)) {
                receiver = this._boundValue();
            } else {
                receiver = target === this ? undefined : this._boundTo;
            }
        }
        this._fireEvent("promiseChained", this, promise);
    }

    var domain = getDomain();
    if (!((bitField & 50397184) === 0)) {
        var handler, value, settler = target._settlePromiseCtx;
        if (((bitField & 33554432) !== 0)) {
            value = target._rejectionHandler0;
            handler = didFulfill;
        } else if (((bitField & 16777216) !== 0)) {
            value = target._fulfillmentHandler0;
            handler = didReject;
            target._unsetRejectionIsUnhandled();
        } else {
            settler = target._settlePromiseLateCancellationObserver;
            value = new CancellationError("late cancellation observer");
            target._attachExtraTrace(value);
            handler = didReject;
        }

        async.invoke(settler, target, {
            handler: domain === null ? handler
                : (typeof handler === "function" &&
                    util.domainBind(domain, handler)),
            promise: promise,
            receiver: receiver,
            value: value
        });
    } else {
        target._addCallbacks(didFulfill, didReject, promise, receiver, domain);
    }

    return promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._unsetCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetCancelled ()](#apidoc.element.gulp-buster._Promise.prototype._unsetCancelled)
- description and source-code
```javascript
_unsetCancelled = function () {
    this._bitField = this._bitField & (~65536);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._unsetDisposable"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetDisposable ()](#apidoc.element.gulp-buster._Promise.prototype._unsetDisposable)
- description and source-code
```javascript
_unsetDisposable = function () {
    this._bitField = this._bitField & (~131072);
    this._disposer = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._unsetOnCancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetOnCancel ()](#apidoc.element.gulp-buster._Promise.prototype._unsetOnCancel)
- description and source-code
```javascript
_unsetOnCancel = function () {
    this._onCancelField = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._unsetRejectionIsUnhandled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetRejectionIsUnhandled ()](#apidoc.element.gulp-buster._Promise.prototype._unsetRejectionIsUnhandled)
- description and source-code
```javascript
_unsetRejectionIsUnhandled = function () {
    this._bitField = this._bitField & (~1048576);
    if (this._isUnhandledRejectionNotified()) {
        this._unsetUnhandledRejectionIsNotified();
        this._notifyUnhandledRejectionIsHandled();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._unsetUnhandledRejectionIsNotified"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_unsetUnhandledRejectionIsNotified ()](#apidoc.element.gulp-buster._Promise.prototype._unsetUnhandledRejectionIsNotified)
- description and source-code
```javascript
_unsetUnhandledRejectionIsNotified = function () {
    this._bitField = this._bitField & (~262144);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._value"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_value ()](#apidoc.element.gulp-buster._Promise.prototype._value)
- description and source-code
```javascript
_value = function () {
    return this._settledValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype._warn"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>_warn (message, shouldUseOwnTrace, promise)](#apidoc.element.gulp-buster._Promise.prototype._warn)
- description and source-code
```javascript
_warn = function (message, shouldUseOwnTrace, promise) {
    return warn(message, shouldUseOwnTrace, promise || this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.all"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>all ()](#apidoc.element.gulp-buster._Promise.prototype.all)
- description and source-code
```javascript
all = function () {
    if (arguments.length > 0) {
        this._warn(".all() was passed arguments but it does not take any");
    }
    return new PromiseArray(this).promise();
}
```
- example usage
```shell
...
				if (typeof hashed !== 'string') throw error('Return/fulfill value of 'options.algo' must be a string');
				hashes[relativePath(file.cwd, options.relativePath, file.path)] = sliceHash(hashed, options);
			})
		);
	}

	function endStream() {
		Promise.all(hashingPromises).bind(this).then(function() {
			return options.transform.call(undefined, assign({}, hashes));
		}).then(function(transformed) {
			return options.formatter.call(undefined, transformed);
		}).then(function(formatted) {
			if (typeof formatted !== 'string') throw error('Return/fulfill value of 'options.formatter' must be a string');

			this.emit('data', new gutil.File({
...
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.any"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>any ()](#apidoc.element.gulp-buster._Promise.prototype.any)
- description and source-code
```javascript
any = function () {
    return any(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.asCallback"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>asCallback (nodeback, options)](#apidoc.element.gulp-buster._Promise.prototype.asCallback)
- description and source-code
```javascript
asCallback = function (nodeback, options) {
    if (typeof nodeback == "function") {
        var adapter = successAdapter;
        if (options !== undefined && Object(options).spread) {
            adapter = spreadAdapter;
        }
        this._then(
            adapter,
            errorAdapter,
            undefined,
            this,
            nodeback
        );
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.bind"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>bind (thisArg)](#apidoc.element.gulp-buster._Promise.prototype.bind)
- description and source-code
```javascript
bind = function (thisArg) {
    if (!calledBind) {
        calledBind = true;
        Promise.prototype._propagateFrom = debug.propagateFromFunction();
        Promise.prototype._boundValue = debug.boundValueFunction();
    }
    var maybePromise = tryConvertToPromise(thisArg);
    var ret = new Promise(INTERNAL);
    ret._propagateFrom(this, 1);
    var target = this._target();
    ret._setBoundTo(maybePromise);
    if (maybePromise instanceof Promise) {
        var context = {
            promiseRejectionQueued: false,
            promise: ret,
            target: target,
            bindingPromise: maybePromise
        };
        target._then(INTERNAL, targetRejected, undefined, ret, context);
        maybePromise._then(
            bindingResolved, bindingRejected, undefined, ret, context);
        ret._setOnCancel(maybePromise);
    } else {
        ret._resolveCallback(target);
    }
    return ret;
}
```
- example usage
```shell
...

	function hashFile(file) {
		if (file.isNull()) return; // ignore
		if (file.isStream()) return this.emit('error', error('Streaming not supported'));

		// start hashing files as soon as they are received for maximum concurrency
		hashingPromises.push(
			Promise.try(hash.bind(undefined, file, options)).then(function(hashed) {
				if (typeof hashed !== 'string') throw error('Return/fulfill value of 'options.algo' must be a string');
				hashes[relativePath(file.cwd, options.relativePath, file.path)] = sliceHash(hashed, options);
			})
		);
	}

	function endStream() {
...
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.break"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>break ()](#apidoc.element.gulp-buster._Promise.prototype.break)
- description and source-code
```javascript
break = function () {
    if (!debug.cancellation()) return this._warn("cancellation is disabled");

    var promise = this;
    var child = promise;
    while (promise._isCancellable()) {
        if (!promise._cancelBy(child)) {
            if (child._isFollowing()) {
                child._followee().cancel();
            } else {
                child._cancelBranched();
            }
            break;
        }

        var parent = promise._cancellationParent;
        if (parent == null || !parent._isCancellable()) {
            if (promise._isFollowing()) {
                promise._followee().cancel();
            } else {
                promise._cancelBranched();
            }
            break;
        } else {
            if (promise._isFollowing()) promise._followee().cancel();
            promise._setWillBeCancelled();
            child = promise;
            promise = parent;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.call"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>call (methodName)](#apidoc.element.gulp-buster._Promise.prototype.call)
- description and source-code
```javascript
call = function (methodName) {
    var $_len = arguments.length;var args = new Array(Math.max($_len - 1, 0)); for(var $_i = 1; $_i < $_len; ++$_i) {args[$_i -
1] = arguments[$_i];};
    if (!false) {
        if (canEvaluate) {
            var maybeCaller = getMethodCaller(methodName);
            if (maybeCaller !== null) {
                return this._then(
                    maybeCaller, undefined, undefined, args, undefined);
            }
        }
    }
    args.push(methodName);
    return this._then(caller, undefined, undefined, args, undefined);
}
```
- example usage
```shell
...

function error(msg) {
	return new gutil.PluginError('gulp-buster', msg);
}

function hash(file, options) {
	return typeof options.algo === 'function'
		? options.algo.call(undefined, file)
		: crypto.createHash(options.algo).update(file.contents).digest('hex');
}

function sliceHash(hash, options) {
	// positive length = leading characters; negative = trailing
	return options.length
		? options.length > 0
...
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.cancel"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>cancel ()](#apidoc.element.gulp-buster._Promise.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
    if (!debug.cancellation()) return this._warn("cancellation is disabled");

    var promise = this;
    var child = promise;
    while (promise._isCancellable()) {
        if (!promise._cancelBy(child)) {
            if (child._isFollowing()) {
                child._followee().cancel();
            } else {
                child._cancelBranched();
            }
            break;
        }

        var parent = promise._cancellationParent;
        if (parent == null || !parent._isCancellable()) {
            if (promise._isFollowing()) {
                promise._followee().cancel();
            } else {
                promise._cancelBranched();
            }
            break;
        } else {
            if (promise._isFollowing()) promise._followee().cancel();
            promise._setWillBeCancelled();
            child = promise;
            promise = parent;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.catch"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>catch (fn)](#apidoc.element.gulp-buster._Promise.prototype.catch)
- description and source-code
```javascript
catch = function (fn) {
    var len = arguments.length;
    if (len > 1) {
        var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (util.isObject(item)) {
                catchInstances[j++] = item;
            } else {
                return apiRejection("Catch statement predicate: " +
                    "expecting an object but got " + util.classString(item));
            }
        }
        catchInstances.length = j;
        fn = arguments[i];
        return this.then(undefined, catchFilter(catchInstances, fn, this));
    }
    return this.then(undefined, fn);
}
```
- example usage
```shell
...
			if (typeof formatted !== 'string') throw error('Return/fulfill value of 'options.formatter' must be a string');

			this.emit('data', new gutil.File({
				path: path.join(process.cwd(), options.fileName),
				contents: new Buffer(formatted),
			}));
			this.emit('end');
		}).catch(function(err) {
			this.emit('error', err instanceof gutil.PluginError ? err : error(err));
		});
	}

	return through(hashFile, endStream);
};
...
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.catchReturn"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>catchReturn (value)](#apidoc.element.gulp-buster._Promise.prototype.catchReturn)
- description and source-code
```javascript
catchReturn = function (value) {
    if (arguments.length <= 1) {
        if (value instanceof Promise) value.suppressUnhandledRejections();
        return this._then(
            undefined, returner, undefined, {value: value}, undefined);
    } else {
        var _value = arguments[1];
        if (_value instanceof Promise) _value.suppressUnhandledRejections();
        var handler = function() {return _value;};
        return this.caught(value, handler);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.catchThrow"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>catchThrow (reason)](#apidoc.element.gulp-buster._Promise.prototype.catchThrow)
- description and source-code
```javascript
catchThrow = function (reason) {
    if (arguments.length <= 1) {
        return this._then(
            undefined, thrower, undefined, {reason: reason}, undefined);
    } else {
        var _reason = arguments[1];
        var handler = function() {throw _reason;};
        return this.caught(reason, handler);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.caught"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>caught (fn)](#apidoc.element.gulp-buster._Promise.prototype.caught)
- description and source-code
```javascript
caught = function (fn) {
    var len = arguments.length;
    if (len > 1) {
        var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (util.isObject(item)) {
                catchInstances[j++] = item;
            } else {
                return apiRejection("Catch statement predicate: " +
                    "expecting an object but got " + util.classString(item));
            }
        }
        catchInstances.length = j;
        fn = arguments[i];
        return this.then(undefined, catchFilter(catchInstances, fn, this));
    }
    return this.then(undefined, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.delay"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>delay (ms)](#apidoc.element.gulp-buster._Promise.prototype.delay)
- description and source-code
```javascript
delay = function (ms) {
    return delay(ms, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.disposer"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>disposer (fn)](#apidoc.element.gulp-buster._Promise.prototype.disposer)
- description and source-code
```javascript
disposer = function (fn) {
    if (typeof fn === "function") {
        return new FunctionDisposer(fn, this, createContext());
    }
    throw new TypeError();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.done"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>done (didFulfill, didReject)](#apidoc.element.gulp-buster._Promise.prototype.done)
- description and source-code
```javascript
done = function (didFulfill, didReject) {
    var promise =
        this._then(didFulfill, didReject, undefined, undefined, undefined);
    promise._setIsFinal();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.each"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>each (fn)](#apidoc.element.gulp-buster._Promise.prototype.each)
- description and source-code
```javascript
each = function (fn) {
    return PromiseReduce(this, fn, INTERNAL, 0)
              ._then(promiseAllThis, undefined, undefined, this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.error"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>error (fn)](#apidoc.element.gulp-buster._Promise.prototype.error)
- description and source-code
```javascript
error = function (fn) {
    return this.caught(util.originatesFromRejection, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.filter"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>filter (fn, options)](#apidoc.element.gulp-buster._Promise.prototype.filter)
- description and source-code
```javascript
filter = function (fn, options) {
    return PromiseMap(this, fn, options, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.finally"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>finally (handler)](#apidoc.element.gulp-buster._Promise.prototype.finally)
- description and source-code
```javascript
finally = function (handler) {
    return this._passThrough(handler,
                             0,
                             finallyHandler,
                             finallyHandler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.get"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>get (propertyName)](#apidoc.element.gulp-buster._Promise.prototype.get)
- description and source-code
```javascript
get = function (propertyName) {
    var isIndex = (typeof propertyName === "number");
    var getter;
    if (!isIndex) {
        if (canEvaluate) {
            var maybeGetter = getGetter(propertyName);
            getter = maybeGetter !== null ? maybeGetter : namedGetter;
        } else {
            getter = namedGetter;
        }
    } else {
        getter = indexedGetter;
    }
    return this._then(getter, undefined, undefined, propertyName, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.isCancellable"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isCancellable ()](#apidoc.element.gulp-buster._Promise.prototype.isCancellable)
- description and source-code
```javascript
isCancellable = function () {
    return this.isPending() && !this.isCancelled();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.isCancelled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isCancelled ()](#apidoc.element.gulp-buster._Promise.prototype.isCancelled)
- description and source-code
```javascript
isCancelled = function () {
    return (this._target()._bitField & 8454144) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.isFulfilled"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isFulfilled ()](#apidoc.element.gulp-buster._Promise.prototype.isFulfilled)
- description and source-code
```javascript
isFulfilled = function () {
    return isFulfilled.call(this._target());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.isPending"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isPending ()](#apidoc.element.gulp-buster._Promise.prototype.isPending)
- description and source-code
```javascript
isPending = function () {
    return isPending.call(this._target());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.isRejected"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isRejected ()](#apidoc.element.gulp-buster._Promise.prototype.isRejected)
- description and source-code
```javascript
isRejected = function () {
    return isRejected.call(this._target());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.isResolved"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>isResolved ()](#apidoc.element.gulp-buster._Promise.prototype.isResolved)
- description and source-code
```javascript
isResolved = function () {
    return isResolved.call(this._target());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.lastly"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>lastly (handler)](#apidoc.element.gulp-buster._Promise.prototype.lastly)
- description and source-code
```javascript
lastly = function (handler) {
    return this._passThrough(handler,
                             0,
                             finallyHandler,
                             finallyHandler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.map"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>map (fn, options)](#apidoc.element.gulp-buster._Promise.prototype.map)
- description and source-code
```javascript
map = function (fn, options) {
    return map(this, fn, options, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.mapSeries"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>mapSeries (fn)](#apidoc.element.gulp-buster._Promise.prototype.mapSeries)
- description and source-code
```javascript
mapSeries = function (fn) {
    return PromiseReduce(this, fn, INTERNAL, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.nodeify"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>nodeify (nodeback, options)](#apidoc.element.gulp-buster._Promise.prototype.nodeify)
- description and source-code
```javascript
nodeify = function (nodeback, options) {
    if (typeof nodeback == "function") {
        var adapter = successAdapter;
        if (options !== undefined && Object(options).spread) {
            adapter = spreadAdapter;
        }
        this._then(
            adapter,
            errorAdapter,
            undefined,
            this,
            nodeback
        );
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.props"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>props ()](#apidoc.element.gulp-buster._Promise.prototype.props)
- description and source-code
```javascript
props = function () {
    return props(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.race"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>race ()](#apidoc.element.gulp-buster._Promise.prototype.race)
- description and source-code
```javascript
race = function () {
    return race(this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.reason"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>reason ()](#apidoc.element.gulp-buster._Promise.prototype.reason)
- description and source-code
```javascript
reason = function () {
    var target = this._target();
    target._unsetRejectionIsUnhandled();
    return reason.call(target);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.reduce"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>reduce (fn, initialValue)](#apidoc.element.gulp-buster._Promise.prototype.reduce)
- description and source-code
```javascript
reduce = function (fn, initialValue) {
    return reduce(this, fn, initialValue, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.reflect"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>reflect ()](#apidoc.element.gulp-buster._Promise.prototype.reflect)
- description and source-code
```javascript
reflect = function () {
    return this._then(reflectHandler,
        reflectHandler, undefined, this, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.return"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>return (value)](#apidoc.element.gulp-buster._Promise.prototype.return)
- description and source-code
```javascript
return = function (value) {
    if (value instanceof Promise) value.suppressUnhandledRejections();
    return this._then(
        returner, undefined, undefined, {value: value}, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.settle"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>settle ()](#apidoc.element.gulp-buster._Promise.prototype.settle)
- description and source-code
```javascript
settle = function () {
    return Promise.settle(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.some"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>some (howMany)](#apidoc.element.gulp-buster._Promise.prototype.some)
- description and source-code
```javascript
some = function (howMany) {
    return some(this, howMany);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.spread"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>spread (fn)](#apidoc.element.gulp-buster._Promise.prototype.spread)
- description and source-code
```javascript
spread = function (fn) {
    if (typeof fn !== "function") {
        return apiRejection("expecting a function but got " + util.classString(fn));
    }
    return this.all()._then(fn, undefined, undefined, APPLY, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.suppressUnhandledRejections"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>suppressUnhandledRejections ()](#apidoc.element.gulp-buster._Promise.prototype.suppressUnhandledRejections)
- description and source-code
```javascript
suppressUnhandledRejections = function () {
    var target = this._target();
    target._bitField = ((target._bitField & (~1048576)) |
                      524288);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.tap"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>tap (handler)](#apidoc.element.gulp-buster._Promise.prototype.tap)
- description and source-code
```javascript
tap = function (handler) {
    return this._passThrough(handler, 1, finallyHandler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.tapCatch"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>tapCatch (handlerOrPredicate)](#apidoc.element.gulp-buster._Promise.prototype.tapCatch)
- description and source-code
```javascript
tapCatch = function (handlerOrPredicate) {
    var len = arguments.length;
    if(len === 1) {
        return this._passThrough(handlerOrPredicate,
                                 1,
                                 undefined,
                                 finallyHandler);
    } else {
         var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (util.isObject(item)) {
                catchInstances[j++] = item;
            } else {
                return Promise.reject(new TypeError(
                    "tapCatch statement predicate: "
                    + "expecting an object but got " + util.classString(item)
                ));
            }
        }
        catchInstances.length = j;
        var handler = arguments[i];
        return this._passThrough(catchFilter(catchInstances, handler, this),
                                 1,
                                 undefined,
                                 finallyHandler);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.then"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>then (didFulfill, didReject)](#apidoc.element.gulp-buster._Promise.prototype.then)
- description and source-code
```javascript
then = function (didFulfill, didReject) {
    if (debug.warnings() && arguments.length > 0 &&
        typeof didFulfill !== "function" &&
        typeof didReject !== "function") {
        var msg = ".then() only accepts functions but was passed: " +
                util.classString(didFulfill);
        if (arguments.length > 1) {
            msg += ", " + util.classString(didReject);
        }
        this._warn(msg);
    }
    return this._then(didFulfill, didReject, undefined, undefined, undefined);
}
```
- example usage
```shell
...

	function hashFile(file) {
		if (file.isNull()) return; // ignore
		if (file.isStream()) return this.emit('error', error('Streaming not supported'));

		// start hashing files as soon as they are received for maximum concurrency
		hashingPromises.push(
			Promise.try(hash.bind(undefined, file, options)).then(function(hashed) {
				if (typeof hashed !== 'string') throw error('Return/fulfill value of 'options.algo' must be a string');
				hashes[relativePath(file.cwd, options.relativePath, file.path)] = sliceHash(hashed, options);
			})
		);
	}

	function endStream() {
...
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.thenReturn"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>thenReturn (value)](#apidoc.element.gulp-buster._Promise.prototype.thenReturn)
- description and source-code
```javascript
thenReturn = function (value) {
    if (value instanceof Promise) value.suppressUnhandledRejections();
    return this._then(
        returner, undefined, undefined, {value: value}, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.thenThrow"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>thenThrow (reason)](#apidoc.element.gulp-buster._Promise.prototype.thenThrow)
- description and source-code
```javascript
thenThrow = function (reason) {
    return this._then(
        thrower, undefined, undefined, {reason: reason}, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.throw"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>throw (reason)](#apidoc.element.gulp-buster._Promise.prototype.throw)
- description and source-code
```javascript
throw = function (reason) {
    return this._then(
        thrower, undefined, undefined, {reason: reason}, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.timeout"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>timeout (ms, message)](#apidoc.element.gulp-buster._Promise.prototype.timeout)
- description and source-code
```javascript
timeout = function (ms, message) {
    ms = +ms;
    var ret, parent;

    var handleWrapper = new HandleWrapper(setTimeout(function timeoutTimeout() {
        if (ret.isPending()) {
            afterTimeout(ret, message, parent);
        }
    }, ms));

    if (debug.cancellation()) {
        parent = this.then();
        ret = parent._then(successClear, failureClear,
                            undefined, handleWrapper, undefined);
        ret._setOnCancel(handleWrapper);
    } else {
        ret = this._then(successClear, failureClear,
                            undefined, handleWrapper, undefined);
    }

    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>toJSON ()](#apidoc.element.gulp-buster._Promise.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    var ret = {
        isFulfilled: false,
        isRejected: false,
        fulfillmentValue: undefined,
        rejectionReason: undefined
    };
    if (this.isFulfilled()) {
        ret.fulfillmentValue = this.value();
        ret.isFulfilled = true;
    } else if (this.isRejected()) {
        ret.rejectionReason = this.reason();
        ret.isRejected = true;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.toString"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>toString ()](#apidoc.element.gulp-buster._Promise.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return "[object Promise]";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-buster._Promise.prototype.value"></a>[function <span class="apidocSignatureSpan">gulp-buster._Promise.prototype.</span>value ()](#apidoc.element.gulp-buster._Promise.prototype.value)
- description and source-code
```javascript
value = function () {
    return value.call(this._target());
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
