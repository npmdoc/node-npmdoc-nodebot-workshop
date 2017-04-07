# api documentation for  [nodebot-workshop (v3.2.0)](https://github.com/tableflip/nodebot-workshop#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-nodebot-workshop.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nodebot-workshop) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nodebot-workshop.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nodebot-workshop)
#### A nodeschool workshop that will make your Ardunio alive with johnny-five

[![NPM](https://nodei.co/npm/nodebot-workshop.png?downloads=true)](https://www.npmjs.com/package/nodebot-workshop)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nodebot-workshop_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nodebot-workshop/build/apidoc.html)

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
            "name": "olizilla",
            "email": "oli@zilla.org.uk"
        },
        {
            "name": "alanshaw",
            "email": "alan138@gmail.com"
        },
        {
            "name": "achingbrain",
            "email": "alex@achingbrain.net"
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
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nodebot-workshop](#apidoc.module.nodebot-workshop)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.</span>serialport_stub {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub)
1.  object <span class="apidocSignatureSpan">nodebot-workshop.</span>five
1.  object <span class="apidocSignatureSpan">nodebot-workshop.</span>io_stub

#### [module nodebot-workshop.five](#apidoc.module.nodebot-workshop.five)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Accelerometer (opts)](#apidoc.element.nodebot-workshop.five.Accelerometer)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Altimeter (opts)](#apidoc.element.nodebot-workshop.five.Altimeter)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Analog (opts)](#apidoc.element.nodebot-workshop.five.Analog)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Animation (target)](#apidoc.element.nodebot-workshop.five.Animation)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Barometer (opts)](#apidoc.element.nodebot-workshop.five.Barometer)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Board (opts)](#apidoc.element.nodebot-workshop.five.Board)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Boards (opts)](#apidoc.element.nodebot-workshop.five.Boards)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Button (opts)](#apidoc.element.nodebot-workshop.five.Button)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Buttons (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Buttons)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Collection (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Collection)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Color (opts)](#apidoc.element.nodebot-workshop.five.Color)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Compass (opts)](#apidoc.element.nodebot-workshop.five.Compass)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Digital (opts)](#apidoc.element.nodebot-workshop.five.Digital)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>ESC (opts)](#apidoc.element.nodebot-workshop.five.ESC)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>ESCs (numsOrObjects)](#apidoc.element.nodebot-workshop.five.ESCs)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Expander (opts)](#apidoc.element.nodebot-workshop.five.Expander)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>GPS (opts)](#apidoc.element.nodebot-workshop.five.GPS)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Gripper (opts)](#apidoc.element.nodebot-workshop.five.Gripper)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Gyro (opts)](#apidoc.element.nodebot-workshop.five.Gyro)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Hygrometer (opts)](#apidoc.element.nodebot-workshop.five.Hygrometer)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>IMU (opts)](#apidoc.element.nodebot-workshop.five.IMU)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>IR ()](#apidoc.element.nodebot-workshop.five.IR)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Joystick (opts)](#apidoc.element.nodebot-workshop.five.Joystick)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Keypad (opts)](#apidoc.element.nodebot-workshop.five.Keypad)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>LCD (opts)](#apidoc.element.nodebot-workshop.five.LCD)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Led (opts)](#apidoc.element.nodebot-workshop.five.Led)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>LedControl (opts)](#apidoc.element.nodebot-workshop.five.LedControl)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Leds (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Leds)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Light (opts)](#apidoc.element.nodebot-workshop.five.Light)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Luxmeter (options)](#apidoc.element.nodebot-workshop.five.Luxmeter)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Magnetometer (options)](#apidoc.element.nodebot-workshop.five.Magnetometer)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Motion (opts)](#apidoc.element.nodebot-workshop.five.Motion)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Motor (opts)](#apidoc.element.nodebot-workshop.five.Motor)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Motors (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Motors)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Multi (opts)](#apidoc.element.nodebot-workshop.five.Multi)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Nunchuk (opts)](#apidoc.element.nodebot-workshop.five.Nunchuk)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Piezo (opts)](#apidoc.element.nodebot-workshop.five.Piezo)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Pin (opts)](#apidoc.element.nodebot-workshop.five.Pin)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Ping (opts)](#apidoc.element.nodebot-workshop.five.Ping)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Pins (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Pins)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Proximity (opts)](#apidoc.element.nodebot-workshop.five.Proximity)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Relay (opts)](#apidoc.element.nodebot-workshop.five.Relay)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Relays (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Relays)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Repl (opts)](#apidoc.element.nodebot-workshop.five.Repl)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Sensor (opts)](#apidoc.element.nodebot-workshop.five.Sensor)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Sensors (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Sensors)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Servo (opts)](#apidoc.element.nodebot-workshop.five.Servo)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Servos (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Servos)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>ShiftRegister (opts)](#apidoc.element.nodebot-workshop.five.ShiftRegister)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Sonar (opts)](#apidoc.element.nodebot-workshop.five.Sonar)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Stepper (opts)](#apidoc.element.nodebot-workshop.five.Stepper)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Switch (opts)](#apidoc.element.nodebot-workshop.five.Switch)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Switches (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Switches)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Temperature (opts)](#apidoc.element.nodebot-workshop.five.Temperature)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Thermometer (opts)](#apidoc.element.nodebot-workshop.five.Thermometer)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Touchpad (opts)](#apidoc.element.nodebot-workshop.five.Touchpad)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Wii (opts)](#apidoc.element.nodebot-workshop.five.Wii)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>spyOn ()](#apidoc.element.nodebot-workshop.five.spyOn)
1.  object <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Fn
1.  object <span class="apidocSignatureSpan">nodebot-workshop.five.</span>stubs

#### [module nodebot-workshop.io_stub](#apidoc.module.nodebot-workshop.io_stub)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.io_stub.</span>Board (port, callback)](#apidoc.element.nodebot-workshop.io_stub.Board)

#### [module nodebot-workshop.serialport_stub](#apidoc.module.nodebot-workshop.serialport_stub)
1.  boolean <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>called
1.  boolean <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledOnce
1.  boolean <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledThrice
1.  boolean <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledTwice
1.  boolean <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>isSinonProxy
1.  boolean <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>notCalled
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.</span>serialport_stub {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub.serialport_stub)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledOn ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledOn)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWith ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWith)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWithExactly ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithExactly)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWithMatch ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithMatch)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWithNew ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithNew)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysReturned ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysReturned)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysThrew ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysThrew)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArg ()](#apidoc.element.nodebot-workshop.serialport_stub.callArg)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArgOn ()](#apidoc.element.nodebot-workshop.serialport_stub.callArgOn)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArgOnWith ()](#apidoc.element.nodebot-workshop.serialport_stub.callArgOnWith)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArgWith ()](#apidoc.element.nodebot-workshop.serialport_stub.callArgWith)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledAfter (spyFn)](#apidoc.element.nodebot-workshop.serialport_stub.calledAfter)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledBefore (spyFn)](#apidoc.element.nodebot-workshop.serialport_stub.calledBefore)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledOn ()](#apidoc.element.nodebot-workshop.serialport_stub.calledOn)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWith ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWith)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWithExactly ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWithExactly)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWithMatch ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWithMatch)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWithNew ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWithNew)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>getCall (i)](#apidoc.element.nodebot-workshop.serialport_stub.getCall)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>getCalls ()](#apidoc.element.nodebot-workshop.serialport_stub.getCalls)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>instantiateFake (func, spyLength)](#apidoc.element.nodebot-workshop.serialport_stub.instantiateFake)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>invoke (func, thisValue, args)](#apidoc.element.nodebot-workshop.serialport_stub.invoke)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>invokeCallback ()](#apidoc.element.nodebot-workshop.serialport_stub.invokeCallback)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>list {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub.list)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>matches (args, strict)](#apidoc.element.nodebot-workshop.serialport_stub.matches)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>named (name)](#apidoc.element.nodebot-workshop.serialport_stub.named)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>neverCalledWith ()](#apidoc.element.nodebot-workshop.serialport_stub.neverCalledWith)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>neverCalledWithMatch ()](#apidoc.element.nodebot-workshop.serialport_stub.neverCalledWithMatch)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>printf (format)](#apidoc.element.nodebot-workshop.serialport_stub.printf)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>reset ()](#apidoc.element.nodebot-workshop.serialport_stub.reset)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>returned ()](#apidoc.element.nodebot-workshop.serialport_stub.returned)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>spyCall {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub.spyCall)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>threw ()](#apidoc.element.nodebot-workshop.serialport_stub.threw)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>toString ()](#apidoc.element.nodebot-workshop.serialport_stub.toString)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>withArgs ()](#apidoc.element.nodebot-workshop.serialport_stub.withArgs)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yield ()](#apidoc.element.nodebot-workshop.serialport_stub.yield)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yieldOn ()](#apidoc.element.nodebot-workshop.serialport_stub.yieldOn)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yieldTo ()](#apidoc.element.nodebot-workshop.serialport_stub.yieldTo)
1.  [function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yieldToOn ()](#apidoc.element.nodebot-workshop.serialport_stub.yieldToOn)
1.  number <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callCount
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>args
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callIds
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>exceptions
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>firstCall
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>formatters
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>lastCall
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>returnValues
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>secondCall
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>stacks
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>thirdCall
1.  object <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>thisValues
1.  string <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>displayName
1.  string <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>id



# <a name="apidoc.module.nodebot-workshop"></a>[module nodebot-workshop](#apidoc.module.nodebot-workshop)

#### <a name="apidoc.element.nodebot-workshop.serialport_stub"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.</span>serialport_stub {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub)
- description and source-code
```javascript
SerialPort
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodebot-workshop.five"></a>[module nodebot-workshop.five](#apidoc.module.nodebot-workshop.five)

#### <a name="apidoc.element.nodebot-workshop.five.Accelerometer"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Accelerometer (opts)](#apidoc.element.nodebot-workshop.five.Accelerometer)
- description and source-code
```javascript
function Accelerometer(opts) {
  if (!(this instanceof Accelerometer)) {
    return new Accelerometer(opts);
  }

  var controller = null;

  var state = {
    enabled: true,
    x: {
      value: 0,
      previous: 0,
      stash: [],
      orientation: null,
      inclination: null,
      acceleration: null,
      calibration: []
    },
    y: {
      value: 0,
      previous: 0,
      stash: [],
      orientation: null,
      inclination: null,
      acceleration: null,
      calibration: []
    },
    z: {
      value: 0,
      previous: 0,
      stash: [],
      orientation: null,
      inclination: null,
      acceleration: null,
      calibration: []
    }
  };

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.ANALOG;
  }

  Board.Controller.call(this, controller, opts);

  if (!this.toGravity) {
    this.toGravity = opts.toGravity || function(raw) {
      return raw;
    };
  }

  if (!this.enabledChanged) {
    this.enabledChanged = function() {};
  }

  priv.set(this, state);

<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      var isChange = false;

      if (!state.enabled) {
        return;
      }

      Object.keys(data).forEach(function(axis) {
        var value = data[axis];
        var sensor = state[axis];

        if (opts.autoCalibrate && sensor.calibration.length < calibrationSize) {
          var axisIndex = axes.indexOf(axis);
          sensor.calibration.push(value);

          if (!Array.isArray(state.zeroV)) {
            state.zeroV = [];
          }

          state.zeroV[axisIndex] = sum(sensor.calibration) / sensor.calibration.length;
          if (axis === aZ) {
            state.zeroV[axisIndex] -= state.sensitivity;
          }
        }

        // The first run needs to prime the "stash"
        // of data values.
        if (sensor.stash.length === 0) {
          for (var i = 0; i < 5; i++) {
            sensor.stash[i] = value;
          }
        }

        sensor.previous = sensor.value;
        sensor.stash.shift();
        sensor.stash.push(value);

        sensor.value = (sum(sensor.stash) / 5) | 0;

        if (this.acceleration !== sensor.acceleration) {
          sensor.acceleration = this.acceleration;
          isChange = true;
          this.emit("acceleration", sensor.acceleration);
        }

        if (this.orientation !== sensor.orientation) {
          sensor.orientation = this.orientation;
          isChange = true;
          this.emit("orientation", sensor.orientation);
        }

        if (this.inclination !== sensor.inclination) {
          sensor.inclination = this.inclination;
          isChange = true;
          this.emit("inclination", sensor.inclination);
        }
      }, this);

      this.emit("data", {
        x: state.x.value,
        y: state.y.value,
        z: state.z.value
      });

      if (isChange) {
        this.emit("change", {
          x: this.x,
          y: this.y,
          z: this.z
        });
      }
    }.bind(this));
  }

  Object.defineProperties(this, {
    hasAxis: {
      writable: true,
      value: function(axis) {
        /* istanbul ignore next */
        return state[axis] ? state[axis].stash.length > 0 : false;
      }
    },
    enable: {
      value: function() {
        state.enabled = true;
        this.enabledChanged(true);
        return this;
      }
    },
    disable: {
      value: function() {
        state.enabled = false;
        this.enabledChanged(false);
        return this;
      }
    },
    zeroV: {
      get: function() {
        return state.zeroV;
      }
    },
    /**
     * [read-only] Calculated pitch value
     * @property pitch
     * @type Number
     */
    pitch: {
      get: function() {
        var x = this.x;
        var y = this.y;
        var z = this.z;
        var r ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Altimeter"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Altimeter (opts)](#apidoc.element.nodebot-workshop.five.Altimeter)
- description and source-code
```javascript
function Altimeter(opts) {
  if (!(this instanceof Altimeter)) {
    return new Altimeter(opts);
  }

  var controller = null;
  var freq;
  var last = null;
  var raw = null;
  var state = {};

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  freq = opts.freq || 25;


  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    throw new Error("Altimeter expects a valid controller");
  }

  priv.set(this, state);

  Board.Controller.call(this, controller, opts);

  if (!this.toMeters) {
    this.toMeters = opts.toMeters || function(x) {
      return x;
    };
  }

  var descriptors = {
    meters: {
      get: function() {
        return this.toMeters(raw);
      }
    },
    feet: {
      get: function() {
        return Fn.toFixed(this.meters * 3.28084, 2);
      }
    }
  };
  // Convenience aliases
  descriptors.m = descriptors.meters;
  descriptors.ft = descriptors.feet;

  Object.defineProperties(this, descriptors);


<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  setInterval(function() {
    if (raw == null) {
      return;
    }

    var data = {};
    data.m = data.meters = this.meters;
    data.ft = data.feet = this.feet;

    this.emit("data", data);

    /* istanbul ignore else */
    if (this.meters !== last) {
      last = this.meters;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Analog"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Analog (opts)](#apidoc.element.nodebot-workshop.five.Analog)
- description and source-code
```javascript
Analog = function (opts) {
  return new module.exports.Sensor(opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Animation"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Animation (target)](#apidoc.element.nodebot-workshop.five.Animation)
- description and source-code
```javascript
function Animation(target) {

  // Necessary to avoid loading temporal unless necessary
  if (!temporal) {
    temporal = require("temporal");
  }

  if (!(this instanceof Animation)) {
    return new Animation(target);
  }

  Animation.Segment.call(this);

  this.defaultTarget = target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Barometer"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Barometer (opts)](#apidoc.element.nodebot-workshop.five.Barometer)
- description and source-code
```javascript
function Barometer(opts) {
  if (!(this instanceof Barometer)) {
    return new Barometer(opts);
  }

  var controller = null;
  var last = null;
  var raw = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var freq = opts.freq || 25;

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    // controller = Controllers["ANALOG"];
    throw new Error("Missing Barometer controller");
  }

  Board.Controller.call(this, controller, opts);

  if (!this.toPressure) {
    this.toPressure = opts.toPressure || function(raw) {
      return raw;
    };
  }

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  Object.defineProperties(this, {
    pressure: {
      get: function() {
        return toFixed(this.toPressure(raw), 4);
      }
    }
  });

  setInterval(function() {
    if (raw === null) {
      return;
    }

    var data = {
      pressure: this.pressure
    };

    this.emit("data", data);

    if (this.pressure !== last) {
      last = this.pressure;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Board"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Board (opts)](#apidoc.element.nodebot-workshop.five.Board)
- description and source-code
```javascript
function Board(opts) {

  if (!(this instanceof Board)) {
    return new Board(opts);
  }

  // Ensure opts is an object
  opts = opts || {};

  // Used to define the board instance's own
  // properties in the REPL's scope.
  var replContext = {};

  // It's feasible that an IO-Plugin may emit
  // "connect" and "ready" events out of order.
  // This is used to enforce the order, by
  // postponing the "ready" event if the IO-Plugin
  // hasn't emitted a "connect" event. Once
  // the "connect" event is emitted, the
  // postponement is lifted and the board may
  // proceed with emitting the events in the
  // correct order.
  var isPostponed = false;

  // Initialize this Board instance with
  // param specified properties.
  Object.assign(this, opts);

  this.timer = null;

  this.isConnected = false;

  // Easily track state of hardware
  this.isReady = false;

  // Initialize instance property to reference io board
  this.io = this.io || null;

  // Registry of components
  this.register = [];

  // Pins, Addr (alt Pin name), Addresses
  this.occupied = [];

  // Registry of drivers by address (i.e. I2C Controllers)
  this.Drivers = {};

  // Identify for connect hardware cache
  if (!this.id) {
    this.id = Fn.uid();
  }

  // If no debug flag, default to true
  if (typeof this.debug === UNDEFINED) {
    this.debug = true;
  }

  // If no repl flag, default to true
  if (typeof this.repl === UNDEFINED) {
    this.repl = true;
  }

  // If no sigint flag, default to true
  if (typeof this.sigint === UNDEFINED) {
    this.sigint = true;
  }

  // Specially processed pin capabilities object
  // assigned when physical board has reported
  // "ready" via Firmata or IO-Plugin.
  this.pins = null;

  // Create a Repl instance and store as
  // instance property of this io/board.
  // This will reduce the amount of boilerplate
  // code required to _always_ have a Repl
  // session available.
  //
  // If a sesssion exists, use it
  // (instead of creating a new session)
  //
<span class="apidocCodeCommentSpan">  /* istanbul ignore if */
</span>  if (this.repl) {
    /* istanbul ignore if */
    if (Repl.ref) {
      /* istanbul ignore next */
      replContext[this.id] = this;
      /* istanbul ignore next */
      Repl.ref.on("ready", function() {
        /* istanbul ignore next */
        Repl.ref.inject(replContext);
      });
      /* istanbul ignore next */
      this.repl = Repl.ref;
    } else {
      replContext[this.id] = replContext.board = this;
      this.repl = new Repl(replContext);
    }
  }

  if (opts.io) {
    // If you already have a connected io instance
    this.io = opts.io;
    this.isReady = opts.io.isReady;
    this.transport = this.io.transport || null;
    this.port = this.io.name;
    this.pins = Board.Pins(this);
  } else {

    if (this.port && opts.port) {
      Serial.connect.call(this, this.port, finalizeAndBroadcast);
    } else {
      Serial.detect.call(this, function(path) {
        Serial.connect.call(this, path, finalizeAndBroadcast);
      });
    }
  }

  // Either an IO instance was provided or isOnBoard is true
  if (!opts.port && this.io !== null) {
    /* istanbul ignore next */
    this.info("Device(s)", chalk.grey(this.io.name || "unknown"));

    ["connect", "ready"].forEach(function(type) {
      this.io.once(type, function() {
        // Since connection and readiness happen asynchronously,
        // it's actually possible for Johnny-Five to receive the
        // events out of order and that should be ok.
        if (type === "ready" && !this.isConnected) {
          isPostponed = true;
        } else {
          // Will emit the "connect" and "ready" events
          // if received in order. If out of order, this
          // will only emit the "connect" event. The
          // "ready" event will be handled in the next
          // condition's consequent.
          finalizeAndBroadcast.call(this, null, type, this.io);
        }

        if (type === "connect" && isPostponed) {
          finalizeAndBroadcast.call(this, null, "ready", this.io);
        }
      }.bind(this));

      if (this.io.isReady) { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Boards"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Boards (opts)](#apidoc.element.nodebot-workshop.five.Boards)
- description and source-code
```javascript
function Boards(opts) {
  if (!(this instanceof Boards)) {
    return new Boards(opts);
  }

  var ports;

  // new Boards([ ...Array of board opts ])
  if (Array.isArray(opts)) {
    ports = opts.slice();
    opts = {
      ports: ports,
    };
  }

  // new Boards({ ports: [ ...Array of board opts ], .... })
<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (!Array.isArray(opts) && typeof opts === "object" && opts.ports !== undefined) {
    ports = opts.ports;
  }

  // new Boards(non-Array?)
  // new Boards({ ports: non-Array? })
  /* istanbul ignore if */
  if (!Array.isArray(ports)) {
    throw new Error("Expected ports to be an array");
  }

  if (typeof opts.debug === UNDEFINED) {
    opts.debug = true;
  }

  if (typeof opts.repl === UNDEFINED) {
    opts.repl = true;
  }

  var initialized = {};
  var noRepl = ports.some(function(port) { return port.repl === false; });
  var noDebug = ports.some(function(port) { return port.debug === false; });

  this.length = ports.length;
  this.debug = opts.debug;
  this.repl = opts.repl;

  // If any of the port definitions have
  // explicitly shut off debug output, bubble up
  // to the Boards instance
  /* istanbul ignore else */
  if (noDebug) {
    this.debug = false;
  }

  // If any of the port definitions have
  // explicitly shut off the repl, bubble up
  // to the Boards instance
  /* istanbul ignore else */
  if (noRepl) {
    this.repl = false;
  }

  var expecteds = ports.map(function(port, index) {
    var portOpts;

    if (typeof port === "string") {
      portOpts = {};

      // If the string matches a known valid port
      // name pattern, then assume this is what
      // the user code intended.
      if (rport.test(port)) {
        portOpts.port = port;
      } else {
        // Otherwise they expect Johnny-Five to figure
        // out what ports to use and intended this
        // value to be used an id
        portOpts.id = port;
      }
    } else {
      portOpts = port;
    }

    // Shut off per-board repl instance creation
    portOpts.repl = false;

    this[index] = initialized[portOpts.id] = new Board(portOpts);

    // "error" event is not async, register immediately
    this[index].on("error", function(error) {
      this.emit("error", error);
    }.bind(this));

    return new Promise(function(resolve) {
      this[index].on("ready", function() {
        resolve(initialized[portOpts.id]);
      });
    }.bind(this));
  }, this);

  Promise.all(expecteds).then(function(boards) {
    Object.assign(this, boards);

    this.each(function(board) {
      board.info("Board ID: ", chalk.green(board.id));
    });

    // If the Boards instance requires a REPL,
    // make sure it's created before calling "ready"
    if (this.repl) {
      this.repl = new Repl(
        Object.assign({}, initialized, {
          board: this
        })
      );
      this.repl.initialize(function() {
        this.emit("ready", initialized);
      }.bind(this));
    } else {
      // Otherwise, call ready immediately
      this.emit("ready", initialized);
    }
  }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Button"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Button (opts)](#apidoc.element.nodebot-workshop.five.Button)
- description and source-code
```javascript
function Button(opts) {
  if (!(this instanceof Button)) {
    return new Button(opts);
  }

  var pinValue;
  var raw;
  var invert = false;
  var downValue = 1;
  var upValue = 0;
  var controller = null;
  var state = {
    interval: null,
    last: null
  };

  // Create a debounce boundary on event triggers
  // this avoids button events firing on
  // press noise and false positives
  var trigger = Fn.debounce(function(key) {
    aliases[key].forEach(function(type) {
      this.emit(type);
    }, this);
  }, 7);

  pinValue = typeof opts === "object" ? opts.pin : opts;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  opts.pinValue = pinValue;

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.DEFAULT;
  }

  Board.Controller.call(this, controller, opts);

  // 'holdtime' is used by an interval to determine
  // if the button has been released within a specified
  // time frame, in milliseconds.
  this.holdtime = opts.holdtime || 500;

  // 'opts.isPullup' is included as part of an effort to
  // phase out "isFoo" options properties
  this.pullup = opts.pullup || opts.isPullup || false;

  this.pulldown = opts.pulldown || opts.isPulldown || false;

  // Turns out some button circuits will send
  // 0 for up and 1 for down, and some the inverse,
  // so we can invert our function with this option.
  // Default to invert in pullup mode, but use opts.invert
  // if explicitly defined (even if false)
  invert = typeof opts.invert !== "undefined" ?
    opts.invert : (this.pullup || false);

  if (invert) {
    downValue = downValue ^ 1;
    upValue = upValue ^ 1;
  }

  state.last = upValue;

  // Create a "state" entry for privately
  // storing the state of the button
  priv.set(this, state);

  Object.defineProperties(this, {
    value: {
      get: function() {
        return Number(this.isDown);
      }
    },
    invert: {
      get: function() {
        return invert;
      },
      set: function(value) {
        invert = value;
        downValue = invert ? 0 : 1;
        upValue = invert ? 1 : 0;

        state.last = upValue;
      }
    },
    downValue: {
      get: function() {
        return downValue;
      },
      set: function(value) {
        downValue = value;
        upValue = value ^ 1;
        invert = value ? true : false;

        state.last = upValue;
      }
    },
    upValue: {
      get: function() {
        return upValue;
      },
      set: function(value) {
        upValue = value;
        downValue = value ^ 1;
        invert = value ? true : false;

        state.last = downValue;
      }
    },
    isDown: {
      get: function() {
        return this.toBoolean(raw);
      }
    }
  });

<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      // Update the raw data value, which
      // is used by isDown = toBoolean()
      raw = data;

      if (!this.isDown) {
        /* istanbul ignore else */
        if (state.interval) {
          clearInterval(state.interval);
        }
        trigger.call(this, "up");
      }

      if (this.isDown) {
        trigger.call(this, "down");

        state.interval = setInterval(function() {
          /* istanbul ignore else */
          if (this.isDown) {
            this.emit("hold");
          }
        }.bind(this), this.holdtime);
      }

      state.last = data;
    }.bind(this));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Buttons"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Buttons (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Buttons)
- description and source-code
```javascript
function Buttons(numsOrObjects) {
  if (!(this instanceof Buttons)) {
    return new Buttons(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Button
  });

  Collection.Emitter.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Collection"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Collection (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Collection)
- description and source-code
```javascript
function Collection(numsOrObjects) {
  var Type = this.type;
  var initObjects = [];

  this.length = 0;

  if (Array.isArray(numsOrObjects)) {
    initObjects = numsOrObjects;
  } else {
    // Initialize with a Shared Properties object
<span class="apidocCodeCommentSpan">    /* istanbul ignore else */
</span>    if (Array.isArray(numsOrObjects.pins)) {
      var keys = Object.keys(numsOrObjects).filter(function(key) {
        return key !== "pins";
      });
      initObjects = numsOrObjects.pins.map(function(pin) {
        var obj = {};

        if (Array.isArray(pin)) {
          obj.pins = pin;
        } else {
          obj.pin = pin;
        }

        return keys.reduce(function(accum, key) {
          accum[key] = numsOrObjects[key];
          return accum;
        }, obj);
      });
    }
  }

  /* istanbul ignore else */
  if (initObjects.length) {
    while (initObjects.length) {
      var numOrObject = initObjects.shift();

      // When a Type exists, respect it!
      if (typeof Type === "function") {
        if (!(numOrObject instanceof Type || numOrObject instanceof this.constructor)) {
          numOrObject = new Type(numOrObject);
        }
      }

      this.add(numOrObject);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Color"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Color (opts)](#apidoc.element.nodebot-workshop.five.Color)
- description and source-code
```javascript
function Color(opts) {

  if (!(this instanceof Color)) {
    return new Color(opts);
  }

  var controller = null;
  var state = {};
  var freq = opts.freq || 25;
  var raw = 0;
  var last = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (typeof opts.controller === "string") {
    controller = Controllers[opts.controller];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    throw new Error("Color expects a valid controller");
  }

  priv.set(this, state);

  Board.Controller.call(this, controller, opts);

  if (!this.toRGB) {
    this.toRGB = opts.toRGB || function(x) {
      return x;
    };
  }

  Object.defineProperties(this, {
    value: {
      get: function() {
        return raw;
      }
    },
    rgb: {
      get: function() {
        return this.toRGB(raw).reduce(function(accum, value, index) {
          accum[colorNames[index]] = value;
          return accum;
        }, {});
      }
    }
  });

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  setInterval(function() {
    if (raw === undefined) {
      return;
    }

    var data = {
      rgb: this.rgb,
    };

    this.emit("data", data);

    if (raw !== last) {
      last = raw;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Compass"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Compass (opts)](#apidoc.element.nodebot-workshop.five.Compass)
- description and source-code
```javascript
function Compass(opts) {

  if (!(this instanceof Compass)) {
    return new Compass(opts);
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var freq = opts.freq || 25;
  var controller = null;
  var raw = {
    x: null,
    y: null,
    z: null,
  };
  var state = {
    x: 0,
    y: 0,
    z: 0,
    scale: 0,
    register: 0,
    heading: 0
  };

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    throw new Error("Compass expects a valid controller");
  }

  Board.Controller.call(this, controller, opts);

  if (!this.toScaledHeading) {
    this.toScaledHeading = opts.toScaledHeading || function(raw) {
      return raw;
    };
  }

  priv.set(this, state);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  setInterval(function() {
    if (raw.x === null) {
      return;
    }
    var isChange = false;

    state.x = raw.x;
    state.y = raw.y;
    state.z = raw.z;

    var heading = this.heading;

    if (heading !== state.heading) {
      state.heading = heading;
      isChange = true;
    }

    this.emit("data", {
      heading: state.heading
    });

    if (isChange) {
      this.emit("change", {
        heading: state.heading
      });
    }
  }.bind(this), freq);

  Object.defineProperties(this, {
<span class="apidocCodeCommentSpan">    /**
     * [read-only] Bearing information
     * @name bearing
     * @property
     * @type Object
     *
     *
        name
        abbr
        low
        mid
        high
        heading
     *
     */
</span>
    bearing: {
      get: function() {
        var length = Compass.Points.length;
        var heading = Math.floor(this.heading);
        var point;

        for (var i = 0; i < length; i++) {
          point = Compass.Points[i];

          if (point.range.includes(heading)) {
            // Specify fields to return to avoid returning the
            // range array (too much noisy data)
            return {
              name: point.name,
              abbr: point.abbr,
              low: point.low,
              high: point.high,
              heading: heading
            };
          }
        }
      }
    },

    /**
     * [read-only] Heading (azimuth)
     * @name heading
     * @property
     * @type number
     */
    heading: {
      get: function() {
        return this.toScaledHeading(raw);
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Digital"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Digital (opts)](#apidoc.element.nodebot-workshop.five.Digital)
- description and source-code
```javascript
Digital = function (opts) {
  var pin;

  if (typeof opts === "number" || typeof opts === "string") {
    pin = opts;
    opts = {
      type: "digital",
      pin: pin
    };
  } else {
    opts.type = opts.type || "digital";
  }

  return new module.exports.Sensor(opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.ESC"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>ESC (opts)](#apidoc.element.nodebot-workshop.five.ESC)
- description and source-code
```javascript
function ESC(opts) {
  if (!(this instanceof ESC)) {
    return new ESC(opts);
  }

  var controller = null;
  var pinValue;
  var device;
  var state = {
    // All speed history for this ESC
    // history = [
    //   {
    //     timestamp: Date.now(),
    //     speed: speed
    //   }
    // ];
    history: [],
    value: 0
  };

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  priv.set(this, state);

  this.startAt = typeof opts.startAt !== "undefined" ? opts.startAt : null;
  this.neutral = opts.neutral;
  this.range = opts.range || [0, 100];
  this.pwmRange = opts.pwmRange || [544, 2400];
  this.interval = null;

  // StandardFirmata on Arduino allows controlling
  // servos from analog pins.
  // If we're currently operating with an Arduino
  // and the user has provided an analog pin name
  // (eg. "A0", "A5" etc.), parse out the numeric
  // value and capture the fully qualified analog
  // pin number.
  if (typeof opts.controller === "undefined" && Pins.isFirmata(this)) {
    if (typeof pinValue === "string" && pinValue[0] === "A") {
      pinValue = this.io.analogPins[+pinValue.slice(1)];
    }

    pinValue = +pinValue;

    // If the board's default pin normalization
    // came up with something different, use the
    // the local value.
    if (!Number.isNaN(pinValue) && this.pin !== pinValue) {
      this.pin = pinValue;
    }
  }

  // Allow users to pass in custom device types
  device = typeof opts.device === "string" ?
    Devices[opts.device] : opts.device;

  if (!device) {
    device = Devices.FORWARD;
  }

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (!controller) {
    controller = Controllers.DEFAULT;
  }

  Object.defineProperties(this, Object.assign({}, device, controller, {
    value: {
      get: function() {
        return state.value;
      }
    },
    history: {
      get: function() {
        return state.history.slice(-5);
      }
    },
    last: {
      get: function() {
        return state.history[state.history.length - 1] || {
          last: null
        };
      }
    }
  }));

  this.initialize(opts);

  if (this.deviceName !== "FORWARD") {
    if (Number.isNaN(+this.neutral)) {
      throw new Error("Directional speed controllers require a neutral point from 0-100 (number)");
    }

    this.startAt = this.neutral;
  }

  // Match either null or undefined, but not 0
  if (this.startAt !== null && this.startAt !== undefined) {
    this.speed(this.startAt);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.ESCs"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>ESCs (numsOrObjects)](#apidoc.element.nodebot-workshop.five.ESCs)
- description and source-code
```javascript
function ESCs(numsOrObjects) {
  if (!(this instanceof ESCs)) {
    return new ESCs(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: ESC
  });

  Collection.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Expander"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Expander (opts)](#apidoc.element.nodebot-workshop.five.Expander)
- description and source-code
```javascript
function Expander(opts) {
  if (!(this instanceof Expander)) {
    return new Expander(opts);
  }

  Base.call(this);

  var expander = null;
  var addressError = "Expander cannot reuse an active address";
  var controller = null;
  var state = {};
  var controllerValue;

  if (typeof opts === "string") {
    controllerValue = opts;
  }

  Board.Component.call(
    this, opts = Board.Options(opts), {
      normalizePin: false,
      requestPin: false
    }
  );

  expander = active.get(this.address);

  if (expander) {
    if (this.bus && (expander.bus !== undefined && expander.bus === this.bus)) {
      addressError += " on this bus";
    }
    throw new Error(addressError);
  }

  if (typeof opts.controller === "undefined" && controllerValue) {
    opts.controller = controllerValue;
  }

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    throw new Error("Expander expects a valid controller");
  }

  Board.Controller.call(this, controller, opts);

  priv.set(this, state);

  if (typeof this.initialize === "function") {
    this.initialize(opts);
  }

  active.set(this.address, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.GPS"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>GPS (opts)](#apidoc.element.nodebot-workshop.five.GPS)
- description and source-code
```javascript
function GPS(opts) {

  var breakout, receiver, chip, state;

  if (!(this instanceof GPS)) {
    return new GPS(opts);
  }

  // Allow users to pass in a 2 element array for rx and tx pins
  if (Array.isArray(opts)) {
    opts = {
      pins: {
        rx: opts[0],
        tx: opts[1],
        onOff: opts[2]
      }
    };
  }

  if (typeof opts.pins === "undefined") {
    opts.pins = {};
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );



  // Get user values for breakout, receiver and chip
  breakout = opts.breakout || {};
  receiver = opts.receiver;
  chip = opts.chip;

  // If a breakout is defined check for receiver and chip
  if (Breakouts[breakout]) {
    if (!receiver && Breakouts[breakout].receiver) {
      receiver = Breakouts[breakout].receiver.value;
    }

    if (!chip && Breakouts[breakout].chip) {
      chip = Breakouts[breakout].chip.value;
    }
  }

  // If a receiver was defined or derived but chip was not
  if (!chip) {
    if (receiver && Receivers[receiver].chip) {
      chip = Receivers[receiver].chip.value;
    } else {
      chip = "DEFAULT";
    }
  }

  // Allow users to pass in custom chip types
  chip = typeof chip === "string" ?
    Chips[chip] : opts.chip;

  // Allow users to pass in custom receiver types
  receiver = typeof receiver === "string" ?
    Receivers[receiver] : opts.receiver;

  // Chip decorates the instance
  Object.defineProperties(this, chip);

  // Receiver decorates this instance
  if (receiver) {
    Object.defineProperties(this, receiver);
  }

  // breakout decorates the instance
  if (opts.breakout) {
    breakout = typeof opts.breakout === "string" ?
      Breakouts[opts.breakout] : opts.breakout;

    Board.Controller.call(this, breakout, opts);
  }

  // If necessary set default property values
  this.fixed = opts.fixed || 6;
  this.baud = opts.baud || this.baud;

  // Create a "state" entry for privately
  // storing the state of the instance
  state = {
    sat: {},
    latitude: 0.0,
    longitude: 0.0,
    altitude: 0.0,
    speed: 0.0,
    course: 0.0,
    frequency: 1,
    lowPowerMode: false
  };

  priv.set(this, state);

  // Getters for private state values
  Object.defineProperties(this, {
    latitude: {
      get: function() {
        return state.latitude;
      }
    },
    longitude: {
      get: function() {
        return state.longitude;
      }
    },
    altitude: {
      get: function() {
        return state.altitude;
      }
    },
    sat: {
      get: function() {
        return state.sat;
      }
    },
    speed: {
      get: function() {
        return state.speed;
      }
    },
    course: {
      get: function() {
        return state.course;
      }
    },
    time: {
      get: function() {
        return state.time;
      }
    }
  });

  if (this.initialize) {
    this.initialize(opts);
  }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Gripper"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Gripper (opts)](#apidoc.element.nodebot-workshop.five.Gripper)
- description and source-code
```javascript
function Gripper(opts) {

  if (!(this instanceof Gripper)) {
    return new Gripper(opts);
  }

  // Default options mode, assume only when opts is a pin number
  if (typeof opts === "number") {
    opts = {
      servo: {
        pin: opts,
        range: [0, 180]
      },
      scale: [0, 10]
    };
  }

  // Default set() args to 0-10
  this.scale = opts.scale || [0, 10];

  // Setup servo
  // Allows pre-constructed servo or creating new servo.
  // Defaults for new Servo creation fall back to Servo defaults
  this.servo = opts.servo instanceof Servo ?
    opts.servo : new Servo(opts.servo);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Gyro"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Gyro (opts)](#apidoc.element.nodebot-workshop.five.Gyro)
- description and source-code
```javascript
function Gyro(opts) {
  if (!(this instanceof Gyro)) {
    return new Gyro(opts);
  }

  var controller = null;
  var isCalibrated = false;
  var sampleSize = 100;

  var state = {
    x: {
      angle: 0,
      value: 0,
      previous: 0,
      calibration: [],
      stash: [0, 0, 0, 0, 0],
      center: 0,
      hasValue: false
    },
    y: {
      angle: 0,
      value: 0,
      previous: 0,
      calibration: [],
      stash: [0, 0, 0, 0, 0],
      center: 0,
      hasValue: false
    },
    z: {
      angle: 0,
      value: 0,
      previous: 0,
      calibration: [],
      stash: [0, 0, 0, 0, 0],
      center: 0,
      hasValue: false
    }
  };

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.ANALOG;
  }

  Board.Controller.call(this, controller, opts);

  if (!this.toNormal) {
    this.toNormal = opts.toNormal || function(raw) {
      return raw;
    };
  }

  if (!this.toDegreesPerSecond) {
    this.toDegreesPerSecond = opts.toDegreesPerSecond || function(raw) {
      return raw;
    };
  }

  priv.set(this, state);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      var isChange = false;

      Object.keys(data).forEach(function(axis) {
        var value = data[axis];
        var sensor = state[axis];

        sensor.previous = sensor.value;
        sensor.stash.shift();
        sensor.stash.push(value);
        sensor.hasValue = true;
        sensor.value = (sum(sensor.stash) / 5) | 0;

        if (!isCalibrated &&
          (state.x.calibration.length === sampleSize &&
            state.y.calibration.length === sampleSize &&
            (this.z === undefined || state.z.calibration.length === sampleSize))) {

          isCalibrated = true;
          state.x.center = (sum(state.x.calibration) / sampleSize) | 0;
          state.y.center = (sum(state.y.calibration) / sampleSize) | 0;
          state.z.center = (sum(state.z.calibration) / sampleSize) | 0;

          state.x.calibration.length = 0;
          state.y.calibration.length = 0;
          state.z.calibration.length = 0;
        } else {
          if (sensor.calibration.length < sampleSize) {
            sensor.calibration.push(value);
          }
        }

        if (sensor.previous !== sensor.value) {
          isChange = true;
        }
      }, this);

      if (isCalibrated) {
        state.x.angle += this.rate.x / 100;
        state.y.angle += this.rate.y / 100;
        state.z.angle += this.rate.z / 100;

        this.emit("data", {
          x: this.x,
          y: this.y,
          z: this.z
        });

        if (isChange) {
          this.emit("change", {
            x: this.x,
            y: this.y,
            z: this.z
          });
        }
      }
    }.bind(this));
  }

  Object.defineProperties(this, {
    isCalibrated: {
      get: function() {
        return isCalibrated;
      },
      set: function(value) {
        if (typeof value === "boolean") {
          isCalibrated = value;
        }
      }
    },
    pitch: {
      get: function() {
        return {
          rate: toFixed(this.rate.y, 2),
          angle: toFixed(state.y.angle, 2)
        };
      }
    },
    roll: {
      get: function() {
        return {
          rate: toFixed(this.rate.x, 2),
          angle: toFixed(state.x.angle, 2)
        };
      }
    },
    yaw: {
      get: function() {
        return {
          rate: this.z !== undefined ? toFixed(this.rate.z, 2) : 0,
          angle: this.z !== undefined ? toFixed(state.z.angle, 2) : 0
        };
      }
    },
    x: {
      get: function() {
        return toFixed(this.toNormal(state.x.value), 4);
      }
    },
    y: {
      get: function() {
        return toFixed(this.toNormal(state.y.value), 4);
      }
    },
    z: {
      get: function() {
        return state.z.hasValue ? toFixed(this.toNormal(state. ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Hygrometer"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Hygrometer (opts)](#apidoc.element.nodebot-workshop.five.Hygrometer)
- description and source-code
```javascript
function Hygrometer(opts) {
  if (!(this instanceof Hygrometer)) {
    return new Hygrometer(opts);
  }

  var controller = null;
  var last = null;
  var raw = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var freq = opts.freq || 25;

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    throw new Error("Missing Hygrometer controller");
  }

  priv.set(this, {});

  Board.Controller.call(this, controller, opts);

  if (!this.toRelativeHumidity) {
    this.toRelativeHumidity = opts.toRelativeHumidity || function(x) {
      return x;
    };
  }

  var propDescriptors = {
    relativeHumidity: {
      get: function() {
        return this.toRelativeHumidity(raw);
      }
    }
  };
  // Convenience aliases
  propDescriptors.RH = propDescriptors.relativeHumidity;

  Object.defineProperties(this, propDescriptors);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  setInterval(function() {
    if (raw == null) {
      return;
    }

    if (Number.isNaN(this.relativeHumidity)) {
      return;
    }

    var data = {};
    data.RH = data.relativeHumidity = this.relativeHumidity;

    this.emit("data", data);

    if (this.relativeHumidity !== last) {
      last = this.relativeHumidity;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.IMU"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>IMU (opts)](#apidoc.element.nodebot-workshop.five.IMU)
- description and source-code
```javascript
function IMU(opts) {

  if (!(this instanceof IMU)) {
    return new IMU(opts);
  }

  var controller, state;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    throw new Error("Missing IMU/Multi controller");
  }

  this.freq = opts.freq || 20;

  state = {};
  priv.set(this, state);

  Board.Controller.call(this, controller, opts);

  if (typeof this.initialize === "function") {
    this.initialize(opts);
  }

  // The IMU/Multi isn't considered "ready"
  // until one of the components has notified via
  // a change event.
  this.isReady = false;

  setInterval(function() {
    if (this.isReady) {
      this.emit("data", this);
    }
  }.bind(this), this.freq);

  var awaiting = this.components.slice();

  if (this.components && this.components.length > 0) {
    this.components.forEach(function(component) {
      if (!(this[component] instanceof Emitter)) {
        return;
      }

      this[component].on("change", function() {
        if (awaiting.length) {
          var index = awaiting.indexOf(component);

          if (index !== -1) {
            awaiting.splice(index, 1);
          }
        }

        if (!awaiting.length && !this.isReady) {
          this.isReady = true;
        }

        if (this.isReady) {
          this.emit("change", this, component);
        }
      }.bind(this));
    }, this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.IR"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>IR ()](#apidoc.element.nodebot-workshop.five.IR)
- description and source-code
```javascript
IR = function () {
  throw new Error("IR has been removed. Use Motion or Proximity instead.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Joystick"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Joystick (opts)](#apidoc.element.nodebot-workshop.five.Joystick)
- description and source-code
```javascript
function Joystick(opts) {
  if (!(this instanceof Joystick)) {
    return new Joystick(opts);
  }

  var controller = null;

  var state = {
    x: {
      invert: false,
      value: 0,
      previous: 0,
      zeroV: 0,
      calibrated: false
    },
    y: {
      invert: false,
      value: 0,
      previous: 0,
      zeroV: 0,
      calibrated: false
    }
  };

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.ANALOG;
  }

  Board.Controller.call(this, controller, opts);

  if (!this.toAxis) {
    this.toAxis = opts.toAxis || function(raw) {
      return raw;
    };
  }

  state.x.zeroV = opts.zeroV === undefined ? 0 : (opts.zeroV.x || 0);
  state.y.zeroV = opts.zeroV === undefined ? 0 : (opts.zeroV.y || 0);

  state.x.invert = opts.invertX || opts.invert || false;
  state.y.invert = opts.invertY || opts.invert || false;

  priv.set(this, state);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      var isChange = false;
      var computed = {
        x: null,
        y: null
      };

      Object.keys(data).forEach(function(axis) {
        var value = data[axis];
        var sensor = state[axis];

        // Set the internal ADC reading value...
        sensor.value = value;

        if (!state[axis].calibrated) {
          state[axis].calibrated = true;
          state[axis].zeroV = value;
          isChange = true;
        }

        // ... Get the computed axis value.
        computed[axis] = this[axis];

        var absAxis = Math.abs(computed[axis]);
        var absPAxis = Math.abs(sensor.previous);

        if ((absAxis < absPAxis) ||
          (absAxis > absPAxis)) {
          isChange = true;
        }

        sensor.previous = computed[axis];
      }, this);

      this.emit("data", {
        x: computed.x,
        y: computed.y
      });

      if (isChange) {
        this.emit("change", {
          x: computed.x,
          y: computed.y
        });
      }
    }.bind(this));
  }

  Object.defineProperties(this, {
    x: {
      get: function() {
        return this.toAxis(state.x.value, "x") * (state.x.invert ? -1 : 1);
      }
    },
    y: {
      get: function() {
        return this.toAxis(state.y.value, "y") * (state.y.invert ? -1 : 1);
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Keypad"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Keypad (opts)](#apidoc.element.nodebot-workshop.five.Keypad)
- description and source-code
```javascript
function Keypad(opts) {

  if (!(this instanceof Keypad)) {
    return new Keypad(opts);
  }

  // Initialize a Device instance on a Board
  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var raw = null;
  var controller = null;
  var state = {
    touches: null,
    timeout: null,
    length: null,
    keys: null,
    mapping: null,
    holdtime: null,
  };

  var trigger = Fn.debounce(function(type, value) {
    var event = {
      type: type,
      which: value,
      timestamp: Date.now()
    };
    aliases[type].forEach(function(type) {
      this.emit(type, event);
    }, this);

    this.emit("change", Object.assign({}, event));
  }, 5);


  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.ANALOG;
  }

  Board.Controller.call(this, controller, opts);

  state.holdtime = opts.holdtime ? opts.holdtime : 500;

  priv.set(this, state);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {

      raw = data;

      var now = Date.now();
      var indices = this.toIndices(data);
      var kLength = state.length;

      var lists = {
        down: [],
        hold: [],
        up: [],
      };

      var target = null;
      var alias = null;

      for (var k = 0; k < kLength; k++) {
        alias = this.toAlias(k);

        if (indices.includes(k)) {
          if (state.touches[k].value === 0) {

            state.touches[k].timeout = now + state.holdtime;
            lists.down.push(alias);

          } else if (state.touches[k].value === 1) {
            if (state.touches[k].timeout !== null && now > state.touches[k].timeout) {
              state.touches[k].timeout = now + state.holdtime;
              lists.hold.push(alias);
            }
          }

          state.touches[k].value = 1;
        } else {
          if (state.touches[k].value === 1) {
            state.touches[k].timeout = null;
            lists.up.push(alias);
          }
          state.touches[k].value = 0;
        }
        target = null;
        alias = null;
      }

      Object.keys(lists).forEach(function(key) {
        var list = lists[key];

        if (list.length) {
          trigger.call(this, key, list);
        }
      }, this);
    }.bind(this));
  }

  Object.defineProperties(this, {
    isMultitouch: {
      get: function() {
        return state.isMultitouch;
      }
    },
    value: {
      get: function() {
        return raw;
      }
    },
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.LCD"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>LCD (opts)](#apidoc.element.nodebot-workshop.five.LCD)
- description and source-code
```javascript
function LCD(opts) {

  if (!(this instanceof LCD)) {
    return new LCD(opts);
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var controller = null;

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.PARALLEL;
  }

  Board.Controller.call(this, controller, opts);

  this.ctype = opts.controller;

  if (this.initialize) {
    this.initialize(opts);
  }

  Object.defineProperties(this, {
    characters: {
      get: function() {
        return Object.assign({}, priv.get(this).characters);
      },
    },
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Led"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Led (opts)](#apidoc.element.nodebot-workshop.five.Led)
- description and source-code
```javascript
function Led(opts) {
  if (!(this instanceof Led)) {
    return new Led(opts);
  }

  var pinValue = typeof opts === "object" ? opts.pin : opts;
  var controller = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.DEFAULT;
  }

  Object.defineProperties(this, controller);

  var state = {
    isAnode: opts.isAnode,
    isOn: false,
    isRunning: false,
    value: null,
    direction: 1,
    mode: null,
    intensity: 0,
    interval: null
  };

  priv.set(this, state);

  Object.defineProperties(this, {
    value: {
      get: function() {
        return state.value;
      }
    },
    mode: {
      get: function() {
        return state.mode;
      }
    },
    isOn: {
      get: function() {
        return !!state.value;
      }
    },
    isRunning: {
      get: function() {
        return state.isRunning;
      }
    },
    animation: {
      get: function() {
        return state.animation;
      }
    }
  });

<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (typeof this.initialize === "function") {
    this.initialize(opts, pinValue);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.LedControl"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>LedControl (opts)](#apidoc.element.nodebot-workshop.five.LedControl)
- description and source-code
```javascript
function LedControl(opts) {

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

<span class="apidocCodeCommentSpan">  /*
   device instance uses an interface from Controllers:
   either MAX 7219 (default) or HT16K33
   */
</span>  var controller = null;

  if (typeof opts.controller === "string") {
    controller = Controllers[opts.controller];
  } else {
    controller = opts.controller;
  }

  if (typeof controller === "undefined") {
    controller = Controllers.DEFAULT;
  }

  // functions from Controller interface

  this.clear = controller.clear;
  this.led = controller.led;
  this.row = controller.row;
  this.scanLimit = controller.scanLimit;
  this.send = controller.send;
  this.sendDigit = controller.sendDigit;
  this.initialize = controller.initialize;

  // controller specific op codes
  this.OP = controller.OP;

  // digit indexes may be ordered left to right (1) or reversed (-1)
  this.digitOrder = 1;

  // Does the device have a built-in colon?
  /* istanbul ignore else */
  if (!this.isMatrix) {
    this.colon = opts.colon || false;
  }

  // extra functions for HT16K33 devices only
  if (controller.writeDisplay) {
    this.writeDisplay = controller.writeDisplay;
  }
  if (controller.blink) {
    this.blink = controller.blink;
  }
  /*
    devices variable indicates number of connected LED devices
    Here's an example of multiple devices:
    http://tronixstuff.com/2013/10/11/tutorial-arduino-max7219-led-display-driver-ic/
   */
  var devices = opts.devices || (opts.addresses ? opts.addresses.length : 1);

  this.memory = Array(64).fill(0);

  opts.dims = opts.dims || LedControl.MATRIX_DIMENSIONS["8x8"];
  if (typeof opts.dims === "string") {
    opts.dims = LedControl.MATRIX_DIMENSIONS[opts.dims];
  }
  if (Array.isArray(opts.dims)) {
    opts.dims = {
      rows: opts.dims[0],
      columns: opts.dims[1],
    };
  }
  var state = {
    devices: devices,
    digits: opts.digits || 8,
    isMatrix: !!opts.isMatrix,
    isBicolor: !!opts.isBicolor,
    rows: opts.dims.rows,
    columns: opts.dims.columns
  };

  if (!(state.columns === 8 || state.columns === 16) || !(state.rows === 8 || state.rows === 16) || (state.columns + state.rows ===
32)) {
    throw new Error("Invalid matrix dimensions specified: must be 8x8, 16x8 or 8x16");
  }

  Object.defineProperties(this, {
    devices: {
      get: function() {
        return state.devices;
      }
    },
    digits: {
      get: function() {
        return state.digits;
      }
    },
    isMatrix: {
      get: function() {
        return state.isMatrix;
      }
    },
    isBicolor: {
      get: function() {
        return state.isBicolor;
      }
    },
    rows: {
      get: function() {
        return state.rows;
      }
    },
    columns: {
      get: function() {
        return state.columns;
      }
    }
  });

  priv.set(this, state);
  controller.initialize.call(this, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Leds"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Leds (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Leds)
- description and source-code
```javascript
function Leds(numsOrObjects) {
  if (!(this instanceof Leds)) {
    return new Leds(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Led
  });

  Collection.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Light"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Light (opts)](#apidoc.element.nodebot-workshop.five.Light)
- description and source-code
```javascript
function Light(opts) {

  if (!(this instanceof Light)) {
    return new Light(opts);
  }

  var controller = null;
  var state = {};
  var raw = 0;
  var last = 0;
  var freq = opts.freq || 25;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (typeof opts.controller === "string") {
    controller = Controllers[opts.controller];
  } else {
    controller = opts.controller || Controllers.DEFAULT;
  }

  Board.Controller.call(this, controller, opts);

  if (!this.toIntensityLevel) {
    this.toIntensityLevel = opts.toIntensityLevel || function(x) {
      return x;
    };
  }

  if (!this.toLux) {
    this.toLux = opts.toLux || function(x) {
      return x;
    };
  }

  Object.defineProperties(this, {
    value: {
      get: function() {
        return raw;
      },
    },
    level: {
      get: function() {
        return this.toIntensityLevel(raw);
      },
    },
  });

  priv.set(this, state);

<span class="apidocCodeCommentSpan">  /* istanbul ignore else */
</span>  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  if (typeof this.lux === "undefined") {
    Object.defineProperty(this, "lux", {
      get: function() {
        return this.toLux(raw);
      },
    });
  }

  var data = {
    level: 0,
    lux: 0,
  };

  setInterval(function() {
    data.level = this.level;
    data.lux = this.lux;

    this.emit("data", data);

    if (raw !== last) {
      last = raw;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Luxmeter"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Luxmeter (options)](#apidoc.element.nodebot-workshop.five.Luxmeter)
- description and source-code
```javascript
Luxmeter = function (options) {
  return new module.exports.Light(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Magnetometer"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Magnetometer (options)](#apidoc.element.nodebot-workshop.five.Magnetometer)
- description and source-code
```javascript
Magnetometer = function (options) {
  return new module.exports.Compass(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Motion"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Motion (opts)](#apidoc.element.nodebot-workshop.five.Motion)
- description and source-code
```javascript
function Motion(opts) {

  if (!(this instanceof Motion)) {
    return new Motion(opts);
  }

  var freq = opts.freq || 25;
  var last = false;
  var controller;
  var state;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (typeof opts.controller === "string") {
    controller = Controllers[opts.controller];
  } else {
    controller = opts.controller || Controllers["PIR"];
  }

  Board.Controller.call(this, controller, opts);

  state = {
    value: false,
    isCalibrated: false
  };

  priv.set(this, state);

  Object.defineProperties(this, {
<span class="apidocCodeCommentSpan">    /**
     * [read-only] Current sensor state
     * @property detectedMotion
     * @type Boolean
     */
</span>    detectedMotion: {
      get: function() {
        return this.toBoolean(state.value);
      }
    },
    /**
     * [read-only] Sensor calibration status
     * @property isCalibrated
     * @type Boolean
     */
    isCalibrated: {
      get: function() {
        return state.isCalibrated;
      }
    },
  });

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      state.value = data;
    });
  }

  setInterval(function() {
    var isChange = false;
    var eventData = {
      timestamp: Date.now(),
      detectedMotion: this.detectedMotion,
      isCalibrated: state.isCalibrated
    };

    if (state.isCalibrated && this.detectedMotion && !last) {
      this.emit("motionstart", eventData);
    }

    if (state.isCalibrated && !this.detectedMotion && last) {
      this.emit("motionend", eventData);
    }

    if (last !== this.detectedMotion) {
      isChange = true;
    }

    this.emit("data", eventData);

    if (isChange) {
      this.emit("change", eventData);
    }

    last = this.detectedMotion;
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Motor"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Motor (opts)](#apidoc.element.nodebot-workshop.five.Motor)
- description and source-code
```javascript
function Motor(opts) {

  var device, controller, state;

  if (!(this instanceof Motor)) {
    return new Motor(opts);
  }

  Board.Component.call(
    this, this.opts = Board.Options(opts)
  );

  controller = opts.controller || null;

  // Derive device based on pins passed
  if (typeof this.opts.device === "undefined") {

    this.opts.device = (typeof this.opts.pins === "undefined" && typeof this.opts.register !== "object") ?
      "NONDIRECTIONAL" : "DIRECTIONAL";

    if (this.opts.pins && (this.opts.pins.cdir || this.opts.pins.length > 2)) {
      this.opts.device = "CDIR";
    }

    if (typeof controller === "string" &&
      (controller.startsWith("EVS") || controller.startsWith("GROVE_I2C"))) {
      this.opts.device = "DIRECTIONAL";
    }
  }

  // Allow users to pass in custom device types
  device = typeof this.opts.device === "string" ?
    Devices[this.opts.device] : this.opts.device;

  this.threshold = typeof this.opts.threshold !== "undefined" ?
    this.opts.threshold : 30;

  this.invertPWM = typeof this.opts.invertPWM !== "undefined" ?
    this.opts.invertPWM : false;

  Object.defineProperties(this, device);

  if (this.opts.register) {
    this.opts.controller = "ShiftRegister";
  }

<span class="apidocCodeCommentSpan">  /**
   * Note: Controller decorates the device. Used for adding
   * special controllers (i.e. PCA9685)
   **/
</span>  if (this.opts.controller) {
    controller = typeof this.opts.controller === "string" ?
      Controllers[this.opts.controller] : this.opts.controller;

    Board.Controller.call(this, controller, opts);
  }

  // current just wraps a Sensor
  if (this.opts.current) {
    this.opts.current.board = this.board;
    this.current = new Sensor(this.opts.current);
  }

  // Create a "state" entry for privately
  // storing the state of the motor
  state = {
    isOn: false,
    currentSpeed: typeof this.opts.speed !== "undefined" ?
      this.opts.speed : 128,
    braking: false,
    enabled: true
  };

  priv.set(this, state);

  Object.defineProperties(this, {
    // Calculated, read-only motor on/off state
    // true|false
    isOn: {
      get: function() {
        return state.isOn;
      }
    },
    currentSpeed: {
      get: function() {
        return state.currentSpeed;
      }
    },
    braking: {
      get: function() {
        return state.braking;
      }
    },
    enabled: {
      get: function() {
        return state.enabled;
      }
    }
  });

  // We need to store and initialize the state of the dir pin(s)
  this.direction = {
    value: 1
  };

  if (this.initialize) {
    this.initialize(opts);
  }

  this.enable();
  this.dir(this.direction);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Motors"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Motors (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Motors)
- description and source-code
```javascript
function Motors(numsOrObjects) {
  if (!(this instanceof Motors)) {
    return new Motors(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Motor
  });

  Collection.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Multi"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Multi (opts)](#apidoc.element.nodebot-workshop.five.Multi)
- description and source-code
```javascript
function IMU(opts) {

  if (!(this instanceof IMU)) {
    return new IMU(opts);
  }

  var controller, state;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    throw new Error("Missing IMU/Multi controller");
  }

  this.freq = opts.freq || 20;

  state = {};
  priv.set(this, state);

  Board.Controller.call(this, controller, opts);

  if (typeof this.initialize === "function") {
    this.initialize(opts);
  }

  // The IMU/Multi isn't considered "ready"
  // until one of the components has notified via
  // a change event.
  this.isReady = false;

  setInterval(function() {
    if (this.isReady) {
      this.emit("data", this);
    }
  }.bind(this), this.freq);

  var awaiting = this.components.slice();

  if (this.components && this.components.length > 0) {
    this.components.forEach(function(component) {
      if (!(this[component] instanceof Emitter)) {
        return;
      }

      this[component].on("change", function() {
        if (awaiting.length) {
          var index = awaiting.indexOf(component);

          if (index !== -1) {
            awaiting.splice(index, 1);
          }
        }

        if (!awaiting.length && !this.isReady) {
          this.isReady = true;
        }

        if (this.isReady) {
          this.emit("change", this, component);
        }
      }.bind(this));
    }, this);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Nunchuk"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Nunchuk (opts)](#apidoc.element.nodebot-workshop.five.Nunchuk)
- description and source-code
```javascript
Nunchuk = function (opts) {
  opts = opts || {};
  opts.device = "RVL-004";

  return new Wii(opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Piezo"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Piezo (opts)](#apidoc.element.nodebot-workshop.five.Piezo)
- description and source-code
```javascript
function Piezo(opts) {

  if (!(this instanceof Piezo)) {
    return new Piezo(opts);
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var controller = null;

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.DEFAULT;
  }

  Object.defineProperties(this, controller);

  Board.Controller.call(this, controller, opts);

  // Piezo instance properties
  var state = {
    isPlaying: false,
    timeout: null,
    address: null,
  };

  priv.set(this, state);

  Object.defineProperties(this, {
    isPlaying: {
      get: function() {
        return state.isPlaying;
      }
    }
  });

  if (typeof this.initialize === "function") {
    this.initialize(opts);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Pin"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Pin (opts)](#apidoc.element.nodebot-workshop.five.Pin)
- description and source-code
```javascript
function Pin(opts) {
  if (!(this instanceof Pin)) {
    return new Pin(opts);
  }
  if (opts === undefined || (typeof opts === "object" &&
      opts.addr === undefined && opts.pin === undefined)) {
    throw new Error("Pins must have a pin number");
  }

  var pinValue = typeof opts === "object" ? (opts.addr || opts.pin || 0) : opts;
  var isAnalogInput = Pin.isAnalog(opts);
  var isDTOA = false;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  opts.addr = opts.addr || opts.pin;

  if (this.io.analogPins.includes(pinValue)) {
    isAnalogInput = false;
    isDTOA = true;
  }

  var isPin = typeof opts !== "object";
  var addr = isDTOA ? pinValue : (isPin ? opts : opts.addr);
  var type = opts.type || (isAnalogInput ? "analog" : "digital");

  // Create a private side table
  var state = {
    mode: null,
    last: null,
    value: 0
  };

  priv.set(this, state);

  // Create read-only "addr(address)" property
  Object.defineProperties(this, {
    type: {
      get: function() {
        return type;
      }
    },
    addr: {
      get: function() {
        return addr;
      }
    },
    value: {
      get: function() {
        return state.value;
      }
    },
    mode: {
      set: function(mode) {
        var state = priv.get(this);
        state.mode = mode;
        this.io.pinMode(this.addr, mode);
      },
      get: function() {
        return priv.get(this).mode;
      }
    }
  });

  this.mode = typeof opts.as !== "undefined" ? opts.as :
    (typeof opts.mode !== "undefined" ? opts.mode : (isAnalogInput ? 0x02 : 0x01));

  this.freq = typeof opts.freq !== "undefined" ? opts.freq : 20;

  if (this.mode === 0 || this.mode === 2) {
    read(this);
  }

  if (type === "digital") {
    Object.defineProperties(this, {
      isHigh: {
        get: function() {
          return !!state.value;
        }
      },
      isLow: {
        get: function() {
          return !state.value;
        }
      },
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Ping"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Ping (opts)](#apidoc.element.nodebot-workshop.five.Ping)
- description and source-code
```javascript
function Ping(opts) {

  if (!(this instanceof Ping)) {
    return new Ping(opts);
  }

  var last = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  this.pin = opts && opts.pin || 7;
  this.freq = opts.freq || 20;
  // this.pulse = opts.pulse || 250;

  var state = {
    value: null
  };

  // Private settings object
  var settings = {
    pin: this.pin,
    value: this.io.HIGH,
    pulseOut: 5
  };

  this.io.setMaxListeners(100);

  // Interval for polling pulse duration as reported in microseconds
  setInterval(function() {
    this.io.pingRead(settings, function(microseconds) {
      state.value = microseconds;
    });
  }.bind(this), 225);

  // Interval for throttled event
  setInterval(function() {
    if (state.value === null) {
      return;
    }

    // The "read" event has been deprecated in
    // favor of a "data" event.
    this.emit("data", state.value);

    // If the state.value for this interval is not the same as the
    // state.value in the last interval, fire a "change" event.
    if (state.value !== last) {
      this.emit("change", state.value);
    }

    // Store state.value for comparison in next interval
    last = state.value;

    // Reset samples;
    // samples.length = 0;
  }.bind(this), this.freq);

  Object.defineProperties(this, {
    value: {
      get: function() {
        return state.value;
      }
    },
    // Based on the round trip travel time in microseconds,
    // Calculate the distance in inches and centimeters
    inches: {
      get: function() {
        return toFixed(state.value / 74 / 2, 2);
      }
    },
    in: {
      get: function() {
        return this.inches;
      }
    },
    cm: {
      get: function() {
        return toFixed(state.value / 29 / 2, 3);
      }
    }
  });

  priv.set(this, state);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Pins"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Pins (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Pins)
- description and source-code
```javascript
function Pins(numsOrObjects) {
  if (!(this instanceof Pins)) {
    return new Pins(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Pin
  });

  Collection.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Proximity"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Proximity (opts)](#apidoc.element.nodebot-workshop.five.Proximity)
- description and source-code
```javascript
function Proximity(opts) {

  if (!(this instanceof Proximity)) {
    return new Proximity(opts);
  }

  var controller = null;
  var state = {};
  var raw = 0;
  var freq = opts.freq || 25;
  var last = 0;
  var pinValue = typeof opts === "object" ? opts.pin : opts;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (typeof opts.controller === "string") {
    controller = Controllers[opts.controller];
  } else {
    controller = opts.controller || Controllers["GP2Y0A21YK"];
  }

  Board.Controller.call(this, controller, opts);

  if (!this.toCm) {
    this.toCm = opts.toCm || function(x) {
      return x;
    };
  }

  priv.set(this, state);

  Object.defineProperties(this, {
<span class="apidocCodeCommentSpan">    /**
     * [read-only] Calculated centimeter value
     * @property centimeters
     * @type Number
     */
</span>    centimeters: {
      get: function() {
        return this.toCm(raw);
      }
    },
    cm: {
      get: function() {
        return this.centimeters;
      }
    },
    /**
     * [read-only] Calculated inch value
     * @property inches
     * @type Number
     */
    inches: {
      get: function() {
        return toFixed(this.centimeters * 0.39, 2);
      }
    },
    in: {
      get: function() {
        return this.inches;
      }
    },
  });

  if (typeof this.initialize === "function") {
    opts.pinValue = pinValue;
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  setInterval(function() {
    if (raw === undefined) {
      return;
    }

    var data = {
      cm: this.cm,
      centimeters: this.centimeters,
      in: this.in,
      inches: this.inches
    };

    this.emit("data", data);

    if (raw !== last) {
      last = raw;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Relay"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Relay (opts)](#apidoc.element.nodebot-workshop.five.Relay)
- description and source-code
```javascript
function Relay(opts) {

  var state;

  if (!(this instanceof Relay)) {
    return new Relay(opts);
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  opts.type = opts.type || "NO";

  state = {
    isInverted: opts.type === "NC",
    isOn: false,
    value: null,
  };

  priv.set(this, state);

  Object.defineProperties(this, {
    value: {
      get: function() {
        return Number(this.isOn);
      }
    },
    type: {
      get: function() {
        return state.isInverted ? "NC" : "NO";
      }
    },
    isOn: {
      get: function() {
        return state.isOn;
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Relays"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Relays (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Relays)
- description and source-code
```javascript
function Relays(numsOrObjects) {
  if (!(this instanceof Relays)) {
    return new Relays(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Relay
  });

  Collection.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Repl"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Repl (opts)](#apidoc.element.nodebot-workshop.five.Repl)
- description and source-code
```javascript
function Repl(opts) {
  if (!Repl.isActive) {
    Repl.isActive = true;

    if (!(this instanceof Repl)) {
      return new Repl(opts);
    }

    // Store context values in instance property
    // this will be used for managing scope when
    // injecting new values into an existing Repl
    // session.
    this.context = {};
    this.ready = false;

    var state = {
      opts: opts,
      board: opts.board,
    };

    priv.set(this, state);

    // Store an accessible copy of the Repl instance
    // on a static property. This is later used by the
    // Board constructor to automattically setup Repl
    // sessions for all programs, which reduces the
    // boilerplate requirement.
    Repl.ref = this;
  } else {
    return Repl.ref;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Sensor"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Sensor (opts)](#apidoc.element.nodebot-workshop.five.Sensor)
- description and source-code
```javascript
function Sensor(opts) {

  if (!(this instanceof Sensor)) {
    return new Sensor(opts);
  }

  // Defaults to 10-bit resolution
  var resolution = 0x3FF;
  var raw = null;
  var last = -1;
  var samples = [];

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (!opts.type) {
    opts.type = "analog";
  }

  if (this.io.RESOLUTION &&
      (this.io.RESOLUTION.ADC &&
        (this.io.RESOLUTION.ADC !== resolution))) {
    resolution = this.io.RESOLUTION.ADC;
  }

  // Set the pin to ANALOG (INPUT) mode
  this.mode = opts.type === "digital" ?
    this.io.MODES.INPUT :
    this.io.MODES.ANALOG;

  this.io.pinMode(this.pin, this.mode);

  // Create a "state" entry for privately
  // storing the state of the sensor
  var state = {
    enabled: typeof opts.enabled === "undefined" ? true : opts.enabled,
    booleanBarrier: opts.type === "digital" ? 0 : null,
    intervalId: null,
    scale: null,
    value: 0,
    median: 0,
    freq: opts.freq || 25,
    previousFreq: opts.freq || 25,
  };
  // Put a reference where the prototype methods defined in this file have access
  priv.set(this, state);

  // Sensor instance properties
  this.range = opts.range || [0, resolution];
  this.limit = opts.limit || null;
  this.threshold = opts.threshold === undefined ? 1 : opts.threshold;
  this.isScaled = false;

  this.io[opts.type + "Read"](this.pin, function(data) {
    raw = data;

    // Only append to the samples when noise filtering can/will be used
    if (opts.type !== "digital") {
      samples.push(raw);
    }
  }.bind(this));

  // Throttle
  // TODO: The event (interval) processing function should be outside of the Sensor
  // constructor function (with appropriate passed (and bound?) arguments), to
  // avoid creating a separate copy (of the function) for each Sensor instance.
  var eventProcessing = function() {
    var err, boundary;

    err = null;

    // For digital sensors, skip the analog
    // noise filtering provided below.
    if (opts.type === "digital") {
      this.emit("data", raw);

<span class="apidocCodeCommentSpan">      /* istanbul ignore else */
</span>      if (last !== raw) {
        this.emit("change", raw);
        last = raw;
      }
      return;
    }

    // Keep the previous calculated value if there were no new readings
    if (samples.length > 0) {
      // Filter the accumulated sample values to reduce analog reading noise
      state.median = median(samples);
    }

    this.emit("data", state.median);

    // If the filtered (state.median) value for this interval is at least ± the
    // configured threshold from last, fire change events
    if (state.median <= (last - this.threshold) || state.median >= (last + this.threshold)) {
      this.emit("change", state.median);
      // Update the instance-local 'last' value (only) when a new change event
      // has been emitted.  For comparison in the next interval
      last = state.median;
    }

    if (this.limit) {
      if (state.median <= this.limit[0]) {
        boundary = "lower";
      }
      if (state.median >= this.limit[1]) {
        boundary = "upper";
      }

      if (boundary) {
        this.emit("limit", {
          boundary: boundary,
          value: state.median
        });
        this.emit("limit:" + boundary, state.median);
      }
    }

    // Reset samples
    samples.length = 0;
  }.bind(this); // ./function eventProcessing()


  Object.defineProperties(this, {
    raw: {
      get: function() {
        return raw;
      }
    },
    analog: {
      get: function() {
        if (opts.type === "digital") {
          return raw;
        }

        return raw === null ? 0 :
          Fn.map(this.raw, 0, resolution, 0, 255) | 0;
      },
    },
    constrained: {
      get: function() {
        if (opts.type === "digital") {
          return raw;
        }

        return raw === null ? 0 :
          Fn.constrain(this.raw, 0, 255);
      }
    },
    boolean: {
      get: function() {
        var state = priv.get(this);
        var booleanBarrier = state.booleanBarrier;
        var scale = state.scale || [0, resolution];

        if (boolean ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Sensors"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Sensors (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Sensors)
- description and source-code
```javascript
function Sensors(numsOrObjects) {
  if (!(this instanceof Sensors)) {
    return new Sensors(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Sensor
  });

  Collection.Emitter.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Servo"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Servo (opts)](#apidoc.element.nodebot-workshop.five.Servo)
- description and source-code
```javascript
function Servo(opts) {

  if (!(this instanceof Servo)) {
    return new Servo(opts);
  }

  var history = [];
  var pinValue = typeof opts === "object" ? opts.pin : opts;
  var controller = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  this.range = opts.range || [0, 180];
  this.deadband = opts.deadband || [90, 90];
  this.fps = opts.fps || 100;
  this.offset = opts.offset || 0;
  this.mode = this.io.MODES.SERVO;
  this.interval = null;
  this.value = null;

  // StandardFirmata on Arduino allows controlling
  // servos from analog pins.
  // If we're currently operating with an Arduino
  // and the user has provided an analog pin name
  // (eg. "A0", "A5" etc.), parse out the numeric
  // value and capture the fully qualified analog
  // pin number.
  if (typeof opts.controller === "undefined" && Pins.isFirmata(this)) {
    if (typeof pinValue === "string" && pinValue[0] === "A") {
      pinValue = this.io.analogPins[+pinValue.slice(1)];
    }

    pinValue = +pinValue;

    // If the board's default pin normalization
    // came up with something different, use the
    // the local value.
    if (!Number.isNaN(pinValue) && this.pin !== pinValue) {
      this.pin = pinValue;
    }
  }


  // The type of servo determines certain alternate
  // behaviours in the API
  this.type = opts.type || "standard";

  // Invert the value of all servoWrite operations
  // eg. 80 => 100, 90 => 90, 0 => 180
  if (opts.isInverted) {
    console.warn("The 'isInverted' property has been renamed 'invert'");
  }
  this.invert = opts.isInverted || opts.invert || false;

  // Allow "setup"instructions to come from
  // constructor options properties
  this.startAt = 90;

  // Collect all movement history for this servo
  // history = [
  //   {
  //     timestamp: Date.now(),
  //     degrees: degrees
  //   }
  // ];

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.Standard;
  }

  priv.set(this, {
    history: history
  });

  Board.Controller.call(this, controller, opts);

  Object.defineProperties(this, {
    history: {
      get: function() {
        return history.slice(-5);
      }
    },
    last: {
      get: function() {
        return history[history.length - 1];
      }
    },
    position: {
      get: function() {
        return history.length ? history[history.length - 1].degrees : -1;
      }
    }
  });

  this.initialize(opts);

  // If "startAt" is defined and center is falsy
  // set servo to min or max degrees
  if (opts.startAt !== undefined) {
    this.startAt = opts.startAt;
    this.to(opts.startAt);
  }

  // If "center" true set servo to 90deg
  if (opts.center) {
    this.center();
  }

  if (opts.type === "continuous") {
    this.stop();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Servos"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Servos (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Servos)
- description and source-code
```javascript
function Servos(numsOrObjects) {
  if (!(this instanceof Servos)) {
    return new Servos(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Servo
  });

  Collection.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.ShiftRegister"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>ShiftRegister (opts)](#apidoc.element.nodebot-workshop.five.ShiftRegister)
- description and source-code
```javascript
function ShiftRegister(opts) {
  if (!(this instanceof ShiftRegister)) {
    return new ShiftRegister(opts);
  }

  if (Array.isArray(opts)) {
    // [Data, Clock, Latch, Reset]
    opts = {
      pins: {
        data: opts[0],
        clock: opts[1],
        latch: opts[2],
        reset: opts.length === 4 ? opts[3] : null,
      }
    };
  } else if (typeof opts.pins === "object" && Array.isArray(opts.pins)) {
    opts.pins = {
      data: opts.pins[0],
      clock: opts.pins[1],
      latch: opts.pins[2],
      reset: opts.pins.length === 4 ? opts.pins[3] : null,
    };
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  this.size = opts.size || 1;
  this.pins.reset = typeof opts.pins.reset !== "undefined" ? opts.pins.reset : null;

  var isAnode = typeof opts.isAnode !== "undefined" ? opts.isAnode : false;
  var clear = isAnode ? 255 : 0;
  var state = {
    isAnode: isAnode,
    value: new Array(this.size).fill(clear),
    encoded: encoded[isAnode ? "anode" : "cathode"],
    clear: clear,
  };

  priv.set(this, state);

  Object.defineProperties(this, {
    isAnode: {
      get: function() {
        return isAnode;
      }
    },
    value: {
      get: function() {
        return state.value;
      }
    },
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Sonar"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Sonar (opts)](#apidoc.element.nodebot-workshop.five.Sonar)
- description and source-code
```javascript
function Sonar(opts) {

  if (!(this instanceof Sonar)) {
    return new Sonar(opts);
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var device, state;

  // Sonar instance properties
  this.freq = opts.freq || 100;
  this.value = null;

  state = {
    last: 0,
    median: 0,
    samples: []
  };

  priv.set(this, state);

  if (typeof opts.device === "string") {
    device = Devices[opts.device];
  } else {
    device = opts.device;
  }

  if (typeof device === "undefined") {
    device = Devices.DEFAULT;
  }

  device.initialize.call(this, opts);

  if (!device.descriptor.inches) {
    device.descriptor.inches = {
      get: function() {
        return +(this.cm * 0.39).toFixed(2);
      }
    };
  }

  device.descriptor.in = device.descriptor.inches;

  Object.defineProperties(this, device.descriptor);

  // Throttle
  setInterval(function() {
    // Nothing read since previous interval
    if (state.samples.length === 0) {
      return;
    }

    state.median = state.samples.sort()[Math.floor(state.samples.length / 2)];
    this.value = state.median;

    this.emit("data", state.median);

    // If the state.median value for this interval is not the same as the
    // state.median value in the last interval, fire a "change" event.
    //
    if (state.last && state.median &&
      (state.median.toFixed(1) !== state.last.toFixed(1))) {
      this.emit("change", state.median);
    }

    // Store this media value for comparison
    // in next interval
    state.last = state.median;

    // Reset state.samples;
    state.samples.length = 0;
  }.bind(this), this.freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Stepper"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Stepper (opts)](#apidoc.element.nodebot-workshop.five.Stepper)
- description and source-code
```javascript
function Stepper(opts) {
  var state, params = [];

  if (!(this instanceof Stepper)) {
    return new Stepper(opts);
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  if (!isSupported(this.io)) {
    throw new Error(
      "Stepper is not supported"
    );
  }

  if (!opts.pins) {
    throw new Error(
      "Stepper requires a 'pins' object or array"
    );
  }

  if (!opts.stepsPerRev) {
    throw new Error(
      "Stepper requires a 'stepsPerRev' number value"
    );
  }

  steppers.set(this.board, steppers.get(this.board) || []);
  this.id = steppers.get(this.board).length;

  if (this.id >= MAXSTEPPERS) {
    throw new Error(
      "Stepper cannot exceed max steppers (" + MAXSTEPPERS + ")"
    );
  }

  // Convert an array of pins to the appropriate named pin
  if (Array.isArray(this.pins)) {
    if (this.pins.length === 2) {
      // Using an array of 2 pins requres a TYPE
      // to disambiguate DRIVER and TWO_WIRE
      if (!opts.type) {
        throw new Error(
          "Stepper requires a 'type' number value (DRIVER, TWO_WIRE)"
        );
      }
    }

    if (opts.type === Stepper.TYPE.DRIVER) {
      this.pins = {
        step: this.pins[0],
        dir: this.pins[1]
      };
    } else {
      this.pins = new MotorPins(this.pins);
    }
  }

  // Attempt to guess the type if none is provided
  if (!opts.type) {
    if (this.pins.dir) {
      opts.type = Stepper.TYPE.DRIVER;
    } else {
      if (this.pins.motor3) {
        opts.type = Stepper.TYPE.FOUR_WIRE;
      } else {
        opts.type = Stepper.TYPE.TWO_WIRE;
      }
    }
  }


  // Initial Stepper config params (same for all 3 types)
  params.push(this.id, opts.type, opts.stepsPerRev);


  if (opts.type === Stepper.TYPE.DRIVER) {
    if (typeof this.pins.dir === "undefined" ||
        typeof this.pins.step === "undefined") {
      throw new Error(
        "Stepper.TYPE.DRIVER expects: 'pins.dir', 'pins.step'"
      );
    }

    params.push(
      this.pins.dir, this.pins.step
    );
  }

  if (opts.type === Stepper.TYPE.TWO_WIRE) {
    if (typeof this.pins.motor1 === "undefined" ||
        typeof this.pins.motor2 === "undefined") {
      throw new Error(
        "Stepper.TYPE.TWO_WIRE expects: 'pins.motor1', 'pins.motor2'"
      );
    }

    params.push(
      this.pins.motor1, this.pins.motor2
    );
  }

  if (opts.type === Stepper.TYPE.FOUR_WIRE) {
    if (typeof this.pins.motor1 === "undefined" ||
        typeof this.pins.motor2 === "undefined" ||
        typeof this.pins.motor3 === "undefined" ||
        typeof this.pins.motor4 === "undefined") {
      throw new Error(
        "Stepper.TYPE.FOUR_WIRE expects: 'pins.motor1', 'pins.motor2', 'pins.motor3', 'pins.motor4'"
      );
    }

    params.push(
      this.pins.motor1, this.pins.motor2, this.pins.motor3, this.pins.motor4
    );
  }

  // Iterate the params and set each pin's mode to MODES.STEPPER
  // Params:
  // [deviceNum, type, stepsPerRev, dirOrMotor1Pin, stepOrMotor2Pin, motor3Pin, motor4Pin]
  // The first 3 are required, the remaining 2-4 will be pins
  params.slice(3).forEach(function(pin) {
    this.io.pinMode(pin, this.io.MODES.STEPPER);
  }, this);

  this.io.stepperConfig.apply(this.io, params);

  steppers.get(this.board).push(this);

  state = Step.PROPERTIES.reduce(function(state, key, i) {
    return (state[key] = typeof opts[key] !== "undefined" ? opts[key] : Step.DEFAULTS[i], state);
  }, {
    isRunning: false,
    type: opts.type,
    pins: this.pins
  });

  priv.set(this, state);

  Object.defineProperties(this, {
    type: {
      get: function() {
        return state.type;
      }
    },

    pins: {
      get: function() {
        return state.pins;
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Switch"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Switch (opts)](#apidoc.element.nodebot-workshop.five.Switch)
- description and source-code
```javascript
function Switch(opts) {

  if (!(this instanceof Switch)) {
    return new Switch(opts);
  }

  // Create a 5 ms debounce boundary on event triggers
  // this avoids button events firing on
  // press noise and false positives
  var trigger = Fn.debounce(function(key) {
    aliases[key].forEach(function(type) {
      this.emit(type, null);
    }, this);
  }, 5);

  // Resolve the default type to Normally Open
  opts.type = opts.type || "NO";

  // Is this instance Normally Open?
  var isNormallyOpen = opts.type === "NO";
  var raw = null;
  var invert = typeof opts.invert !== "undefined" ?
    opts.invert : (isNormallyOpen || false);

  // Logical Defaults
  var closeValue = 1;
  var openValue = 0;

  if (invert) {
    closeValue ^= 1;
    openValue ^= 1;
  }

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  this.io.pinMode(this.pin, this.io.MODES.INPUT);

  if (isNormallyOpen) {
    this.io.digitalWrite(this.pin, this.io.HIGH);
  }

  this.io.digitalRead(this.pin, function(data) {
    raw = data;

    trigger.call(this, this.isOpen ? "open" : "close");
  }.bind(this));

  Object.defineProperties(this, {
    value: {
      get: function() {
        return Number(this.isOpen);
      }
    },
    invert: {
      get: function() {
        return invert;
      },
      set: function(value) {
        invert = value;
        closeValue = invert ? 0 : 1;
        openValue = invert ? 1 : 0;
      }
    },
    closeValue: {
      get: function() {
        return closeValue;
      },
      set: function(value) {
        closeValue = value;
        openValue = value ^ 1;
      }
    },
    openValue: {
      get: function() {
        return openValue;
      },
      set: function(value) {
        openValue = value;
        closeValue = value ^ 1;
      }
    },
    isOpen: {
      get: function() {
        return raw === openValue;
      }
    },
    isClosed: {
      get: function() {
        return raw === closeValue;
      }
    },
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Switches"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Switches (numsOrObjects)](#apidoc.element.nodebot-workshop.five.Switches)
- description and source-code
```javascript
function Switches(numsOrObjects) {
  if (!(this instanceof Switches)) {
    return new Switches(numsOrObjects);
  }

  Object.defineProperty(this, "type", {
    value: Switch
  });

  Collection.Emitter.call(this, numsOrObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Temperature"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Temperature (opts)](#apidoc.element.nodebot-workshop.five.Temperature)
- description and source-code
```javascript
function Thermometer(opts) {

  if (!(this instanceof Thermometer)) {
    return new Thermometer(opts);
  }

  var controller = null;
  var last = null;
  var raw = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var freq = opts.freq || 25;

  // Analog Reference Voltage (default to board.io.aref || 5)
  this.aref = opts.aref || this.io.aref || 5;

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.ANALOG;
  }

  priv.set(this, {});

  Board.Controller.call(this, controller, opts);

  if (!this.toCelsius) {
    this.toCelsius = opts.toCelsius || function(x) {
      return x;
    };
  }

  var descriptors = {
    celsius: {
      get: function() {
        return this.toCelsius(raw);
      }
    },
    fahrenheit: {
      get: function() {
        return toFixed((this.celsius * 9 / 5) + 32, 2);
      }
    },
    kelvin: {
      get: function() {
        return toFixed(this.celsius + CELSIUS_TO_KELVIN, 2);
      }
    }
  };
  // Convenience aliases
  descriptors.C = descriptors.celsius;
  descriptors.F = descriptors.fahrenheit;
  descriptors.K = descriptors.kelvin;

  Object.defineProperties(this, descriptors);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  setInterval(function() {
    if (raw == null) {
      return;
    }

    var data = {};
    data.C = data.celsius = this.celsius;
    data.F = data.fahrenheit = this.fahrenheit;
    data.K = data.kelvin = this.kelvin;

    this.emit("data", data);

    if (this.celsius !== last) {
      last = this.celsius;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Thermometer"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Thermometer (opts)](#apidoc.element.nodebot-workshop.five.Thermometer)
- description and source-code
```javascript
function Thermometer(opts) {

  if (!(this instanceof Thermometer)) {
    return new Thermometer(opts);
  }

  var controller = null;
  var last = null;
  var raw = null;

  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var freq = opts.freq || 25;

  // Analog Reference Voltage (default to board.io.aref || 5)
  this.aref = opts.aref || this.io.aref || 5;

  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.ANALOG;
  }

  priv.set(this, {});

  Board.Controller.call(this, controller, opts);

  if (!this.toCelsius) {
    this.toCelsius = opts.toCelsius || function(x) {
      return x;
    };
  }

  var descriptors = {
    celsius: {
      get: function() {
        return this.toCelsius(raw);
      }
    },
    fahrenheit: {
      get: function() {
        return toFixed((this.celsius * 9 / 5) + 32, 2);
      }
    },
    kelvin: {
      get: function() {
        return toFixed(this.celsius + CELSIUS_TO_KELVIN, 2);
      }
    }
  };
  // Convenience aliases
  descriptors.C = descriptors.celsius;
  descriptors.F = descriptors.fahrenheit;
  descriptors.K = descriptors.kelvin;

  Object.defineProperties(this, descriptors);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {
      raw = data;
    });
  }

  setInterval(function() {
    if (raw == null) {
      return;
    }

    var data = {};
    data.C = data.celsius = this.celsius;
    data.F = data.fahrenheit = this.fahrenheit;
    data.K = data.kelvin = this.kelvin;

    this.emit("data", data);

    if (this.celsius !== last) {
      last = this.celsius;
      this.emit("change", data);
    }
  }.bind(this), freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Touchpad"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Touchpad (opts)](#apidoc.element.nodebot-workshop.five.Touchpad)
- description and source-code
```javascript
function Keypad(opts) {

  if (!(this instanceof Keypad)) {
    return new Keypad(opts);
  }

  // Initialize a Device instance on a Board
  Board.Component.call(
    this, opts = Board.Options(opts)
  );

  var raw = null;
  var controller = null;
  var state = {
    touches: null,
    timeout: null,
    length: null,
    keys: null,
    mapping: null,
    holdtime: null,
  };

  var trigger = Fn.debounce(function(type, value) {
    var event = {
      type: type,
      which: value,
      timestamp: Date.now()
    };
    aliases[type].forEach(function(type) {
      this.emit(type, event);
    }, this);

    this.emit("change", Object.assign({}, event));
  }, 5);


  if (opts.controller && typeof opts.controller === "string") {
    controller = Controllers[opts.controller.toUpperCase()];
  } else {
    controller = opts.controller;
  }

  if (controller == null) {
    controller = Controllers.ANALOG;
  }

  Board.Controller.call(this, controller, opts);

  state.holdtime = opts.holdtime ? opts.holdtime : 500;

  priv.set(this, state);

  if (typeof this.initialize === "function") {
    this.initialize(opts, function(data) {

      raw = data;

      var now = Date.now();
      var indices = this.toIndices(data);
      var kLength = state.length;

      var lists = {
        down: [],
        hold: [],
        up: [],
      };

      var target = null;
      var alias = null;

      for (var k = 0; k < kLength; k++) {
        alias = this.toAlias(k);

        if (indices.includes(k)) {
          if (state.touches[k].value === 0) {

            state.touches[k].timeout = now + state.holdtime;
            lists.down.push(alias);

          } else if (state.touches[k].value === 1) {
            if (state.touches[k].timeout !== null && now > state.touches[k].timeout) {
              state.touches[k].timeout = now + state.holdtime;
              lists.hold.push(alias);
            }
          }

          state.touches[k].value = 1;
        } else {
          if (state.touches[k].value === 1) {
            state.touches[k].timeout = null;
            lists.up.push(alias);
          }
          state.touches[k].value = 0;
        }
        target = null;
        alias = null;
      }

      Object.keys(lists).forEach(function(key) {
        var list = lists[key];

        if (list.length) {
          trigger.call(this, key, list);
        }
      }, this);
    }.bind(this));
  }

  Object.defineProperties(this, {
    isMultitouch: {
      get: function() {
        return state.isMultitouch;
      }
    },
    value: {
      get: function() {
        return raw;
      }
    },
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.Wii"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>Wii (opts)](#apidoc.element.nodebot-workshop.five.Wii)
- description and source-code
```javascript
function Wii(opts) {

  if (!(this instanceof Wii)) {
    return new Wii(opts);
  }

  Board.Component.call(this, opts);

  // Derive device definition from Devices
  var device = Devices[opts.device];
  var address = device.address;
  var bytes = device.bytes;
  var delay = device.delay;
  var data = device.data.bind(this);
  var setup = device.setup;
  var preread = device.preread;

  // Wii controller instance properties
  this.freq = opts.freq || 100;

  // Button instance properties
  this.holdtime = opts.holdtime || 500;
  this.threshold = opts.threshold || 10;

  // Initialize components
  device.initialize.call(this);

  // Set initial "last data" byte array
  last.set(this, [0, 0, 0, 0, 0, 0, 0]);

  // Set up I2C data connection
  this.io.i2cConfig(opts);

  // Iterate and write each set of setup instructions
  setup.forEach(function(bytes) {
    this.io.i2cWrite(address, bytes);
  }, this);

  // Unthrottled i2c read request loop
  setInterval(function() {

    // Send this command to get all sensor data and store into
    // the 6-byte register within Wii controller.
    // This must be execute before reading data from the Wii.

    // Iterate and write each set of setup instructions
    preread.forEach(function(bytes) {
      this.io.i2cWrite(address, bytes);
    }, this);


    // Request six bytes of data from the controller
    this.io.i2cReadOnce(address, bytes, data);

    // Use the high-frequency data read loop as the change event
    // emitting loop. This drastically improves change event
    // frequency and sensitivity
    //
    // Emit change events if any delta is greater than
    // the threshold

    // RVL-005 does not have a read method at this time.
    if (typeof device.read !== "undefined") {
      device.read.call(this);
    }
  }.bind(this), delay || this.freq);

  // Throttled "read" event loop
  setInterval(function() {
    var event = new Board.Event({
      target: this
    });

    this.emit("data", event);

  }.bind(this), this.freq);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.five.spyOn"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.five.</span>spyOn ()](#apidoc.element.nodebot-workshop.five.spyOn)
- description and source-code
```javascript
spyOn = function () {
  var args = Array.prototype.slice.call(arguments)

  args.forEach(function (name) {
    this[name] = createSpy(this[name])
  }, this)

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodebot-workshop.io_stub"></a>[module nodebot-workshop.io_stub](#apidoc.module.nodebot-workshop.io_stub)

#### <a name="apidoc.element.nodebot-workshop.io_stub.Board"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.io_stub.</span>Board (port, callback)](#apidoc.element.nodebot-workshop.io_stub.Board)
- description and source-code
```javascript
Board = function (port, callback) {
  if(module.exports.singleton) {
    throw new Error('Board already created');
  }

  var singleton = new IO(port, callback);

  // spy on every IO method
  for(var key in singleton) {
    if(singleton[key] instanceof Function) {
      singleton[key] = sinon.spy(singleton[key]);
    }
  }

  // we're going to interrogate the singleton during solution verification
  module.exports.singleton = singleton;

  return singleton;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodebot-workshop.serialport_stub"></a>[module nodebot-workshop.serialport_stub](#apidoc.module.nodebot-workshop.serialport_stub)

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.serialport_stub"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.</span>serialport_stub {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub.serialport_stub)
- description and source-code
```javascript
SerialPort
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledOn"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledOn ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledOn)
- description and source-code
```javascript
alwaysCalledOn = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWith"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWith ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWith)
- description and source-code
```javascript
alwaysCalledWith = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithExactly"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWithExactly ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithExactly)
- description and source-code
```javascript
alwaysCalledWithExactly = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithMatch"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWithMatch ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithMatch)
- description and source-code
```javascript
alwaysCalledWithMatch = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithNew"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysCalledWithNew ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysCalledWithNew)
- description and source-code
```javascript
alwaysCalledWithNew = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.alwaysReturned"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysReturned ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysReturned)
- description and source-code
```javascript
alwaysReturned = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.alwaysThrew"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>alwaysThrew ()](#apidoc.element.nodebot-workshop.serialport_stub.alwaysThrew)
- description and source-code
```javascript
alwaysThrew = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.callArg"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArg ()](#apidoc.element.nodebot-workshop.serialport_stub.callArg)
- description and source-code
```javascript
callArg = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.callArgOn"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArgOn ()](#apidoc.element.nodebot-workshop.serialport_stub.callArgOn)
- description and source-code
```javascript
callArgOn = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.callArgOnWith"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArgOnWith ()](#apidoc.element.nodebot-workshop.serialport_stub.callArgOnWith)
- description and source-code
```javascript
callArgOnWith = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.callArgWith"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>callArgWith ()](#apidoc.element.nodebot-workshop.serialport_stub.callArgWith)
- description and source-code
```javascript
callArgWith = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.calledAfter"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledAfter (spyFn)](#apidoc.element.nodebot-workshop.serialport_stub.calledAfter)
- description and source-code
```javascript
function calledAfter(spyFn) {
    if (!this.called || !spyFn.called) {
        return false;
    }

    return this.callIds[this.callCount - 1] > spyFn.callIds[spyFn.callCount - 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.calledBefore"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledBefore (spyFn)](#apidoc.element.nodebot-workshop.serialport_stub.calledBefore)
- description and source-code
```javascript
function calledBefore(spyFn) {
    if (!this.called) {
        return false;
    }

    if (!spyFn.called) {
        return true;
    }

    return this.callIds[0] < spyFn.callIds[spyFn.callIds.length - 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.calledOn"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledOn ()](#apidoc.element.nodebot-workshop.serialport_stub.calledOn)
- description and source-code
```javascript
calledOn = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.calledWith"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWith ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWith)
- description and source-code
```javascript
calledWith = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.calledWithExactly"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWithExactly ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWithExactly)
- description and source-code
```javascript
calledWithExactly = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.calledWithMatch"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWithMatch ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWithMatch)
- description and source-code
```javascript
calledWithMatch = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.calledWithNew"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>calledWithNew ()](#apidoc.element.nodebot-workshop.serialport_stub.calledWithNew)
- description and source-code
```javascript
calledWithNew = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.getCall"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>getCall (i)](#apidoc.element.nodebot-workshop.serialport_stub.getCall)
- description and source-code
```javascript
function getCall(i) {
    if (i < 0 || i >= this.callCount) {
        return null;
    }

    return sinon.spyCall(this, this.thisValues[i], this.args[i],
                            this.returnValues[i], this.exceptions[i],
                            this.callIds[i], this.stacks[i]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.getCalls"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>getCalls ()](#apidoc.element.nodebot-workshop.serialport_stub.getCalls)
- description and source-code
```javascript
getCalls = function () {
    var calls = [];
    var i;

    for (i = 0; i < this.callCount; i++) {
        calls.push(this.getCall(i));
    }

    return calls;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.instantiateFake"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>instantiateFake (func, spyLength)](#apidoc.element.nodebot-workshop.serialport_stub.instantiateFake)
- description and source-code
```javascript
function create(func, spyLength) {
    var name;

    if (typeof func !== "function") {
        func = function () { };
    } else {
        name = sinon.functionName(func);
    }

    if (!spyLength) {
        spyLength = func.length;
    }

    var proxy = createProxy(func, spyLength);

    sinon.extend(proxy, spy);
    delete proxy.create;
    sinon.extend(proxy, func);

    proxy.reset();
    proxy.prototype = func.prototype;
    proxy.displayName = name || "spy";
    proxy.toString = sinon.functionToString;
    proxy.instantiateFake = sinon.spy.create;
    proxy.id = "spy#" + uuid++;

    return proxy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.invoke"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>invoke (func, thisValue, args)](#apidoc.element.nodebot-workshop.serialport_stub.invoke)
- description and source-code
```javascript
function invoke(func, thisValue, args) {
    var matching = matchingFake(this.fakes, args);
    var exception, returnValue;

    incrementCallCount.call(this);
    push.call(this.thisValues, thisValue);
    push.call(this.args, args);
    push.call(this.callIds, callId++);

    // Make call properties available from within the spied function:
    createCallProperties.call(this);

    try {
        this.invoking = true;

        if (matching) {
            returnValue = matching.invoke(func, thisValue, args);
        } else {
            returnValue = (this.func || func).apply(thisValue, args);
        }

        var thisCall = this.getCall(this.callCount - 1);
        if (thisCall.calledWithNew() && typeof returnValue !== "object") {
            returnValue = thisValue;
        }
    } catch (e) {
        exception = e;
    } finally {
        delete this.invoking;
    }

    push.call(this.exceptions, exception);
    push.call(this.returnValues, returnValue);
    push.call(this.stacks, new Error().stack);

    // Make return value and exception available in the calls:
    createCallProperties.call(this);

    if (exception !== undefined) {
        throw exception;
    }

    return returnValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.invokeCallback"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>invokeCallback ()](#apidoc.element.nodebot-workshop.serialport_stub.invokeCallback)
- description and source-code
```javascript
invokeCallback = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.list"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>list {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub.list)
- description and source-code
```javascript
stub
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.matches"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>matches (args, strict)](#apidoc.element.nodebot-workshop.serialport_stub.matches)
- description and source-code
```javascript
matches = function (args, strict) {
    var margs = this.matchingAguments;

    if (margs.length <= args.length &&
        sinon.deepEqual(margs, args.slice(0, margs.length))) {
        return !strict || margs.length === args.length;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.named"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>named (name)](#apidoc.element.nodebot-workshop.serialport_stub.named)
- description and source-code
```javascript
function named(name) {
    this.displayName = name;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.neverCalledWith"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>neverCalledWith ()](#apidoc.element.nodebot-workshop.serialport_stub.neverCalledWith)
- description and source-code
```javascript
neverCalledWith = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.neverCalledWithMatch"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>neverCalledWithMatch ()](#apidoc.element.nodebot-workshop.serialport_stub.neverCalledWithMatch)
- description and source-code
```javascript
neverCalledWithMatch = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.printf"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>printf (format)](#apidoc.element.nodebot-workshop.serialport_stub.printf)
- description and source-code
```javascript
printf = function (format) {
    var spyInstance = this;
    var args = slice.call(arguments, 1);
    var formatter;

    return (format || "").replace(/%(.)/g, function (match, specifyer) {
        formatter = spyApi.formatters[specifyer];

        if (typeof formatter === "function") {
            return formatter.call(null, spyInstance, args);
        } else if (!isNaN(parseInt(specifyer, 10))) {
            return sinon.format(args[specifyer - 1]);
        }

        return "%" + specifyer;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.reset"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>reset ()](#apidoc.element.nodebot-workshop.serialport_stub.reset)
- description and source-code
```javascript
reset = function () {
    if (this.invoking) {
        var err = new Error("Cannot reset Sinon function while invoking it. " +
                            "Move the call to .reset outside of the callback.");
        err.name = "InvalidResetException";
        throw err;
    }

    this.called = false;
    this.notCalled = true;
    this.calledOnce = false;
    this.calledTwice = false;
    this.calledThrice = false;
    this.callCount = 0;
    this.firstCall = null;
    this.secondCall = null;
    this.thirdCall = null;
    this.lastCall = null;
    this.args = [];
    this.returnValues = [];
    this.thisValues = [];
    this.exceptions = [];
    this.callIds = [];
    this.stacks = [];
    if (this.fakes) {
        for (var i = 0; i < this.fakes.length; i++) {
            this.fakes[i].reset();
        }
    }

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.returned"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>returned ()](#apidoc.element.nodebot-workshop.serialport_stub.returned)
- description and source-code
```javascript
returned = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.spyCall"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>spyCall {{signature}}](#apidoc.element.nodebot-workshop.serialport_stub.spyCall)
- description and source-code
```javascript
:(
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.threw"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>threw ()](#apidoc.element.nodebot-workshop.serialport_stub.threw)
- description and source-code
```javascript
threw = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.toString"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>toString ()](#apidoc.element.nodebot-workshop.serialport_stub.toString)
- description and source-code
```javascript
function toString() {
    if (this.getCall && this.callCount) {
        var thisValue,
            prop;
        var i = this.callCount;

        while (i--) {
            thisValue = this.getCall(i).thisValue;

            for (prop in thisValue) {
                if (thisValue[prop] === this) {
                    return prop;
                }
            }
        }
    }

    return this.displayName || "sinon fake";
}
```
- example usage
```shell
...
var resolve = function (error, callback) {
  if (error) {
    if (error instanceof TestError) {
      // assertion failure
      afterTest(exercise, false, callback)
    } else {
      // other failure
      console.error(error.stack ? error.stack : error.toString())
      callback(error)
    }
  } else {
    afterTest(exercise, true, callback)
  }
}
...
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.withArgs"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>withArgs ()](#apidoc.element.nodebot-workshop.serialport_stub.withArgs)
- description and source-code
```javascript
withArgs = function () {
    var args = slice.call(arguments);

    if (this.fakes) {
        var match = matchingFake(this.fakes, args, true);

        if (match) {
            return match;
        }
    } else {
        this.fakes = [];
    }

    var original = this;
    var fake = this.instantiateFake();
    fake.matchingAguments = args;
    fake.parent = this;
    push.call(this.fakes, fake);

    fake.withArgs = function () {
        return original.withArgs.apply(original, arguments);
    };

    for (var i = 0; i < this.args.length; i++) {
        if (fake.matches(this.args[i])) {
            incrementCallCount.call(fake);
            push.call(fake.thisValues, this.thisValues[i]);
            push.call(fake.args, this.args[i]);
            push.call(fake.returnValues, this.returnValues[i]);
            push.call(fake.exceptions, this.exceptions[i]);
            push.call(fake.callIds, this.callIds[i]);
        }
    }
    createCallProperties.call(fake);

    return fake;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.yield"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yield ()](#apidoc.element.nodebot-workshop.serialport_stub.yield)
- description and source-code
```javascript
yield = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.yieldOn"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yieldOn ()](#apidoc.element.nodebot-workshop.serialport_stub.yieldOn)
- description and source-code
```javascript
yieldOn = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.yieldTo"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yieldTo ()](#apidoc.element.nodebot-workshop.serialport_stub.yieldTo)
- description and source-code
```javascript
yieldTo = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodebot-workshop.serialport_stub.yieldToOn"></a>[function <span class="apidocSignatureSpan">nodebot-workshop.serialport_stub.</span>yieldToOn ()](#apidoc.element.nodebot-workshop.serialport_stub.yieldToOn)
- description and source-code
```javascript
yieldToOn = function () {
    if (!this.called) {
        if (notCalled) {
            return notCalled.apply(this, arguments);
        }
        return false;
    }

    var currentCall;
    var matches = 0;

    for (var i = 0, l = this.callCount; i < l; i += 1) {
        currentCall = this.getCall(i);

        if (currentCall[actual || method].apply(currentCall, arguments)) {
            matches += 1;

            if (matchAny) {
                return true;
            }
        }
    }

    return matches === this.callCount;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
