# npmdoc-nodebot-workshop

#### api documentation for  [nodebot-workshop (v3.2.0)](https://github.com/tableflip/nodebot-workshop#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-nodebot-workshop.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nodebot-workshop) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nodebot-workshop.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nodebot-workshop)

#### A nodeschool workshop that will make your Ardunio alive with johnny-five

[![NPM](https://nodei.co/npm/nodebot-workshop.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/nodebot-workshop)

- [https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "nodebot-workshop": "./nodebot-workshop.js"
    },
    "bugs": {
        "url": "https://github.com/tableflip/nodebot-workshop/issues"
    },
    "contributors": [
        {
            "name": "olizilla"
        },
        {
            "name": "_alanshaw"
        },
        {
            "name": "achingbrain"
        },
        {
            "name": "gorhgorh"
        },
        {
            "name": "n0bisuke"
        }
    ],
    "dependencies": {
        "async": "^2.0.1",
        "dnode": "^1.2.0",
        "ioboard": "^3.0",
        "johnny-five": "^0.10.0",
        "node-notifier": "^4.3.1",
        "proxyquire": "^1.0.0",
        "sinon": "^1.9",
        "workshopper-adventure": "4.6.1",
        "workshopper-exercise": "^2.5.3"
    },
    "description": "A nodeschool workshop that will make your Ardunio alive with johnny-five",
    "devDependencies": {
        "gulp": "^3.9.1",
        "gulp-jshint": "^2.0.0",
        "gulp-shell": "^0.5.1",
        "jshint": "^2.8.0",
        "jshint-stylish": "^2.1.0",
        "pre-commit": "^1.1.2"
    },
    "directories": {},
    "dist": {
        "shasum": "4d0093840928bd4be9988f497d65c40053b9aba2",
        "tarball": "https://registry.npmjs.org/nodebot-workshop/-/nodebot-workshop-3.2.0.tgz"
    },
    "gitHead": "a1c7c887f6a85631ab4d3c5305a5052f49b9b790",
    "homepage": "https://github.com/tableflip/nodebot-workshop#readme",
    "keywords": [
        "nodeschool",
        "johnny-five",
        "nodebot",
        "arduino",
        "workshop",
        "workshopper",
        "life is not a malfuction"
    ],
    "license": "BSD-2-Clause",
    "main": "nodebot-workshop.js",
    "maintainers": [
        {
            "name": "olizilla"
        },
        {
            "name": "alanshaw"
        },
        {
            "name": "achingbrain"
        }
    ],
    "name": "nodebot-workshop",
    "optionalDependencies": {
        "node-notifier": "^4.3.1"
    },
    "pre-commit": [
        "lint",
        "test"
    ],
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tableflip/nodebot-workshop.git"
    },
    "scripts": {
        "lint": "jshint exercises tests stubs *.js",
        "start": "./nodebot-workshop.js",
        "test": "gulp"
    },
    "version": "3.2.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
