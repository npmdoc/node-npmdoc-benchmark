# api documentation for  [benchmark (v2.1.4)](https://benchmarkjs.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-benchmark.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-benchmark) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-benchmark.svg)](https://travis-ci.org/npmdoc/node-npmdoc-benchmark)
#### A benchmarking library that supports high-resolution timers & returns statistically significant results.

[![NPM](https://nodei.co/npm/benchmark.png?downloads=true)](https://www.npmjs.com/package/benchmark)

[![apidoc](https://npmdoc.github.io/node-npmdoc-benchmark/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-benchmark_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-benchmark/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-benchmark/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Mathias Bynens",
        "email": "mathias@qiwi.be",
        "url": "https://mathiasbynens.be/"
    },
    "bugs": {
        "url": "https://github.com/bestiejs/benchmark.js/issues"
    },
    "contributors": [
        {
            "name": "Mathias Bynens",
            "email": "mathias@qiwi.be",
            "url": "https://mathiasbynens.be/"
        },
        {
            "name": "John-David Dalton",
            "email": "john.david.dalton@gmail.com",
            "url": "http://allyoucanleet.com/"
        },
        {
            "name": "Kit Cambridge",
            "email": "github@kitcambridge.be",
            "url": "http://kitcambridge.be/"
        }
    ],
    "dependencies": {
        "lodash": "^4.17.4",
        "platform": "^1.3.3"
    },
    "description": "A benchmarking library that supports high-resolution timers & returns statistically significant results.",
    "devDependencies": {
        "coveralls": "^2.12.0",
        "docdown": "~0.7.2",
        "istanbul": "0.4.5",
        "qunit-extras": "^3.0.0",
        "qunitjs": "^2.2.1",
        "requirejs": "^2.3.3"
    },
    "directories": {},
    "dist": {
        "shasum": "09f3de31c916425d498cc2ee565a0ebf3c2a5629",
        "tarball": "https://registry.npmjs.org/benchmark/-/benchmark-2.1.4.tgz"
    },
    "files": [
        "benchmark.js"
    ],
    "homepage": "https://benchmarkjs.com/",
    "keywords": [
        "benchmark",
        "performance",
        "speed"
    ],
    "license": "MIT",
    "main": "benchmark.js",
    "maintainers": [
        {
            "name": "jdalton",
            "email": "john@fusejs.com"
        },
        {
            "name": "mathias",
            "email": "mathias@qiwi.be"
        }
    ],
    "name": "benchmark",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/bestiejs/benchmark.js.git"
    },
    "scripts": {
        "doc": "docdown benchmark.js doc/README.md style=github title=\"<a href=\\\"https://benchmarkjs.com/\\\">Benchmark.js</a> <span>v${npm_package_version}</span>\" toc=categories url=https://github.com/bestiejs/benchmark.js/blob/${npm_package_version}/benchmark.js",
        "test": "node test/test"
    },
    "version": "2.1.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module benchmark](#apidoc.module.benchmark)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>Benchmark (name, fn, options)](#apidoc.element.benchmark.Benchmark)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>Deferred (clone)](#apidoc.element.benchmark.Deferred)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>Event (type)](#apidoc.element.benchmark.Event)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>Suite (name, options)](#apidoc.element.benchmark.Suite)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>each (collection, iteratee)](#apidoc.element.benchmark.each)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>filter (array, callback)](#apidoc.element.benchmark.filter)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>forEach (collection, iteratee)](#apidoc.element.benchmark.forEach)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>forOwn (object, iteratee)](#apidoc.element.benchmark.forOwn)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>formatNumber (number)](#apidoc.element.benchmark.formatNumber)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>has (object, path)](#apidoc.element.benchmark.has)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>indexOf (array, value, fromIndex)](#apidoc.element.benchmark.indexOf)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>invoke (benches, name)](#apidoc.element.benchmark.invoke)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>join (object, separator1, separator2)](#apidoc.element.benchmark.join)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>map (collection, iteratee)](#apidoc.element.benchmark.map)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>reduce (collection, iteratee, accumulator)](#apidoc.element.benchmark.reduce)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>runInContext (context)](#apidoc.element.benchmark.runInContext)
1.  object <span class="apidocSignatureSpan">benchmark.</span>Deferred.prototype
1.  object <span class="apidocSignatureSpan">benchmark.</span>Suite.prototype
1.  object <span class="apidocSignatureSpan">benchmark.</span>options
1.  object <span class="apidocSignatureSpan">benchmark.</span>platform
1.  object <span class="apidocSignatureSpan">benchmark.</span>platform.os
1.  object <span class="apidocSignatureSpan">benchmark.</span>support
1.  string <span class="apidocSignatureSpan">benchmark.</span>version

#### [module benchmark.Deferred](#apidoc.module.benchmark.Deferred)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>Deferred (clone)](#apidoc.element.benchmark.Deferred.Deferred)

#### [module benchmark.Deferred.prototype](#apidoc.module.benchmark.Deferred.prototype)
1.  [function <span class="apidocSignatureSpan">benchmark.Deferred.prototype.</span>resolve ()](#apidoc.element.benchmark.Deferred.prototype.resolve)
1.  number <span class="apidocSignatureSpan">benchmark.Deferred.prototype.</span>cycles
1.  number <span class="apidocSignatureSpan">benchmark.Deferred.prototype.</span>elapsed
1.  number <span class="apidocSignatureSpan">benchmark.Deferred.prototype.</span>timeStamp
1.  object <span class="apidocSignatureSpan">benchmark.Deferred.prototype.</span>benchmark

#### [module benchmark.Suite](#apidoc.module.benchmark.Suite)
1.  [function <span class="apidocSignatureSpan">benchmark.</span>Suite (name, options)](#apidoc.element.benchmark.Suite.Suite)
1.  object <span class="apidocSignatureSpan">benchmark.Suite.</span>options

#### [module benchmark.Suite.prototype](#apidoc.module.benchmark.Suite.prototype)
1.  boolean <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>aborted
1.  boolean <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>running
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>abort ()](#apidoc.element.benchmark.Suite.prototype.abort)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>add (name, fn, options)](#apidoc.element.benchmark.Suite.prototype.add)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>clone (options)](#apidoc.element.benchmark.Suite.prototype.clone)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>each ()](#apidoc.element.benchmark.Suite.prototype.each)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>emit (type)](#apidoc.element.benchmark.Suite.prototype.emit)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>filter (callback)](#apidoc.element.benchmark.Suite.prototype.filter)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>forEach ()](#apidoc.element.benchmark.Suite.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>indexOf ()](#apidoc.element.benchmark.Suite.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>join ()](#apidoc.element.benchmark.Suite.prototype.join)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>listeners (type)](#apidoc.element.benchmark.Suite.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>map ()](#apidoc.element.benchmark.Suite.prototype.map)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>off (type, listener)](#apidoc.element.benchmark.Suite.prototype.off)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>on (type, listener)](#apidoc.element.benchmark.Suite.prototype.on)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>pop ()](#apidoc.element.benchmark.Suite.prototype.pop)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>push ()](#apidoc.element.benchmark.Suite.prototype.push)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>reduce ()](#apidoc.element.benchmark.Suite.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>reset ()](#apidoc.element.benchmark.Suite.prototype.reset)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>reverse ()](#apidoc.element.benchmark.Suite.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>run (options)](#apidoc.element.benchmark.Suite.prototype.run)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>shift ()](#apidoc.element.benchmark.Suite.prototype.shift)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>slice ()](#apidoc.element.benchmark.Suite.prototype.slice)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>sort ()](#apidoc.element.benchmark.Suite.prototype.sort)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>splice ()](#apidoc.element.benchmark.Suite.prototype.splice)
1.  [function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>unshift ()](#apidoc.element.benchmark.Suite.prototype.unshift)
1.  number <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>length

#### [module benchmark.platform](#apidoc.module.benchmark.platform)
1.  [function <span class="apidocSignatureSpan">benchmark.platform.</span>parse (ua)](#apidoc.element.benchmark.platform.parse)
1.  [function <span class="apidocSignatureSpan">benchmark.platform.</span>toString ()](#apidoc.element.benchmark.platform.toString)
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>description
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>layout
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>manufacturer
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>name
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>os
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>prerelease
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>product
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>ua
1.  object <span class="apidocSignatureSpan">benchmark.platform.</span>version

#### [module benchmark.platform.os](#apidoc.module.benchmark.platform.os)
1.  [function <span class="apidocSignatureSpan">benchmark.platform.os.</span>toString ()](#apidoc.element.benchmark.platform.os.toString)
1.  object <span class="apidocSignatureSpan">benchmark.platform.os.</span>architecture
1.  object <span class="apidocSignatureSpan">benchmark.platform.os.</span>family
1.  object <span class="apidocSignatureSpan">benchmark.platform.os.</span>version



# <a name="apidoc.module.benchmark"></a>[module benchmark](#apidoc.module.benchmark)

#### <a name="apidoc.element.benchmark.Benchmark"></a>[function <span class="apidocSignatureSpan">benchmark.</span>Benchmark (name, fn, options)](#apidoc.element.benchmark.Benchmark)
- description and source-code
```javascript
function Benchmark(name, fn, options) {
  var bench = this;

  // Allow instance creation without the 'new' operator.
  if (!(bench instanceof Benchmark)) {
    return new Benchmark(name, fn, options);
  }
  // Juggle arguments.
  if (_.isPlainObject(name)) {
    // 1 argument (options).
    options = name;
  }
  else if (_.isFunction(name)) {
    // 2 arguments (fn, options).
    options = fn;
    fn = name;
  }
  else if (_.isPlainObject(fn)) {
    // 2 arguments (name, options).
    options = fn;
    fn = null;
    bench.name = name;
  }
  else {
    // 3 arguments (name, fn [, options]).
    bench.name = name;
  }
  setOptions(bench, options);

  bench.id || (bench.id = ++counter);
  bench.fn == null && (bench.fn = fn);

  bench.stats = cloneDeep(bench.stats);
  bench.times = cloneDeep(bench.times);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.Deferred"></a>[function <span class="apidocSignatureSpan">benchmark.</span>Deferred (clone)](#apidoc.element.benchmark.Deferred)
- description and source-code
```javascript
function Deferred(clone) {
  var deferred = this;
  if (!(deferred instanceof Deferred)) {
    return new Deferred(clone);
  }
  deferred.benchmark = clone;
  clock(deferred);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.Event"></a>[function <span class="apidocSignatureSpan">benchmark.</span>Event (type)](#apidoc.element.benchmark.Event)
- description and source-code
```javascript
function Event(type) {
  var event = this;
  if (type instanceof Event) {
    return type;
  }
  return (event instanceof Event)
    ? _.assign(event, { 'timeStamp': _.now() }, typeof type == 'string' ? { 'type': type } : type)
    : new Event(type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.Suite"></a>[function <span class="apidocSignatureSpan">benchmark.</span>Suite (name, options)](#apidoc.element.benchmark.Suite)
- description and source-code
```javascript
function Suite(name, options) {
  var suite = this;

  // Allow instance creation without the 'new' operator.
  if (!(suite instanceof Suite)) {
    return new Suite(name, options);
  }
  // Juggle arguments.
  if (_.isPlainObject(name)) {
    // 1 argument (options).
    options = name;
  } else {
    // 2 arguments (name [, options]).
    suite.name = name;
  }
  setOptions(suite, options);
}
```
- example usage
```shell
...
* @param {Object} [options={}] Options object.
* @example
*
* // basic usage (the 'new' operator is optional)
* var suite = new Benchmark.Suite;
*
* // or using a name first
* var suite = new Benchmark.Suite('foo');
*
* // or with options
* var suite = new Benchmark.Suite('foo', {
*
*   // called when the suite starts running
*   'onStart': onStart,
*
...
```

#### <a name="apidoc.element.benchmark.each"></a>[function <span class="apidocSignatureSpan">benchmark.</span>each (collection, iteratee)](#apidoc.element.benchmark.each)
- description and source-code
```javascript
function forEach(collection, iteratee) {
  var func = isArray(collection) ? arrayEach : baseEach;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
...
    function setOptions(object, options) {
options = object.options = _.assign({}, cloneDeep(object.constructor.options), cloneDeep(options));

_.forOwn(options, function(value, key) {
  if (value != null) {
    // Add event listeners.
    if (/^on[A-Z]/.test(key)) {
      _.each(key.split(' '), function(key) {
        object.on(key.slice(2).toLowerCase(), value);
      });
    } else if (!_.has(object, key)) {
      object[key] = cloneDeep(value);
    }
  }
});
...
```

#### <a name="apidoc.element.benchmark.filter"></a>[function <span class="apidocSignatureSpan">benchmark.</span>filter (array, callback)](#apidoc.element.benchmark.filter)
- description and source-code
```javascript
function filter(array, callback) {
  if (callback === 'successful') {
    // Callback to exclude those that are errored, unrun, or have hz of Infinity.
    callback = function(bench) {
      return bench.cycles && _.isFinite(bench.hz) && !bench.error;
    };
  }
  else if (callback === 'fastest' || callback === 'slowest') {
    // Get successful, sort by period + margin of error, and filter fastest/slowest.
    var result = filter(array, 'successful').sort(function(a, b) {
      a = a.stats; b = b.stats;
      return (a.mean + a.moe > b.mean + b.moe ? 1 : -1) * (callback === 'fastest' ? 1 : -1);
    });

    return _.filter(result, function(bench) {
      return result[0].compare(bench) == 0;
    });
  }
  return _.filter(array, callback);
}
```
- example usage
```shell
...
  'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
  console.log(String(event.target));
})
.on('complete', function() {
  console.log('Fastest is ' + this.filter('fastest').map('name'));
})
// run async
.run({ 'async': true });

// logs:
// => RegExp#test x 4,161,532 +-0.99% (59 cycles)
// => String#indexOf x 6,139,623 +-1.00% (131 cycles)
...
```

#### <a name="apidoc.element.benchmark.forEach"></a>[function <span class="apidocSignatureSpan">benchmark.</span>forEach (collection, iteratee)](#apidoc.element.benchmark.forEach)
- description and source-code
```javascript
function forEach(collection, iteratee) {
  var func = isArray(collection) ? arrayEach : baseEach;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.forOwn"></a>[function <span class="apidocSignatureSpan">benchmark.</span>forOwn (object, iteratee)](#apidoc.element.benchmark.forOwn)
- description and source-code
```javascript
function forOwn(object, iteratee) {
  return object && baseForOwn(object, getIteratee(iteratee, 3));
}
```
- example usage
```shell
...
     * @private
     * @param {Object} object The benchmark or suite instance.
     * @param {Object} [options={}] Options object.
     */
    function setOptions(object, options) {
options = object.options = _.assign({}, cloneDeep(object.constructor.options), cloneDeep(options));

_.forOwn(options, function(value, key) {
  if (value != null) {
    // Add event listeners.
    if (/^on[A-Z]/.test(key)) {
      _.each(key.split(' '), function(key) {
        object.on(key.slice(2).toLowerCase(), value);
      });
    } else if (!_.has(object, key)) {
...
```

#### <a name="apidoc.element.benchmark.formatNumber"></a>[function <span class="apidocSignatureSpan">benchmark.</span>formatNumber (number)](#apidoc.element.benchmark.formatNumber)
- description and source-code
```javascript
function formatNumber(number) {
  number = String(number).split('.');
  return number[0].replace(/(?=(?:\d{3})+$)(?!\b)/g, ',') +
    (number[1] ? '.' + number[1] : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.has"></a>[function <span class="apidocSignatureSpan">benchmark.</span>has (object, path)](#apidoc.element.benchmark.has)
- description and source-code
```javascript
function has(object, path) {
  return object != null && hasPath(object, path, baseHas);
}
```
- example usage
```shell
...
 * Gets the name of the first argument from a function's source.
 *
 * @private
 * @param {Function} fn The function.
 * @returns {string} The argument name.
 */
function getFirstArgument(fn) {
  return (!_.has(fn, 'toString') &&
    (/^[\s(]*function[^(]*\(([^\s,)]+)/.exec(fn) || 0)[1]) || '';
}

/**
 * Computes the arithmetic mean of a sample.
 *
 * @private
...
```

#### <a name="apidoc.element.benchmark.indexOf"></a>[function <span class="apidocSignatureSpan">benchmark.</span>indexOf (array, value, fromIndex)](#apidoc.element.benchmark.indexOf)
- description and source-code
```javascript
function indexOf(array, value, fromIndex) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return -1;
  }
  var index = fromIndex == null ? 0 : toInteger(fromIndex);
  if (index < 0) {
    index = nativeMax(length + index, 0);
  }
  return baseIndexOf(array, value, index);
}
```
- example usage
```shell
...
var suite = new Benchmark.Suite;

// add tests
suite.add('RegExp#test', function() {
/o/.test('Hello World!');
})
.add('String#indexOf', function() {
'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
console.log(String(event.target));
})
.on('complete', function() {
console.log('Fastest is ' + this.filter('fastest').map('name'));
...
```

#### <a name="apidoc.element.benchmark.invoke"></a>[function <span class="apidocSignatureSpan">benchmark.</span>invoke (benches, name)](#apidoc.element.benchmark.invoke)
- description and source-code
```javascript
function invoke(benches, name) {
  var args,
      bench,
      queued,
      index = -1,
      eventProps = { 'currentTarget': benches },
      options = { 'onStart': _.noop, 'onCycle': _.noop, 'onComplete': _.noop },
      result = _.toArray(benches);

<span class="apidocCodeCommentSpan">  /**
   * Invokes the method of the current object and if synchronous, fetches the next.
   */
</span>  function execute() {
    var listeners,
        async = isAsync(bench);

    if (async) {
      // Use 'getNext' as the first listener.
      bench.on('complete', getNext);
      listeners = bench.events.complete;
      listeners.splice(0, 0, listeners.pop());
    }
    // Execute method.
    result[index] = _.isFunction(bench && bench[name]) ? bench[name].apply(bench, args) : undefined;
    // If synchronous return 'true' until finished.
    return !async && getNext();
  }

  /**
   * Fetches the next bench or executes 'onComplete' callback.
   */
  function getNext(event) {
    var cycleEvent,
        last = bench,
        async = isAsync(last);

    if (async) {
      last.off('complete', getNext);
      last.emit('complete');
    }
    // Emit "cycle" event.
    eventProps.type = 'cycle';
    eventProps.target = last;
    cycleEvent = Event(eventProps);
    options.onCycle.call(benches, cycleEvent);

    // Choose next benchmark if not exiting early.
    if (!cycleEvent.aborted && raiseIndex() !== false) {
      bench = queued ? benches[0] : result[index];
      if (isAsync(bench)) {
        delay(bench, execute);
      }
      else if (async) {
        // Resume execution if previously asynchronous but now synchronous.
        while (execute()) {}
      }
      else {
        // Continue synchronous execution.
        return true;
      }
    } else {
      // Emit "complete" event.
      eventProps.type = 'complete';
      options.onComplete.call(benches, Event(eventProps));
    }
    // When used as a listener 'event.aborted = true' will cancel the rest of
    // the "complete" listeners because they were already called above and when
    // used as part of 'getNext' the 'return false' will exit the execution while-loop.
    if (event) {
      event.aborted = true;
    } else {
      return false;
    }
  }

  /**
   * Checks if invoking 'Benchmark#run' with asynchronous cycles.
   */
  function isAsync(object) {
    // Avoid using 'instanceof' here because of IE memory leak issues with host objects.
    var async = args[0] && args[0].async;
    return name == 'run' && (object instanceof Benchmark) &&
      ((async == null ? object.options.async : async) && support.timeout || object.defer);
  }

  /**
   * Raises 'index' to the next defined index or returns 'false'.
   */
  function raiseIndex() {
    index++;

    // If queued remove the previous bench.
    if (queued && index > 0) {
      shift.call(benches);
    }
    // If we reached the last index then return 'false'.
    return (queued ? benches.length : index < result.length)
      ? index
      : (index = false);
  }
  // Juggle arguments.
  if (_.isString(name)) {
    // 2 arguments (array, name).
    args = slice.call(arguments, 2);
  } else {
    // 2 arguments (array, options).
    options = _.assign(options, name);
    name = options.name;
    args = _.isArray(args = 'args' in options ? options.args : []) ? args : [args];
    queued = options.queued;
  }
  // Start iterating over the array.
  if (raiseIndex() !== false) {
    // Emit "start" event.
    bench = result[index];
    eventProps.type = 'start';
    eventProps.target = bench;
    options.onStart.call(benches, Event(eventProps));

    // End early if the suite was aborted in an "onStart" listener.
    if (name == 'run' && (benches instanceof Suite) && benches.aborted) {
      // Emit "cycle" event.
      eventProps.type = 'cycle';
      options.onCycle.call(benches, Event(eventProps));
      // Emit "complete" event.
      eventProps.type = 'complete';
      options.onComplete.call(benches, Event(eventProps));
    }
    // Start method execution.
    else {
      if (isAsync(bench)) {
        delay(bench, execute);
      } else {
        while (e ...
```
- example usage
```shell
...
* @param {Array} benches Array of benchmarks to iterate over.
* @param {Object|string} name The name of the method to invoke OR options object.
* @param {...*} [args] Arguments to invoke the method with.
* @returns {Array} A new array of values returned from each method invoked.
* @example
*
* // invoke 'reset' on all benchmarks
* Benchmark.invoke(benches, 'reset');
*
* // invoke 'emit' with arguments
* Benchmark.invoke(benches, 'emit', 'complete', listener);
*
* // invoke 'run(true)', treat benchmarks as a queue, and register invoke callbacks
* Benchmark.invoke(benches, {
*
...
```

#### <a name="apidoc.element.benchmark.join"></a>[function <span class="apidocSignatureSpan">benchmark.</span>join (object, separator1, separator2)](#apidoc.element.benchmark.join)
- description and source-code
```javascript
function join(object, separator1, separator2) {
  var result = [],
      length = (object = Object(object)).length,
      arrayLike = length === length >>> 0;

  separator2 || (separator2 = ': ');
  _.each(object, function(value, key) {
    result.push(arrayLike ? value : key + separator2 + value);
  });
  return result.join(separator1 || ',');
}
```
- example usage
```shell
...
      length = (object = Object(object)).length,
      arrayLike = length === length >>> 0;

  separator2 || (separator2 = ': ');
  _.each(object, function(value, key) {
    result.push(arrayLike ? value : key + separator2 + value);
  });
  return result.join(separator1 || ',');
}

/*------------------------------------------------------------------------*/

/**
 * Aborts all benchmarks in the suite.
 *
...
```

#### <a name="apidoc.element.benchmark.map"></a>[function <span class="apidocSignatureSpan">benchmark.</span>map (collection, iteratee)](#apidoc.element.benchmark.map)
- description and source-code
```javascript
function map(collection, iteratee) {
  var func = isArray(collection) ? arrayMap : baseMap;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
...
  'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
  console.log(String(event.target));
})
.on('complete', function() {
  console.log('Fastest is ' + this.filter('fastest').map('name'));
})
// run async
.run({ 'async': true });

// logs:
// => RegExp#test x 4,161,532 +-0.99% (59 cycles)
// => String#indexOf x 6,139,623 +-1.00% (131 cycles)
...
```

#### <a name="apidoc.element.benchmark.reduce"></a>[function <span class="apidocSignatureSpan">benchmark.</span>reduce (collection, iteratee, accumulator)](#apidoc.element.benchmark.reduce)
- description and source-code
```javascript
function reduce(collection, iteratee, accumulator) {
  var func = isArray(collection) ? arrayReduce : baseReduce,
      initAccum = arguments.length < 3;

  return func(collection, getIteratee(iteratee, 4), accumulator, initAccum, baseEach);
}
```
- example usage
```shell
...
 * Computes the arithmetic mean of a sample.
 *
 * @private
 * @param {Array} sample The sample.
 * @returns {number} The mean.
 */
function getMean(sample) {
  return (_.reduce(sample, function(sum, x) {
    return sum + x;
  }) / sample.length) || 0;
}

/**
 * Gets the source code of a function.
 *
...
```

#### <a name="apidoc.element.benchmark.runInContext"></a>[function <span class="apidocSignatureSpan">benchmark.</span>runInContext (context)](#apidoc.element.benchmark.runInContext)
- description and source-code
```javascript
function runInContext(context) {
  // Exit early if unable to acquire lodash.
  var _ = context && context._ || require('lodash') || root._;
  if (!_) {
    Benchmark.runInContext = runInContext;
    return Benchmark;
  }
  // Avoid issues with some ES3 environments that attempt to use values, named
  // after built-in constructors like 'Object', for the creation of literals.
  // ES5 clears this up by stating that literals must use built-in constructors.
  // See http://es5.github.io/#x11.1.5.
  context = context ? _.defaults(root.Object(), context, _.pick(root, contextProps)) : root;

<span class="apidocCodeCommentSpan">  /** Native constructor references. */
</span>  var Array = context.Array,
      Date = context.Date,
      Function = context.Function,
      Math = context.Math,
      Object = context.Object,
      RegExp = context.RegExp,
      String = context.String;

  /** Used for 'Array' and 'Object' method references. */
  var arrayRef = [],
      objectProto = Object.prototype;

  /** Native method shortcuts. */
  var abs = Math.abs,
      clearTimeout = context.clearTimeout,
      floor = Math.floor,
      log = Math.log,
      max = Math.max,
      min = Math.min,
      pow = Math.pow,
      push = arrayRef.push,
      setTimeout = context.setTimeout,
      shift = arrayRef.shift,
      slice = arrayRef.slice,
      sqrt = Math.sqrt,
      toString = objectProto.toString,
      unshift = arrayRef.unshift;

  /** Used to avoid inclusion in Browserified bundles. */
  var req = require;

  /** Detect DOM document object. */
  var doc = isHostType(context, 'document') && context.document;

  /** Used to access Wade Simmons' Node.js 'microtime' module. */
  var microtimeObject = req('microtime');

  /** Used to access Node.js's high resolution timer. */
  var processObject = isHostType(context, 'process') && context.process;

  /** Used to prevent a 'removeChild' memory leak in IE < 9. */
  var trash = doc && doc.createElement('div');

  /** Used to integrity check compiled tests. */
  var uid = 'uid' + _.now();

  /** Used to avoid infinite recursion when methods call each other. */
  var calledBy = {};

  /**
   * An object used to flag environments/features.
   *
   * @static
   * @memberOf Benchmark
   * @type Object
   */
  var support = {};

  (function() {

    /**
     * Detect if running in a browser environment.
     *
     * @memberOf Benchmark.support
     * @type boolean
     */
    support.browser = doc && isHostType(context, 'navigator') && !isHostType(context, 'phantom');

    /**
     * Detect if the Timers API exists.
     *
     * @memberOf Benchmark.support
     * @type boolean
     */
    support.timeout = isHostType(context, 'setTimeout') && isHostType(context, 'clearTimeout');

    /**
     * Detect if function decompilation is support.
     *
     * @name decompilation
     * @memberOf Benchmark.support
     * @type boolean
     */
    try {
      // Safari 2.x removes commas in object literals from 'Function#toString' results.
      // See http://webk.it/11609 for more details.
      // Firefox 3.6 and Opera 9.25 strip grouping parentheses from 'Function#toString' results.
      // See http://bugzil.la/559438 for more details.
      support.decompilation = Function(
        ('return (' + (function(x) { return { 'x': '' + (1 + x) + '', 'y': 0 }; }) + ')')
        // Avoid issues with code added by Istanbul.
        .replace(/__cov__[^;]+;/g, '')
      )()(0).x === '1';
    } catch(e) {
      support.decompilation = false;
    }
  }());

  /**
   * Timer object used by 'clock()' and 'Deferred#resolve'.
   *
   * @private
   * @type Object
   */
  var timer = {

    /**
     * The timer namespace object or constructor.
     *
     * @private
     * @memberOf timer
     * @type {Function|Object}
     */
    'ns': Date,

    /**
     * Starts the deferred timer.
     *
     * @private
     * @memberOf timer
     * @param {Object} deferred The deferred instance.
     */
    'start': null, // Lazy defined in 'clock()'.

    /**
     * Stops the deferred timer.
     *
     * @private
     * @memberOf timer
     * @param {Object} deferre ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.benchmark.Deferred"></a>[module benchmark.Deferred](#apidoc.module.benchmark.Deferred)

#### <a name="apidoc.element.benchmark.Deferred.Deferred"></a>[function <span class="apidocSignatureSpan">benchmark.</span>Deferred (clone)](#apidoc.element.benchmark.Deferred.Deferred)
- description and source-code
```javascript
function Deferred(clone) {
  var deferred = this;
  if (!(deferred instanceof Deferred)) {
    return new Deferred(clone);
  }
  deferred.benchmark = clone;
  clock(deferred);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.benchmark.Deferred.prototype"></a>[module benchmark.Deferred.prototype](#apidoc.module.benchmark.Deferred.prototype)

#### <a name="apidoc.element.benchmark.Deferred.prototype.resolve"></a>[function <span class="apidocSignatureSpan">benchmark.Deferred.prototype.</span>resolve ()](#apidoc.element.benchmark.Deferred.prototype.resolve)
- description and source-code
```javascript
function resolve() {
  var deferred = this,
      clone = deferred.benchmark,
      bench = clone._original;

  if (bench.aborted) {
    // cycle() -> clone cycle/complete event -> compute()'s invoked bench.run() cycle/complete.
    deferred.teardown();
    clone.running = false;
    cycle(deferred);
  }
  else if (++deferred.cycles < clone.count) {
    clone.compiled.call(deferred, context, timer);
  }
  else {
    timer.stop(deferred);
    deferred.teardown();
    delay(clone, function() { cycle(deferred); });
  }
}
```
- example usage
```shell
...
*
*   // a flag to indicate the benchmark is deferred
*   'defer': true,
*
*   // benchmark test function
*   'fn': function(deferred) {
*     // call 'Deferred#resolve' when the deferred test is finished
*     deferred.resolve();
*   }
* });
*
* // or options only
* var bench = new Benchmark({
*
*   // benchmark name
...
```



# <a name="apidoc.module.benchmark.Suite"></a>[module benchmark.Suite](#apidoc.module.benchmark.Suite)

#### <a name="apidoc.element.benchmark.Suite.Suite"></a>[function <span class="apidocSignatureSpan">benchmark.</span>Suite (name, options)](#apidoc.element.benchmark.Suite.Suite)
- description and source-code
```javascript
function Suite(name, options) {
  var suite = this;

  // Allow instance creation without the 'new' operator.
  if (!(suite instanceof Suite)) {
    return new Suite(name, options);
  }
  // Juggle arguments.
  if (_.isPlainObject(name)) {
    // 1 argument (options).
    options = name;
  } else {
    // 2 arguments (name [, options]).
    suite.name = name;
  }
  setOptions(suite, options);
}
```
- example usage
```shell
...
* @param {Object} [options={}] Options object.
* @example
*
* // basic usage (the 'new' operator is optional)
* var suite = new Benchmark.Suite;
*
* // or using a name first
* var suite = new Benchmark.Suite('foo');
*
* // or with options
* var suite = new Benchmark.Suite('foo', {
*
*   // called when the suite starts running
*   'onStart': onStart,
*
...
```



# <a name="apidoc.module.benchmark.Suite.prototype"></a>[module benchmark.Suite.prototype](#apidoc.module.benchmark.Suite.prototype)

#### <a name="apidoc.element.benchmark.Suite.prototype.abort"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>abort ()](#apidoc.element.benchmark.Suite.prototype.abort)
- description and source-code
```javascript
function abortSuite() {
  var event,
      suite = this,
      resetting = calledBy.resetSuite;

  if (suite.running) {
    event = Event('abort');
    suite.emit(event);
    if (!event.cancelled || resetting) {
      // Avoid infinite recursion.
      calledBy.abortSuite = true;
      suite.reset();
      delete calledBy.abortSuite;

      if (!resetting) {
        suite.aborted = true;
        invoke(suite, 'abort');
      }
    }
  }
  return suite;
}
```
- example usage
```shell
...
var event,
    suite = this,
    aborting = calledBy.abortSuite;

if (suite.running && !aborting) {
  // No worries, 'resetSuite()' is called within 'abortSuite()'.
  calledBy.resetSuite = true;
  suite.abort();
  delete calledBy.resetSuite;
}
// Reset if the state has changed.
else if ((suite.aborted || suite.running) &&
    (suite.emit(event = Event('reset')), !event.cancelled)) {
  suite.aborted = suite.running = false;
  if (!aborting) {
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.add"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>add (name, fn, options)](#apidoc.element.benchmark.Suite.prototype.add)
- description and source-code
```javascript
function add(name, fn, options) {
  var suite = this,
      bench = new Benchmark(name, fn, options),
      event = Event({ 'type': 'add', 'target': bench });

  if (suite.emit(event), !event.cancelled) {
    suite.push(bench);
  }
  return suite;
}
```
- example usage
```shell
...

Usage example:

'''js
var suite = new Benchmark.Suite;

// add tests
suite.add('RegExp#test', function() {
  /o/.test('Hello World!');
})
.add('String#indexOf', function() {
  'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.clone"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>clone (options)](#apidoc.element.benchmark.Suite.prototype.clone)
- description and source-code
```javascript
function cloneSuite(options) {
  var suite = this,
      result = new suite.constructor(_.assign({}, suite.options, options));

  // Copy own properties.
  _.forOwn(suite, function(value, key) {
    if (!_.has(result, key)) {
      result[key] = _.isFunction(_.get(value, 'clone'))
        ? value.clone()
        : cloneDeep(value);
    }
  });
  return result;
}
```
- example usage
```shell
...
  var suite = this,
      result = new suite.constructor(_.assign({}, suite.options, options));

  // Copy own properties.
  _.forOwn(suite, function(value, key) {
    if (!_.has(result, key)) {
      result[key] = _.isFunction(_.get(value, 'clone'))
        ? value.clone()
        : cloneDeep(value);
    }
  });
  return result;
}

/**
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.each"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>each ()](#apidoc.element.benchmark.Suite.prototype.each)
- description and source-code
```javascript
each = function () {
  var args = [this];
  push.apply(args, arguments);
  return func.apply(_, args);
}
```
- example usage
```shell
...
    function setOptions(object, options) {
options = object.options = _.assign({}, cloneDeep(object.constructor.options), cloneDeep(options));

_.forOwn(options, function(value, key) {
  if (value != null) {
    // Add event listeners.
    if (/^on[A-Z]/.test(key)) {
      _.each(key.split(' '), function(key) {
        object.on(key.slice(2).toLowerCase(), value);
      });
    } else if (!_.has(object, key)) {
      object[key] = cloneDeep(value);
    }
  }
});
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.emit"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>emit (type)](#apidoc.element.benchmark.Suite.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var listeners,
      object = this,
      event = Event(type),
      events = object.events,
      args = (arguments[0] = event, arguments);

  event.currentTarget || (event.currentTarget = object);
  event.target || (event.target = object);
  delete event.result;

  if (events && (listeners = _.has(events, event.type) && events[event.type])) {
    _.each(listeners.slice(), function(listener) {
      if ((event.result = listener.apply(object, args)) === false) {
        event.cancelled = true;
      }
      return !event.aborted;
    });
  }
  return event.result;
}
```
- example usage
```shell
...
      function getNext(event) {
var cycleEvent,
    last = bench,
    async = isAsync(last);

if (async) {
  last.off('complete', getNext);
  last.emit('complete');
}
// Emit "cycle" event.
eventProps.type = 'cycle';
eventProps.target = last;
cycleEvent = Event(eventProps);
options.onCycle.call(benches, cycleEvent);
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.filter"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>filter (callback)](#apidoc.element.benchmark.Suite.prototype.filter)
- description and source-code
```javascript
function filterSuite(callback) {
  var suite = this,
      result = new suite.constructor(suite.options);

  result.push.apply(result, filter(suite, callback));
  return result;
}
```
- example usage
```shell
...
  'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
  console.log(String(event.target));
})
.on('complete', function() {
  console.log('Fastest is ' + this.filter('fastest').map('name'));
})
// run async
.run({ 'async': true });

// logs:
// => RegExp#test x 4,161,532 +-0.99% (59 cycles)
// => String#indexOf x 6,139,623 +-1.00% (131 cycles)
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.forEach"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>forEach ()](#apidoc.element.benchmark.Suite.prototype.forEach)
- description and source-code
```javascript
forEach = function () {
  var args = [this];
  push.apply(args, arguments);
  return func.apply(_, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.Suite.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>indexOf ()](#apidoc.element.benchmark.Suite.prototype.indexOf)
- description and source-code
```javascript
indexOf = function () {
  var args = [this];
  push.apply(args, arguments);
  return func.apply(_, args);
}
```
- example usage
```shell
...
var suite = new Benchmark.Suite;

// add tests
suite.add('RegExp#test', function() {
/o/.test('Hello World!');
})
.add('String#indexOf', function() {
'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
console.log(String(event.target));
})
.on('complete', function() {
console.log('Fastest is ' + this.filter('fastest').map('name'));
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.join"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>join ()](#apidoc.element.benchmark.Suite.prototype.join)
- description and source-code
```javascript
function join() { [native code] }
```
- example usage
```shell
...
      length = (object = Object(object)).length,
      arrayLike = length === length >>> 0;

  separator2 || (separator2 = ': ');
  _.each(object, function(value, key) {
    result.push(arrayLike ? value : key + separator2 + value);
  });
  return result.join(separator1 || ',');
}

/*------------------------------------------------------------------------*/

/**
 * Aborts all benchmarks in the suite.
 *
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.listeners"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>listeners (type)](#apidoc.element.benchmark.Suite.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var object = this,
      events = object.events || (object.events = {});

  return _.has(events, type) ? events[type] : (events[type] = []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.Suite.prototype.map"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>map ()](#apidoc.element.benchmark.Suite.prototype.map)
- description and source-code
```javascript
map = function () {
  var args = [this];
  push.apply(args, arguments);
  return func.apply(_, args);
}
```
- example usage
```shell
...
  'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
  console.log(String(event.target));
})
.on('complete', function() {
  console.log('Fastest is ' + this.filter('fastest').map('name'));
})
// run async
.run({ 'async': true });

// logs:
// => RegExp#test x 4,161,532 +-0.99% (59 cycles)
// => String#indexOf x 6,139,623 +-1.00% (131 cycles)
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.off"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>off (type, listener)](#apidoc.element.benchmark.Suite.prototype.off)
- description and source-code
```javascript
function off(type, listener) {
  var object = this,
      events = object.events;

  if (!events) {
    return object;
  }
  _.each(type ? type.split(' ') : events, function(listeners, type) {
    var index;
    if (typeof listeners == 'string') {
      type = listeners;
      listeners = _.has(events, type) && events[type];
    }
    if (listeners) {
      if (listener) {
        index = _.indexOf(listeners, listener);
        if (index > -1) {
          listeners.splice(index, 1);
        }
      } else {
        listeners.length = 0;
      }
    }
  });
  return object;
}
```
- example usage
```shell
...
       */
      function getNext(event) {
var cycleEvent,
    last = bench,
    async = isAsync(last);

if (async) {
  last.off('complete', getNext);
  last.emit('complete');
}
// Emit "cycle" event.
eventProps.type = 'cycle';
eventProps.target = last;
cycleEvent = Event(eventProps);
options.onCycle.call(benches, cycleEvent);
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.on"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>on (type, listener)](#apidoc.element.benchmark.Suite.prototype.on)
- description and source-code
```javascript
function on(type, listener) {
  var object = this,
      events = object.events || (object.events = {});

  _.each(type.split(' '), function(type) {
    (_.has(events, type)
      ? events[type]
      : (events[type] = [])
    ).push(listener);
  });
  return object;
}
```
- example usage
```shell
...
suite.add('RegExp#test', function() {
  /o/.test('Hello World!');
})
.add('String#indexOf', function() {
  'Hello World!'.indexOf('o') > -1;
})
// add listeners
.on('cycle', function(event) {
  console.log(String(event.target));
})
.on('complete', function() {
  console.log('Fastest is ' + this.filter('fastest').map('name'));
})
// run async
.run({ 'async': true });
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.pop"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>pop ()](#apidoc.element.benchmark.Suite.prototype.pop)
- description and source-code
```javascript
pop = function () {
  var value = this,
      result = func.apply(value, arguments);

  if (value.length === 0) {
    delete value[0];
  }
  return result;
}
```
- example usage
```shell
...
  var listeners,
      async = isAsync(bench);

  if (async) {
    // Use 'getNext' as the first listener.
    bench.on('complete', getNext);
    listeners = bench.events.complete;
    listeners.splice(0, 0, listeners.pop());
  }
  // Execute method.
  result[index] = _.isFunction(bench && bench[name]) ? bench[name].apply(bench, args) : undefined;
  // If synchronous return 'true' until finished.
  return !async && getNext();
}
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.push"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>push ()](#apidoc.element.benchmark.Suite.prototype.push)
- description and source-code
```javascript
function push() { [native code] }
```
- example usage
```shell
...
function join(object, separator1, separator2) {
  var result = [],
      length = (object = Object(object)).length,
      arrayLike = length === length >>> 0;

  separator2 || (separator2 = ': ');
  _.each(object, function(value, key) {
    result.push(arrayLike ? value : key + separator2 + value);
  });
  return result.join(separator1 || ',');
}

/*------------------------------------------------------------------------*/

/**
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.reduce"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>reduce ()](#apidoc.element.benchmark.Suite.prototype.reduce)
- description and source-code
```javascript
reduce = function () {
  var args = [this];
  push.apply(args, arguments);
  return func.apply(_, args);
}
```
- example usage
```shell
...
 * Computes the arithmetic mean of a sample.
 *
 * @private
 * @param {Array} sample The sample.
 * @returns {number} The mean.
 */
function getMean(sample) {
  return (_.reduce(sample, function(sum, x) {
    return sum + x;
  }) / sample.length) || 0;
}

/**
 * Gets the source code of a function.
 *
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.reset"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>reset ()](#apidoc.element.benchmark.Suite.prototype.reset)
- description and source-code
```javascript
function resetSuite() {
  var event,
      suite = this,
      aborting = calledBy.abortSuite;

  if (suite.running && !aborting) {
    // No worries, 'resetSuite()' is called within 'abortSuite()'.
    calledBy.resetSuite = true;
    suite.abort();
    delete calledBy.resetSuite;
  }
  // Reset if the state has changed.
  else if ((suite.aborted || suite.running) &&
      (suite.emit(event = Event('reset')), !event.cancelled)) {
    suite.aborted = suite.running = false;
    if (!aborting) {
      invoke(suite, 'reset');
    }
  }
  return suite;
}
```
- example usage
```shell
...

      if (suite.running) {
event = Event('abort');
suite.emit(event);
if (!event.cancelled || resetting) {
  // Avoid infinite recursion.
  calledBy.abortSuite = true;
  suite.reset();
  delete calledBy.abortSuite;

  if (!resetting) {
    suite.aborted = true;
    invoke(suite, 'abort');
  }
}
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.reverse"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>reverse ()](#apidoc.element.benchmark.Suite.prototype.reverse)
- description and source-code
```javascript
function reverse() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.Suite.prototype.run"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>run (options)](#apidoc.element.benchmark.Suite.prototype.run)
- description and source-code
```javascript
function runSuite(options) {
  var suite = this;

  suite.reset();
  suite.running = true;
  options || (options = {});

  invoke(suite, {
    'name': 'run',
    'args': options,
    'queued': options.queued,
    'onStart': function(event) {
      suite.emit(event);
    },
    'onCycle': function(event) {
      var bench = event.target;
      if (bench.error) {
        suite.emit({ 'type': 'error', 'target': bench });
      }
      suite.emit(event);
      event.aborted = suite.aborted;
    },
    'onComplete': function(event) {
      suite.running = false;
      suite.emit(event);
    }
  });
  return suite;
}
```
- example usage
```shell
...
.on('cycle', function(event) {
  console.log(String(event.target));
})
.on('complete', function() {
  console.log('Fastest is ' + this.filter('fastest').map('name'));
})
// run async
.run({ 'async': true });

// logs:
// => RegExp#test x 4,161,532 +-0.99% (59 cycles)
// => String#indexOf x 6,139,623 +-1.00% (131 cycles)
// => Fastest is String#indexOf
'''
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.shift"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>shift ()](#apidoc.element.benchmark.Suite.prototype.shift)
- description and source-code
```javascript
shift = function () {
  var value = this,
      result = func.apply(value, arguments);

  if (value.length === 0) {
    delete value[0];
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.Suite.prototype.slice"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>slice ()](#apidoc.element.benchmark.Suite.prototype.slice)
- description and source-code
```javascript
function slice() { [native code] }
```
- example usage
```shell
...
  options = object.options = _.assign({}, cloneDeep(object.constructor.options), cloneDeep(options));

  _.forOwn(options, function(value, key) {
    if (value != null) {
      // Add event listeners.
      if (/^on[A-Z]/.test(key)) {
        _.each(key.split(' '), function(key) {
          object.on(key.slice(2).toLowerCase(), value);
        });
      } else if (!_.has(object, key)) {
        object[key] = cloneDeep(value);
      }
    }
  });
}
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.sort"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>sort ()](#apidoc.element.benchmark.Suite.prototype.sort)
- description and source-code
```javascript
function sort() { [native code] }
```
- example usage
```shell
...
* // or options only
* var bench = new Benchmark({
*
*   // benchmark name
*   'name': 'foo',
*
*   // benchmark test as a string
*   'fn': '[1,2,3,4].sort()'
* });
*
* // a test's 'this' binding is set to the benchmark instance
* var bench = new Benchmark('foo', function() {
*   'My name is '.concat(this.name); // "My name is foo"
* });
*/
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.splice"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>splice ()](#apidoc.element.benchmark.Suite.prototype.splice)
- description and source-code
```javascript
splice = function () {
  var value = this,
      result = func.apply(value, arguments);

  if (value.length === 0) {
    delete value[0];
  }
  return result;
}
```
- example usage
```shell
...
  var listeners,
      async = isAsync(bench);

  if (async) {
    // Use 'getNext' as the first listener.
    bench.on('complete', getNext);
    listeners = bench.events.complete;
    listeners.splice(0, 0, listeners.pop());
  }
  // Execute method.
  result[index] = _.isFunction(bench && bench[name]) ? bench[name].apply(bench, args) : undefined;
  // If synchronous return 'true' until finished.
  return !async && getNext();
}
...
```

#### <a name="apidoc.element.benchmark.Suite.prototype.unshift"></a>[function <span class="apidocSignatureSpan">benchmark.Suite.prototype.</span>unshift ()](#apidoc.element.benchmark.Suite.prototype.unshift)
- description and source-code
```javascript
unshift = function () {
  var value = this;
  unshift.apply(value, arguments);
  return value.length;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.benchmark.platform"></a>[module benchmark.platform](#apidoc.module.benchmark.platform)

#### <a name="apidoc.element.benchmark.platform.parse"></a>[function <span class="apidocSignatureSpan">benchmark.platform.</span>parse (ua)](#apidoc.element.benchmark.platform.parse)
- description and source-code
```javascript
function parse(ua) {

<span class="apidocCodeCommentSpan">  /** The environment context object. */
</span>  var context = root;

  /** Used to flag when a custom context is provided. */
  var isCustomContext = ua && typeof ua == 'object' && getClassOf(ua) != 'String';

  // Juggle arguments.
  if (isCustomContext) {
    context = ua;
    ua = null;
  }

  /** Browser navigator object. */
  var nav = context.navigator || {};

  /** Browser user agent string. */
  var userAgent = nav.userAgent || '';

  ua || (ua = userAgent);

  /** Used to flag when 'thisBinding' is the [ModuleScope]. */
  var isModuleScope = isCustomContext || thisBinding == oldRoot;

  /** Used to detect if browser is like Chrome. */
  var likeChrome = isCustomContext
    ? !!nav.likeChrome
    : /\bChrome\b/.test(ua) && !/internal|\n/i.test(toString.toString());

  /** Internal '[[Class]]' value shortcuts. */
  var objectClass = 'Object',
      airRuntimeClass = isCustomContext ? objectClass : 'ScriptBridgingProxyObject',
      enviroClass = isCustomContext ? objectClass : 'Environment',
      javaClass = (isCustomContext && context.java) ? 'JavaPackage' : getClassOf(context.java),
      phantomClass = isCustomContext ? objectClass : 'RuntimeObject';

  /** Detect Java environments. */
  var java = /\bJava/.test(javaClass) && context.java;

  /** Detect Rhino. */
  var rhino = java && getClassOf(context.environment) == enviroClass;

  /** A character to represent alpha. */
  var alpha = java ? 'a' : '\u03b1';

  /** A character to represent beta. */
  var beta = java ? 'b' : '\u03b2';

  /** Browser document object. */
  var doc = context.document || {};

  /**
   * Detect Opera browser (Presto-based).
   * http://www.howtocreate.co.uk/operaStuff/operaObject.html
   * http://dev.opera.com/articles/view/opera-mini-web-content-authoring-guidelines/#operamini
   */
  var opera = context.operamini || context.opera;

  /** Opera '[[Class]]'. */
  var operaClass = reOpera.test(operaClass = (isCustomContext && opera) ? opera['[[Class]]'] : getClassOf(opera))
    ? operaClass
    : (opera = null);

  /*------------------------------------------------------------------------*/

  /** Temporary variable used over the script's lifetime. */
  var data;

  /** The CPU architecture. */
  var arch = ua;

  /** Platform description array. */
  var description = [];

  /** Platform alpha/beta indicator. */
  var prerelease = null;

  /** A flag to indicate that environment features should be used to resolve the platform. */
  var useFeatures = ua == userAgent;

  /** The browser/environment version. */
  var version = useFeatures && opera && typeof opera.version == 'function' && opera.version();

  /** A flag to indicate if the OS ends with "/ Version" */
  var isSpecialCasedOS;

  /* Detectable layout engines (order is important). */
  var layout = getLayout([
    { 'label': 'EdgeHTML', 'pattern': 'Edge' },
    'Trident',
    { 'label': 'WebKit', 'pattern': 'AppleWebKit' },
    'iCab',
    'Presto',
    'NetFront',
    'Tasman',
    'KHTML',
    'Gecko'
  ]);

  /* Detectable browser names (order is important). */
  var name = getName([
    'Adobe AIR',
    'Arora',
    'Avant Browser',
    'Breach',
    'Camino',
    'Electron',
    'Epiphany',
    'Fennec',
    'Flock',
    'Galeon',
    'GreenBrowser',
    'iCab',
    'Iceweasel',
    'K-Meleon',
    'Konqueror',
    'Lunascape',
    'Maxthon',
    { 'label': 'Microsoft Edge', 'pattern': 'Edge' },
    'Midori',
    'Nook Browser',
    'PaleMoon',
    'PhantomJS',
    'Raven',
    'Rekonq',
    'RockMelt',
    { 'label': 'Samsung Internet', 'pattern': 'SamsungBrowser' },
    'SeaMonkey',
    { 'label': 'Silk', 'pattern': '(?:Cloud9|Silk-Accelerated)' },
    'Sleipnir',
    'SlimBrowser',
    { 'label': 'SRWare Iron', 'pattern': 'Iron' },
    'Sunrise',
    'Swiftfox',
    'Waterfox',
    'WebPositive',
    'Opera Mini',
    { 'label': 'Opera Mini', 'pattern': 'OPiOS' },
    'Opera',
    { 'label': 'Opera', 'pattern': 'OPR' },
    'Chrome',
    { 'label': 'Chrome Mobile', 'pattern': '(?:CriOS|CrMo)' },
    { 'label': 'Firefox', 'pattern': '(?:Firefox|Minefie ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.benchmark.platform.toString"></a>[function <span class="apidocSignatureSpan">benchmark.platform.</span>toString ()](#apidoc.element.benchmark.platform.toString)
- description and source-code
```javascript
function toStringPlatform() {
  return this.description || '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.benchmark.platform.os"></a>[module benchmark.platform.os](#apidoc.module.benchmark.platform.os)

#### <a name="apidoc.element.benchmark.platform.os.toString"></a>[function <span class="apidocSignatureSpan">benchmark.platform.os.</span>toString ()](#apidoc.element.benchmark.platform.os.toString)
- description and source-code
```javascript
toString = function () { return 'null'; }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
