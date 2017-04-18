# npmdoc-deployd

#### api documentation for  [deployd (v0.8.9)](https://github.com/deployd/deployd#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-deployd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-deployd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-deployd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-deployd)

#### the simplest way to build realtime APIs for web and mobile apps

[![NPM](https://nodei.co/npm/deployd.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/deployd)

- [https://npmdoc.github.io/node-npmdoc-deployd/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-deployd/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-deployd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-deployd/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-deployd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-deployd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ritchie Martori"
    },
    "bin": {
        "dpd": "./bin/dpd"
    },
    "bugs": {
        "url": "https://github.com/deployd/deployd/issues"
    },
    "dependencies": {
        "async": "^2.0.1",
        "bluebird": "^3.4.1",
        "commander": "^2.9.0",
        "cookies": "^0.6.1",
        "corser": "^2.0.1",
        "debug": "^2.2.0",
        "doh": "^0.0.4",
        "ejs": "^2.5.1",
        "filed": "^0.1.0",
        "fs-extra": "^0.30.0",
        "mkdirp": "*",
        "mongodb": "^2.2.7",
        "opener": "^1.4.1",
        "qs": "^6.2.1",
        "request": "2.74.0",
        "scrubber": "*",
        "semver": "^5.3.0",
        "send": "^0.14.1",
        "shelljs": "^0.7.3",
        "socket.io": "^1.4.8",
        "step": "^0.0.6",
        "underscore": "^1.8.3",
        "validation": "*"
    },
    "description": "the simplest way to build realtime APIs for web and mobile apps",
    "devDependencies": {
        "chai": "*",
        "less": "*",
        "mocha": "*",
        "mocha-jshint": "2.3.1",
        "mocha-phantomjs": "^4.1.0",
        "rewire": "~2.5.2",
        "sinon": "~1.17.5"
    },
    "directories": {},
    "dist": {
        "shasum": "ec7dceffe7e0f89567893dff81eb137f3d9103b7",
        "tarball": "https://registry.npmjs.org/deployd/-/deployd-0.8.9.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "47c07394127081602b9e3f7442c725f148249c82",
    "homepage": "https://github.com/deployd/deployd#readme",
    "license": "Apache-2.0",
    "main": "index",
    "maintainers": [
        {
            "name": "ritch"
        },
        {
            "name": "jeffbcross"
        },
        {
            "name": "nicolasrtt"
        }
    ],
    "name": "deployd",
    "optionalDependencies": {},
    "repository": {
        "url": "git://github.com/deployd/deployd.git"
    },
    "scripts": {
        "test": "mocha --timeout 5000 && cd test-app && node runtests.js"
    },
    "version": "0.8.9"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
