# npmdoc-benchmark

#### basic api documentation for  [benchmark (v2.1.4)](https://benchmarkjs.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-benchmark.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-benchmark) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-benchmark.svg)](https://travis-ci.org/npmdoc/node-npmdoc-benchmark)

#### A benchmarking library that supports high-resolution timers & returns statistically significant results.

[![NPM](https://nodei.co/npm/benchmark.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/benchmark)

- [https://npmdoc.github.io/node-npmdoc-benchmark/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-benchmark/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-benchmark/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-benchmark/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-benchmark/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-benchmark/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mathias Bynens",
        "url": "https://mathiasbynens.be/"
    },
    "bugs": {
        "url": "https://github.com/bestiejs/benchmark.js/issues"
    },
    "contributors": [
        {
            "name": "Mathias Bynens",
            "url": "https://mathiasbynens.be/"
        },
        {
            "name": "John-David Dalton",
            "url": "http://allyoucanleet.com/"
        },
        {
            "name": "Kit Cambridge",
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
            "name": "jdalton"
        },
        {
            "name": "mathias"
        }
    ],
    "name": "benchmark",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/bestiejs/benchmark.js.git"
    },
    "scripts": {
        "doc": "docdown benchmark.js doc/README.md style=github title=\"<a href=\\\"https://benchmarkjs.com/\\\">Benchmark.js</a> <span>v${npm_package_version}</span>\" toc=categories url=https://github.com/bestiejs/benchmark.js/blob/${npm_package_version}/benchmark.js",
        "test": "node test/test"
    },
    "version": "2.1.4",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
