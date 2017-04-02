# api documentation for  [serialport (v4.0.7)](https://github.com/EmergingTechnologyAdvisors/node-serialport#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-serialport.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-serialport) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-serialport.svg)](https://travis-ci.org/npmdoc/node-npmdoc-serialport)
#### Node.js package to access serial ports. Welcome your robotic javascript overlords. Better yet, program them!

[![NPM](https://nodei.co/npm/serialport.png?downloads=true)](https://www.npmjs.com/package/serialport)

[![apidoc](https://npmdoc.github.io/node-npmdoc-serialport/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-serialport_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-serialport/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-serialport/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Williams",
        "email": "voodootikigod@gmail.com",
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
            "name": "jjrosent",
            "email": "jakerosenthal@gmail.com"
        },
        {
            "name": "reconbot",
            "email": "wizard@roborooter.com"
        },
        {
            "name": "voodootikigod",
            "email": "voodootikigod@gmail.com"
        }
    ],
    "name": "serialport",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module serialport](#apidoc.module.serialport)
1.  [function <span class="apidocSignatureSpan">serialport.</span>list (callback)](#apidoc.element.serialport.list)
1.  [function <span class="apidocSignatureSpan">serialport.</span>super_ ()](#apidoc.element.serialport.super_)
1.  object <span class="apidocSignatureSpan">serialport.</span>bindings
1.  object <span class="apidocSignatureSpan">serialport.</span>parsers

#### [module serialport.bindings](#apidoc.module.serialport.bindings)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>SerialportPoller ()](#apidoc.element.serialport.bindings.SerialportPoller)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>close ()](#apidoc.element.serialport.bindings.close)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>drain ()](#apidoc.element.serialport.bindings.drain)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>flush ()](#apidoc.element.serialport.bindings.flush)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>list (callback)](#apidoc.element.serialport.bindings.list)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>open ()](#apidoc.element.serialport.bindings.open)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>set ()](#apidoc.element.serialport.bindings.set)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>update ()](#apidoc.element.serialport.bindings.update)
1.  [function <span class="apidocSignatureSpan">serialport.bindings.</span>write ()](#apidoc.element.serialport.bindings.write)
1.  object <span class="apidocSignatureSpan">serialport.bindings.</span>platformOptions

#### [module serialport.parsers](#apidoc.module.serialport.parsers)
1.  [function <span class="apidocSignatureSpan">serialport.parsers.</span>byteDelimiter (delimiter)](#apidoc.element.serialport.parsers.byteDelimiter)
1.  [function <span class="apidocSignatureSpan">serialport.parsers.</span>byteLength (length)](#apidoc.element.serialport.parsers.byteLength)
1.  [function <span class="apidocSignatureSpan">serialport.parsers.</span>raw (emitter, buffer)](#apidoc.element.serialport.parsers.raw)
1.  [function <span class="apidocSignatureSpan">serialport.parsers.</span>readline (delimiter, encoding)](#apidoc.element.serialport.parsers.readline)



# <a name="apidoc.module.serialport"></a>[module serialport](#apidoc.module.serialport)

#### <a name="apidoc.element.serialport.list"></a>[function <span class="apidocSignatureSpan">serialport.</span>list (callback)](#apidoc.element.serialport.list)
- description and source-code
```javascript
function listLinux(callback) {
  callback = callback || function(err) {
    if (err) { this.emit('error', err) }
  }.bind(this);
  return listUnix(callback);
}
```
- example usage
```shell
...
port.on('open', function() {
  // open logic
});
'''

### Listing Ports

'.list(callback)'

Retrieves a list of available serial ports with metadata.

* 'callback' is a required function that looks should look like: 'function (err, ports) { ... }'. 'ports' will be an array of objects
 with port info. Only the 'comName' is guaranteed, all the other fields undefined if unavailable. The 'comName' is either the path
 or identifier (eg 'COM1') used to open the serialport.

'''js
// example port information
...
```

#### <a name="apidoc.element.serialport.super_"></a>[function <span class="apidocSignatureSpan">serialport.</span>super_ ()](#apidoc.element.serialport.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.serialport.bindings"></a>[module serialport.bindings](#apidoc.module.serialport.bindings)

#### <a name="apidoc.element.serialport.bindings.SerialportPoller"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>SerialportPoller ()](#apidoc.element.serialport.bindings.SerialportPoller)
- description and source-code
```javascript
function SerialportPoller() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serialport.bindings.close"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>close ()](#apidoc.element.serialport.bindings.close)
- description and source-code
```javascript
function close() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serialport.bindings.drain"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>drain ()](#apidoc.element.serialport.bindings.drain)
- description and source-code
```javascript
function drain() { [native code] }
```
- example usage
```shell
...
**Example**

Writes 'data' and waits until it has finish transmitting to the target serial port before calling the callback.

'''
function writeAndDrain (data, callback) {
  sp.write(data, function () {
    sp.drain(callback);
  });
}
'''

### .close (callback)

Closes an open connection.
...
```

#### <a name="apidoc.element.serialport.bindings.flush"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>flush ()](#apidoc.element.serialport.bindings.flush)
- description and source-code
```javascript
function flush() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serialport.bindings.list"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>list (callback)](#apidoc.element.serialport.bindings.list)
- description and source-code
```javascript
function listLinux(callback) {
  callback = callback || function(err) {
    if (err) { this.emit('error', err) }
  }.bind(this);
  return listUnix(callback);
}
```
- example usage
```shell
...
port.on('open', function() {
  // open logic
});
'''

### Listing Ports

'.list(callback)'

Retrieves a list of available serial ports with metadata.

* 'callback' is a required function that looks should look like: 'function (err, ports) { ... }'. 'ports' will be an array of objects
 with port info. Only the 'comName' is guaranteed, all the other fields undefined if unavailable. The 'comName' is either the path
 or identifier (eg 'COM1') used to open the serialport.

'''js
// example port information
...
```

#### <a name="apidoc.element.serialport.bindings.open"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>open ()](#apidoc.element.serialport.bindings.open)
- description and source-code
```javascript
function open() { [native code] }
```
- example usage
```shell
...
1. Options - optional and described below.

### Opening a Port

Constructing a 'SerialPort' object will open a port on 'nextTick'. You can bind events while the port is opening but you must wait
 until it is open to 'write()' to it. (Most port functions require an open port.) You can call code when a port is opened in three
 ways.

 - The 'open' event is always emitted when the port is opened
 - The constructor's openCallback is passed to '.open()' when the 'autoOpen' option hasn't been disabled, if you have disabled it
 the callback is ignored.
 - The '.open()' function takes a callback that is called after the port is opened. This can be used if you disabled the 'autoOpen
' option or have previously closed an open port.


'''js
var SerialPort = require('serialport');
var port = new SerialPort('/dev/tty-usbserial1');
...
```

#### <a name="apidoc.element.serialport.bindings.set"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>set ()](#apidoc.element.serialport.bindings.set)
- description and source-code
```javascript
function set() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serialport.bindings.update"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>update ()](#apidoc.element.serialport.bindings.update)
- description and source-code
```javascript
function update() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serialport.bindings.write"></a>[function <span class="apidocSignatureSpan">serialport.bindings.</span>write ()](#apidoc.element.serialport.bindings.write)
- description and source-code
```javascript
function write() { [native code] }
```
- example usage
```shell
...


'''js
var SerialPort = require('serialport');
var port = new SerialPort('/dev/tty-usbserial1');

port.on('open', function() {
  port.write('main screen turn on', function(err) {
    if (err) {
      return console.log('Error on write: ', err.message);
    }
    console.log('message written');
  });
});
...
```



# <a name="apidoc.module.serialport.parsers"></a>[module serialport.parsers](#apidoc.module.serialport.parsers)

#### <a name="apidoc.element.serialport.parsers.byteDelimiter"></a>[function <span class="apidocSignatureSpan">serialport.parsers.</span>byteDelimiter (delimiter)](#apidoc.element.serialport.parsers.byteDelimiter)
- description and source-code
```javascript
byteDelimiter = function (delimiter) {
  if (Object.prototype.toString.call(delimiter) !== '[object Array]') {
    delimiter = [ delimiter ];
  }
  var buf = [];
  var nextDelimIndex = 0;
  return function(emitter, buffer) {
    for (var i = 0; i < buffer.length; i++) {
      buf[buf.length] = buffer[i];
      if (buf[buf.length - 1] === delimiter[nextDelimIndex]) {
        nextDelimIndex++;
      }
      if (nextDelimIndex === delimiter.length) {
        emitter.emit('data', buf);
        buf = [];
        nextDelimIndex = 0;
      }
    }
  };
}
```
- example usage
```shell
...
Note that the raw parser does not guarantee that all data it receives will come in a single event.

To use the byte sequence parser, you must provide a delimiter as an array of bytes:
'''js
var SerialPort = require('serialport');

var port = new SerialPort('/dev/tty-usbserial1', {
  parser: SerialPort.parsers.byteDelimiter([10,13])
});
'''

To use the byte length parser, you must provide a delimiter as a length in bytes:
'''js
var SerialPort = require('serialport');
...
```

#### <a name="apidoc.element.serialport.parsers.byteLength"></a>[function <span class="apidocSignatureSpan">serialport.parsers.</span>byteLength (length)](#apidoc.element.serialport.parsers.byteLength)
- description and source-code
```javascript
byteLength = function (length) {
  var data = new Buffer(0);
  return function(emitter, buffer) {
    data = Buffer.concat([data, buffer]);
    while (data.length >= length) {
      var out = data.slice(0, length);
      data = data.slice(length);
      emitter.emit('data', out);
    }
  };
}
```
- example usage
```shell
...
'''

To use the byte length parser, you must provide a delimiter as a length in bytes:
'''js
var SerialPort = require('serialport');

var port = new SerialPort('/dev/tty-usbserial1', {
  parser: SerialPort.parsers.byteLength(5)
});
'''

You can get updates of new data from the Serial Port as follows:

'''js
port.on('data', function (data) {
...
```

#### <a name="apidoc.element.serialport.parsers.raw"></a>[function <span class="apidocSignatureSpan">serialport.parsers.</span>raw (emitter, buffer)](#apidoc.element.serialport.parsers.raw)
- description and source-code
```javascript
raw = function (emitter, buffer) {
  emitter.emit('data', buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.serialport.parsers.readline"></a>[function <span class="apidocSignatureSpan">serialport.parsers.</span>readline (delimiter, encoding)](#apidoc.element.serialport.parsers.readline)
- description and source-code
```javascript
readline = function (delimiter, encoding) {
  if (typeof delimiter === 'undefined' || delimiter === null) { delimiter = '\r' }
  if (typeof encoding === 'undefined' || encoding === null) { encoding = 'utf8' }
  // Delimiter buffer saved in closure
  var data = '';
  return function(emitter, buffer) {
    // Collect data
    data += buffer.toString(encoding);
    // Split collected data by delimiter
    var parts = data.split(delimiter);
    data = parts.pop();
    parts.forEach(function(part) {
      emitter.emit('data', part);
    });
  };
}
```
- example usage
```shell
...

To use the readline parser, you must provide a delimiter as such:

'''js
var SerialPort = require('serialport');

var port = new SerialPort('/dev/tty-usbserial1', {
  parser: SerialPort.parsers.readline('\n')
});
'''

To use the raw parser don't specify any parser, however if you really want to you can:

'''js
var SerialPort = require('serialport');
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
