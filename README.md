# npmdoc-serialport

#### api documentation for  [serialport (v4.0.7)](https://github.com/EmergingTechnologyAdvisors/node-serialport#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-serialport.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-serialport) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-serialport.svg)](https://travis-ci.org/npmdoc/node-npmdoc-serialport)

#### Node.js package to access serial ports. Welcome your robotic javascript overlords. Better yet, program them!

[![NPM](https://nodei.co/npm/serialport.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/serialport)

- [https://npmdoc.github.io/node-npmdoc-serialport/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-serialport/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-serialport/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-serialport/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-serialport/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-serialport/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Williams",
        "url": "http://www.voodootikigod.com"
    },
    "bin": {
        "serialport-list": "./bin/serialport-list.js",
        "serialport-term": "./bin/serialport-terminal.js"
    },
    "binary": {
        "module_name": "serialport",
        "module_path": "build/{configuration}/",
        "host": "https://github.com/EmergingTechnologyAdvisors/node-serialport/releases/download/4.0.7"
    },
    "bugs": {
        "url": "https://github.com/EmergingTechnologyAdvisors/node-serialport/issues"
    },
    "bundleDependencies": [
        "node-pre-gyp"
    ],
    "dependencies": {
        "bindings": "1.2.1",
        "commander": "^2.9.0",
        "debug": "^2.3.2",
        "lie": "^3.1.0",
        "nan": "^2.4.0",
        "node-pre-gyp": "^0.6.32",
        "object.assign": "^4.0.3"
    },
    "description": "Node.js package to access serial ports. Welcome your robotic javascript overlords. Better yet, program them!",
    "devDependencies": {
        "chai": "^3.5.0",
        "chai-subset": "^1.2.2",
        "coveralls": "^2.11.9",
        "eslint-config-standard": "^5.1.0",
        "eslint-plugin-promise": "^1.1.0",
        "eslint-plugin-standard": "^1.3.2",
        "grunt": "^1.0.0",
        "grunt-mocha-test": "^0.12.7",
        "gruntify-eslint": "^2.0.0",
        "mocha": "^2.4.5",
        "node-pre-gyp-github": "^1.1.2",
        "nyc": "^6.4.4",
        "sandboxed-module": "^2.0.3",
        "sinon": "^1.17.3",
        "sinon-chai": "^2.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "421c618a8a612bd40cfa461b4a46154daf2229a5",
        "tarball": "https://registry.npmjs.org/serialport/-/serialport-4.0.7.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "4a2a3cfae7ecba4e22e9c6d4cf7dfb7ec64324f6",
    "gypfile": true,
    "homepage": "https://github.com/EmergingTechnologyAdvisors/node-serialport#readme",
    "keywords": [
        "serialport",
        "johnny-five",
        "serial port",
        "hardware",
        "iot",
        "nodebots"
    ],
    "license": "MIT",
    "main": "./lib/serialport",
    "maintainers": [
        {
            "name": "jjrosent"
        },
        {
            "name": "reconbot"
        },
        {
            "name": "voodootikigod"
        }
    ],
    "name": "serialport",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/EmergingTechnologyAdvisors/node-serialport.git"
    },
    "scripts": {
        "coverage": "nyc report --reporter=text-lcov | coveralls",
        "grunt": "grunt",
        "gyp-rebuild": "node-gyp rebuild",
        "install": "node-pre-gyp install --fallback-to-build",
        "integration": "mocha test/arduinoTest/integration.js test/integration-lite.js",
        "lint": "grunt --verbose lint",
        "rebuild-all": "npm rebuild && node-gyp rebuild",
        "stress": "mocha --no-timeouts test/arduinoTest/stress.js",
        "test": "nyc grunt --verbose test",
        "valgrind": "valgrind --leak-check=full --show-possibly-lost=no node --expose-gc --trace-gc node_modules/.bin/grunt test"
    },
    "version": "4.0.7"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
