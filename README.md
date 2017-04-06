# api documentation for  [deployd (v0.8.9)](https://github.com/deployd/deployd#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-deployd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-deployd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-deployd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-deployd)
#### the simplest way to build realtime APIs for web and mobile apps

[![NPM](https://nodei.co/npm/deployd.png?downloads=true)](https://www.npmjs.com/package/deployd)

[![apidoc](https://npmdoc.github.io/node-npmdoc-deployd/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-deployd_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-deployd/build/apidoc.html)

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
            "name": "ritch",
            "email": "skawful@gmail.com"
        },
        {
            "name": "jeffbcross",
            "email": "middlefloor@gmail.com"
        },
        {
            "name": "nicolasrtt",
            "email": "nicolas@ritouet.com"
        }
    ],
    "name": "deployd",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "url": "git://github.com/deployd/deployd.git"
    },
    "scripts": {
        "test": "mocha --timeout 5000 && cd test-app && node runtests.js"
    },
    "version": "0.8.9"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module deployd](#apidoc.module.deployd)
1.  [function <span class="apidocSignatureSpan">deployd.</span>attach (httpServer, options)](#apidoc.element.deployd.attach)
1.  [function <span class="apidocSignatureSpan">deployd.</span>context (resource, req, res, server)](#apidoc.element.deployd.context)
1.  [function <span class="apidocSignatureSpan">deployd.</span>keys (path)](#apidoc.element.deployd.keys)
1.  [function <span class="apidocSignatureSpan">deployd.</span>resource (name, options)](#apidoc.element.deployd.resource)
1.  [function <span class="apidocSignatureSpan">deployd.</span>router (resources, server)](#apidoc.element.deployd.router)
1.  [function <span class="apidocSignatureSpan">deployd.</span>script (src, path)](#apidoc.element.deployd.script)
1.  [function <span class="apidocSignatureSpan">deployd.</span>server (options)](#apidoc.element.deployd.server)
1.  object <span class="apidocSignatureSpan">deployd.</span>ayepromise
1.  object <span class="apidocSignatureSpan">deployd.</span>config_loader
1.  object <span class="apidocSignatureSpan">deployd.</span>context.prototype
1.  object <span class="apidocSignatureSpan">deployd.</span>db
1.  object <span class="apidocSignatureSpan">deployd.</span>internal_client
1.  object <span class="apidocSignatureSpan">deployd.</span>keys.prototype
1.  object <span class="apidocSignatureSpan">deployd.</span>resource.prototype
1.  object <span class="apidocSignatureSpan">deployd.</span>router.prototype
1.  object <span class="apidocSignatureSpan">deployd.</span>script.prototype
1.  object <span class="apidocSignatureSpan">deployd.</span>server.prototype
1.  object <span class="apidocSignatureSpan">deployd.</span>session

#### [module deployd.ayepromise](#apidoc.module.deployd.ayepromise)
1.  [function <span class="apidocSignatureSpan">deployd.ayepromise.</span>defer ()](#apidoc.element.deployd.ayepromise.defer)

#### [module deployd.config_loader](#apidoc.module.deployd.config_loader)
1.  [function <span class="apidocSignatureSpan">deployd.config_loader.</span>loadConfig (basepath, server, fn)](#apidoc.element.deployd.config_loader.loadConfig)

#### [module deployd.context](#apidoc.module.deployd.context)
1.  [function <span class="apidocSignatureSpan">deployd.</span>context (resource, req, res, server)](#apidoc.element.deployd.context.context)

#### [module deployd.context.prototype](#apidoc.module.deployd.context.prototype)
1.  [function <span class="apidocSignatureSpan">deployd.context.prototype.</span>done (err, res)](#apidoc.element.deployd.context.prototype.done)
1.  [function <span class="apidocSignatureSpan">deployd.context.prototype.</span>end ()](#apidoc.element.deployd.context.prototype.end)

#### [module deployd.db](#apidoc.module.deployd.db)
1.  [function <span class="apidocSignatureSpan">deployd.db.</span>Db (options)](#apidoc.element.deployd.db.Db)
1.  [function <span class="apidocSignatureSpan">deployd.db.</span>Store (namespace, db)](#apidoc.element.deployd.db.Store)
1.  [function <span class="apidocSignatureSpan">deployd.db.</span>create (options)](#apidoc.element.deployd.db.create)

#### [module deployd.internal_client](#apidoc.module.deployd.internal_client)
1.  [function <span class="apidocSignatureSpan">deployd.internal_client.</span>build (server, session, stack, ctx)](#apidoc.element.deployd.internal_client.build)

#### [module deployd.keys](#apidoc.module.deployd.keys)
1.  [function <span class="apidocSignatureSpan">deployd.</span>keys (path)](#apidoc.element.deployd.keys.keys)

#### [module deployd.keys.prototype](#apidoc.module.deployd.keys.prototype)
1.  [function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>create (fn)](#apidoc.element.deployd.keys.prototype.create)
1.  [function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>generate ()](#apidoc.element.deployd.keys.prototype.generate)
1.  [function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>get (key, fn)](#apidoc.element.deployd.keys.prototype.get)
1.  [function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>getLocal (fn)](#apidoc.element.deployd.keys.prototype.getLocal)
1.  [function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>readFile (fn)](#apidoc.element.deployd.keys.prototype.readFile)
1.  [function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>writeFile (data, fn)](#apidoc.element.deployd.keys.prototype.writeFile)

#### [module deployd.resource](#apidoc.module.deployd.resource)
1.  [function <span class="apidocSignatureSpan">deployd.</span>resource (name, options)](#apidoc.element.deployd.resource.resource)
1.  [function <span class="apidocSignatureSpan">deployd.resource.</span>super_ ()](#apidoc.element.deployd.resource.super_)
1.  [function <span class="apidocSignatureSpan">deployd.resource.</span>toJSON ()](#apidoc.element.deployd.resource.toJSON)
1.  object <span class="apidocSignatureSpan">deployd.resource.</span>external

#### [module deployd.resource.prototype](#apidoc.module.deployd.resource.prototype)
1.  boolean <span class="apidocSignatureSpan">deployd.resource.prototype.</span>__resource__
1.  boolean <span class="apidocSignatureSpan">deployd.resource.prototype.</span>clientGeneration
1.  [function <span class="apidocSignatureSpan">deployd.resource.prototype.</span>handle (ctx, next)](#apidoc.element.deployd.resource.prototype.handle)
1.  [function <span class="apidocSignatureSpan">deployd.resource.prototype.</span>load (fn)](#apidoc.element.deployd.resource.prototype.load)
1.  [function <span class="apidocSignatureSpan">deployd.resource.prototype.</span>parse (url)](#apidoc.element.deployd.resource.prototype.parse)
1.  object <span class="apidocSignatureSpan">deployd.resource.prototype.</span>clientGenerationExec
1.  object <span class="apidocSignatureSpan">deployd.resource.prototype.</span>clientGenerationGet

#### [module deployd.router](#apidoc.module.deployd.router)
1.  [function <span class="apidocSignatureSpan">deployd.</span>router (resources, server)](#apidoc.element.deployd.router.router)

#### [module deployd.router.prototype](#apidoc.module.deployd.router.prototype)
1.  [function <span class="apidocSignatureSpan">deployd.router.prototype.</span>generateRegex (path)](#apidoc.element.deployd.router.prototype.generateRegex)
1.  [function <span class="apidocSignatureSpan">deployd.router.prototype.</span>matchResources (url)](#apidoc.element.deployd.router.prototype.matchResources)
1.  [function <span class="apidocSignatureSpan">deployd.router.prototype.</span>route (req, res)](#apidoc.element.deployd.router.prototype.route)

#### [module deployd.script](#apidoc.module.deployd.script)
1.  [function <span class="apidocSignatureSpan">deployd.</span>script (src, path)](#apidoc.element.deployd.script.script)
1.  [function <span class="apidocSignatureSpan">deployd.script.</span>load (path, fn)](#apidoc.element.deployd.script.load)

#### [module deployd.script.prototype](#apidoc.module.deployd.script.prototype)
1.  [function <span class="apidocSignatureSpan">deployd.script.prototype.</span>getFunction (key)](#apidoc.element.deployd.script.prototype.getFunction)
1.  [function <span class="apidocSignatureSpan">deployd.script.prototype.</span>run (ctx, domain, fn)](#apidoc.element.deployd.script.prototype.run)
1.  [function <span class="apidocSignatureSpan">deployd.script.prototype.</span>runWithContext (context)](#apidoc.element.deployd.script.prototype.runWithContext)

#### [module deployd.server](#apidoc.module.deployd.server)
1.  [function <span class="apidocSignatureSpan">deployd.</span>server (options)](#apidoc.element.deployd.server.server)
1.  [function <span class="apidocSignatureSpan">deployd.server.</span>super_ (requestListener)](#apidoc.element.deployd.server.super_)

#### [module deployd.server.prototype](#apidoc.module.deployd.server.prototype)
1.  [function <span class="apidocSignatureSpan">deployd.server.prototype.</span>createStore (namespace)](#apidoc.element.deployd.server.prototype.createStore)
1.  [function <span class="apidocSignatureSpan">deployd.server.prototype.</span>handleRequest (req, res)](#apidoc.element.deployd.server.prototype.handleRequest)
1.  [function <span class="apidocSignatureSpan">deployd.server.prototype.</span>listen (port, host)](#apidoc.element.deployd.server.prototype.listen)
1.  [function <span class="apidocSignatureSpan">deployd.server.prototype.</span>route (req, res)](#apidoc.element.deployd.server.prototype.route)

#### [module deployd.session](#apidoc.module.deployd.session)
1.  [function <span class="apidocSignatureSpan">deployd.session.</span>SessionStore (namespace, db, sockets, options)](#apidoc.element.deployd.session.SessionStore)



# <a name="apidoc.module.deployd"></a>[module deployd](#apidoc.module.deployd)

#### <a name="apidoc.element.deployd.attach"></a>[function <span class="apidocSignatureSpan">deployd.</span>attach (httpServer, options)](#apidoc.element.deployd.attach)
- description and source-code
```javascript
function attach(httpServer, options) {
  var server = process.server = httpServer;

  // defaults
  server.options = options = _.extend({
    db: {port: 27017, host: '127.0.0.1', name: 'deployd'}
  }, options);

  debug('started with options %j', options);

  // an object to map a server to its stores
  server.stores = {};

  // back all memory stores with a db
  server.db = db.create(options.db);

  // use socket io for a session based realtime channel
  if (options.socketIo && options.socketIo.sockets) {
    server.sockets = options.socketIo.sockets;
  } else {
    var socketIo = require('socket.io').listen(server, {'log level':0});
    server.sockets = socketIo.sockets;
  }

  // persist sessions in a store
  server.sessions = new SessionStore('sessions', server.db, server.sockets, options.sessions);

  // persist keys in a store
  server.keys = new Keys();

  server.handleRequest = function handleRequest(req, res) {
    // dont handle socket.io requests
    if(req.url.indexOf('/socket.io/') === 0) return;
    debug('%s %s', req.method, req.url);

    // add utilites to req and res
    setupReqRes(server.options, req, res, function(err, next) {
      if(err) return res.end(err.message);

      var authToken, usesBearerAuth = false;
      if (req.headers && req.headers.authorization) {
        var parts = req.headers.authorization.split(' ');
        var scheme = parts[0]
        , credentials = parts[1];

        if (/^Bearer$/i.test(scheme)) {
          authToken = credentials;
          usesBearerAuth = true;
        }
      }

      server.sessions.createSession(authToken || req.cookies.get('sid'), function(err, session) {

        if(err) {
          debug('session error', err, session);
          throw err;
        } else {
          if (!usesBearerAuth) {
            // (re)set the session id cookie if we're not using Authorization Bearer
            req.cookies.set('sid', session.sid);
          }
          req.session = session;

          var root = req.headers['dpd-ssh-key'] || req.cookies.get('DpdSshKey');

          if (server.options.env === 'development') {
            if (root) {
              req.isRoot = true;
            }
            server.route(req, res);
          } else if (root) {
            // all root requests
            // must be authenticated
            debug('authenticating', root);
            server.keys.get(root, function(err, key) {
              if(err) throw err;
              if(key) req.isRoot = true;
              debug('is root?', session.isRoot);
              server.route(req, res);
            });
          } else {
            // normal route
            server.route(req, res);
          }
        }
      });
    });
  };


  var serverpath = server.options.server_dir || fs.realpathSync('./');

  // mkdir resourcesPath if not exists
  var resourcesPath = path.join(serverpath, 'resources');
  // use sync functions, as only run once when server start-up
  if (!fs.existsSync(resourcesPath)) {
    fs.mkdirSync(resourcesPath);
  }

  server.route = function route(req, res) {
    config.loadConfig(serverpath, server, function(err, resourcesInstances) {
      if (err) throw err;
      server.resources = resourcesInstances;
      var router = server.router = new Router(resourcesInstances, server);
      router.route(req, res);
    });
  };

  // lazy-load OR bootstrap load?
  // config.loadConfig('./', server, function(err, resourcesInstances) {
  //     if (err) {
  //         console.error();
  //         console.error("Error loading resources: ");
  //         console.error(err.stack || err);
  //         process.exit(1);
  //     } else {
  //         server.resources = resourcesInstances;
  //         var router = server.router = new Router(resourcesInstances, server);
  //     }
  // });


  server.on('request:error', function (err, req, res) {
    console.error();
    console.error(req.method, req.url, err.stack || err);
    process.exit(1);
  });




  /**
  * Create a new 'Store' for persisting data using the database info that was passed to the server when it was create ...
```
- example usage
```shell
...
*   var http = require('http');
*   var express = require('express');
*   var app = express();
*   var server = http.createServer(app);
*   var io = require('socket.io').listen(server, {'log level': 0});
*
*   var deployd = require('deployd')
*   deployd.attach(server, {socketIo: io, env: ENV, db:{host:'localhost', port:27015, name:'my-db'} } );
*   app.use(server.handleRequest);
*
*   server.listen();
*
* @param {Object} options
* @return {HttpServer}
*/
...
```

#### <a name="apidoc.element.deployd.context"></a>[function <span class="apidocSignatureSpan">deployd.</span>context (resource, req, res, server)](#apidoc.element.deployd.context)
- description and source-code
```javascript
function Context(resource, req, res, server) {
  var ctx = this;
  this.url = req.url.slice(resource.path.length).split('?')[0];
  if (this.url.indexOf('/') !== 0) this.url = '/' + this.url;

  this.req = req;
  this.res = res;
  this.body = req.body;
  this.query = req.query || {};
  this.server = server;
  this.session = req.session;
  this.method = req && req.method;

  // always bind done to this
  var done = this.done;
  this.done = function() {
    done.apply(ctx, arguments);
  };

  if ((this.query && typeof this.query.$limitRecursion !== 'undefined') || (this.body && typeof this.body.$limitRecursion !== 'undefined
')) {
    var recursionLimit = this.query.$limitRecursion || this.body.$limitRecursion || 0;
    req.stack = req.stack || [];
    req.stack.recursionLimit = recursionLimit;
  }

  this.dpd = internalClient.build(server, req.session, req.stack, ctx);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.keys"></a>[function <span class="apidocSignatureSpan">deployd.</span>keys (path)](#apidoc.element.deployd.keys)
- description and source-code
```javascript
function Keys(path) {
  this.path = path || '.dpd/keys.json';
}
```
- example usage
```shell
...
    }
    fn(err, result);
  });
};

function loadTypes(fn) {
  _loadTypes(function(defaults, types) {
    Object.keys(types).forEach(function(key) {
      defaults[key] = types[key];
    });
    types = defaults;
    fn(null, types);
  });
}
...
```

#### <a name="apidoc.element.deployd.resource"></a>[function <span class="apidocSignatureSpan">deployd.</span>resource (name, options)](#apidoc.element.deployd.resource)
- description and source-code
```javascript
function Resource(name, options) {
  EventEmitter.call(this);
  this.name = name;
  this.path = '/' + name;
  options = this.options = options || {};
  this.config = options.config || {};
  this.events = {};
  var instance = this;
  if(this.constructor.external) {
    instance.external = {};
    Object.keys(this.constructor.external).forEach(function (key) {
      if(typeof instance.constructor.external[key] == 'function') {
        instance.external[key] = function () {
          instance.constructor.external[key].apply(instance, arguments);
        };
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.router"></a>[function <span class="apidocSignatureSpan">deployd.</span>router (resources, server)](#apidoc.element.deployd.router)
- description and source-code
```javascript
function Router(resources, server) {
  this.resources = resources || [];
  this.server = server;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.script"></a>[function <span class="apidocSignatureSpan">deployd.</span>script (src, path)](#apidoc.element.deployd.script)
- description and source-code
```javascript
function Script(src, path) {
  this.scriptSourceCode = src;
  this.path = path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.server"></a>[function <span class="apidocSignatureSpan">deployd.</span>server (options)](#apidoc.element.deployd.server)
- description and source-code
```javascript
function Server(options) {
  var server = process.server = this;
  http.Server.call(this);

  // defaults
  this.options = options = extend({
    port: 2403,
    db: {port: 27017, host: '127.0.0.1', name: 'deployd'}
  }, options);

  debug('started with options %j', options);

  // an object to map a server to its stores
  this.stores = {};

  // back all memory stores with a db
  this.db = db.create(options.db);

  var socketServer = io.listen(this, _.extend({
    'log level': 0
  }, (this.options.socketIo && this.options.socketIo.options) || {}));

  // use socket io for a session based realtime channel
  this.sockets = socketServer.sockets;

  if (this.options.socketIo && this.options.socketIo.adapter) {
    socketServer.adapter(this.options.socketIo.adapter);
  }

  // persist sessions in a store
  this.sessions = new SessionStore('sessions', this.db, this.sockets, options.sessions);

  // persist keys in a store
  this.keys = new Keys();

  this.on('request', server.handleRequest);

  server.on('request:error', function (err, req, res) {
    console.error();
    console.error(req.method, req.url, err.stack || err);
    process.exit(1);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.deployd.ayepromise"></a>[module deployd.ayepromise](#apidoc.module.deployd.ayepromise)

#### <a name="apidoc.element.deployd.ayepromise.defer"></a>[function <span class="apidocSignatureSpan">deployd.ayepromise.</span>defer ()](#apidoc.element.deployd.ayepromise.defer)
- description and source-code
```javascript
defer = function () {
    var state = PENDING,
        outcome,
        thenHandlers = [];

    var doSettle = function (settledState, value) {
        state = settledState;
        // persist for handlers registered after settling
        outcome = value;

        thenHandlers.forEach(function (then) {
            then.handle(state, outcome);
        });

        // Discard all references to handlers to be garbage collected
        thenHandlers = null;
    };

    var doFulfill = function (value) {
        doSettle(FULFILLED, value);
    };

    var doReject = function (error) {
        doSettle(REJECTED, error);
    };

    var registerThenHandler = function (onFulfilled, onRejected) {
        var thenHandler = aThenHandler(onFulfilled, onRejected);

        if (state === PENDING) {
            thenHandlers.push(thenHandler);
        } else {
            thenHandler.handle(state, outcome);
        }

        return thenHandler.promise;
    };

    var safelyResolveThenable = function (thenable) {
        // Either fulfill, reject or reject with error
        var onceWrapper = once();
        try {
            thenable(
                onceWrapper(transparentlyResolveThenablesAndSettle),
                onceWrapper(doReject)
            );
        } catch (e) {
            onceWrapper(doReject)(e);
        }
    };

    var transparentlyResolveThenablesAndSettle = function (value) {
        var thenable;

        try {
            thenable = getThenableIfExists(value);
        } catch (e) {
            doReject(e);
            return;
        }

        if (thenable) {
            safelyResolveThenable(thenable);
        } else {
            doFulfill(value);
        }
    };

    var onceWrapper = once();
    return {
        resolve: onceWrapper(transparentlyResolveThenablesAndSettle),
        reject: onceWrapper(doReject),
        promise: {
            then: registerThenHandler,
            fail: function (onRejected) {
                return registerThenHandler(null, onRejected);
            }
        }
    };
}
```
- example usage
```shell
...
if (typeof obj === "object" && typeof then === "function") {
    // Bind function back to it's object (so fan's of 'this' don't get sad)
    return function() { return then.apply(obj, arguments); };
}
    };

    var aThenHandler = function (onFulfilled, onRejected) {
var defer = ayepromise.defer();

var doHandlerCall = function (func, value) {
    setTimeout(function () {
        var returnValue;
        try {
            returnValue = func(value);
        } catch (e) {
...
```



# <a name="apidoc.module.deployd.config_loader"></a>[module deployd.config_loader](#apidoc.module.deployd.config_loader)

#### <a name="apidoc.element.deployd.config_loader.loadConfig"></a>[function <span class="apidocSignatureSpan">deployd.config_loader.</span>loadConfig (basepath, server, fn)](#apidoc.element.deployd.config_loader.loadConfig)
- description and source-code
```javascript
loadConfig = function (basepath, server, fn) {
  var resources = server.__resourceCache || [];

  if (resources.length) {
    debug("Loading from cache");
    fn(null, resources);
    return;
  }

  var getTypes = async.memoize(loadTypes);

  async.waterfall([
      async.apply(loadResourceDir, basepath)
    , async.apply(loadResources, getTypes, basepath, server)
    , async.apply(addInternalResources, server, basepath)
  ], function(err, result) {
    if (server.options && server.options.env !== 'development') {
      server.__resourceCache = result;
    }
    fn(err, result);
  });
}
```
- example usage
```shell
...
var resourcesPath = path.join(serverpath, 'resources');
// use sync functions, as only run once when server start-up
if (!fs.existsSync(resourcesPath)) {
  fs.mkdirSync(resourcesPath);
}

server.route = function route(req, res) {
  config.loadConfig(serverpath, server, function(err, resourcesInstances) {
    if (err) throw err;
    server.resources = resourcesInstances;
    var router = server.router = new Router(resourcesInstances, server);
    router.route(req, res);
  });
};
...
```



# <a name="apidoc.module.deployd.context"></a>[module deployd.context](#apidoc.module.deployd.context)

#### <a name="apidoc.element.deployd.context.context"></a>[function <span class="apidocSignatureSpan">deployd.</span>context (resource, req, res, server)](#apidoc.element.deployd.context.context)
- description and source-code
```javascript
function Context(resource, req, res, server) {
  var ctx = this;
  this.url = req.url.slice(resource.path.length).split('?')[0];
  if (this.url.indexOf('/') !== 0) this.url = '/' + this.url;

  this.req = req;
  this.res = res;
  this.body = req.body;
  this.query = req.query || {};
  this.server = server;
  this.session = req.session;
  this.method = req && req.method;

  // always bind done to this
  var done = this.done;
  this.done = function() {
    done.apply(ctx, arguments);
  };

  if ((this.query && typeof this.query.$limitRecursion !== 'undefined') || (this.body && typeof this.body.$limitRecursion !== 'undefined
')) {
    var recursionLimit = this.query.$limitRecursion || this.body.$limitRecursion || 0;
    req.stack = req.stack || [];
    req.stack.recursionLimit = recursionLimit;
  }

  this.dpd = internalClient.build(server, req.session, req.stack, ctx);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.deployd.context.prototype"></a>[module deployd.context.prototype](#apidoc.module.deployd.context.prototype)

#### <a name="apidoc.element.deployd.context.prototype.done"></a>[function <span class="apidocSignatureSpan">deployd.context.prototype.</span>done (err, res)](#apidoc.element.deployd.context.prototype.done)
- description and source-code
```javascript
done = function (err, res) {
  var body = res
    , type = 'application/json';

  // default response
  var status = this.res.statusCode = this.res.statusCode || 200;

  if(err) {
    debug('%j', err);
    if(status < 400) this.res.statusCode = 400;
    if(err.statusCode) this.res.statusCode = err.statusCode;
    respond(err, this.req, this.res);
  } else {
    if(typeof body == 'object') {
      body = JSON.stringify(body);
    } else {
      type = 'text/html; charset=utf-8';
    }

    try {
      this.res.setHeader("Cache-Control", "no-cache, no-store, must-revalidate");
      this.res.setHeader("Pragma", "no-cache");
      this.res.setHeader("Expires", "0");
      if(status != 204 && status != 304) {
        if(body) {
          this.res.setHeader('Content-Length', Buffer.isBuffer(body)
               ? body.length
               : Buffer.byteLength(body));
        }
        this.res.setHeader('Content-Type', type);
        this.res.end(body);
      } else {
        this.res.end();
      }
    } catch(e) {
      console.error(e);
    }
  }
}
```
- example usage
```shell
...
   fn();
 }
};

/**
* Handle an incoming request. This gets called by the router.
* Call 'next()' if the resource cannot handle the request.
* Otherwise call 'cxt.done(err, res)' when the resource
* is ready to respond.
*
* Example:
*
*  Override the handle method to return a string:
*
*     function MyResource(settings) {
...
```

#### <a name="apidoc.element.deployd.context.prototype.end"></a>[function <span class="apidocSignatureSpan">deployd.context.prototype.</span>end ()](#apidoc.element.deployd.context.prototype.end)
- description and source-code
```javascript
end = function () {
  return this.res.end.apply(this.res, arguments);
}
```
- example usage
```shell
...
  server.handleRequest = function handleRequest(req, res) {
    // dont handle socket.io requests
    if(req.url.indexOf('/socket.io/') === 0) return;
    debug('%s %s', req.method, req.url);

    // add utilites to req and res
    setupReqRes(server.options, req, res, function(err, next) {
if(err) return res.end(err.message);

var authToken, usesBearerAuth = false;
if (req.headers && req.headers.authorization) {
  var parts = req.headers.authorization.split(' ');
  var scheme = parts[0]
  , credentials = parts[1];
...
```



# <a name="apidoc.module.deployd.db"></a>[module deployd.db](#apidoc.module.deployd.db)

#### <a name="apidoc.element.deployd.db.Db"></a>[function <span class="apidocSignatureSpan">deployd.db.</span>Db (options)](#apidoc.element.deployd.db.Db)
- description and source-code
```javascript
function Db(options) {
  this.options = options;
  this.connectionString = this.options.connectionString;
  this.connectionOptions = this.options.connectionOptions || null;
  if (!this.connectionString && this.options.host) {
    this.connectionString = url.format({
      protocol: "mongodb",
      slashes: true,
      hostname: this.options.host,
      port: this.options.port,
      auth: this.options.credentials ? this.options.credentials.username + ":" + this.options.credentials.password : null,
      pathname: this.options.name
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.db.Store"></a>[function <span class="apidocSignatureSpan">deployd.db.</span>Store (namespace, db)](#apidoc.element.deployd.db.Store)
- description and source-code
```javascript
function Store(namespace, db) {
  this.namespace = namespace;
  this._db = db;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.db.create"></a>[function <span class="apidocSignatureSpan">deployd.db.</span>create (options)](#apidoc.element.deployd.db.create)
- description and source-code
```javascript
create = function (options) {
  var db = new Db(options);
  return db;
}
```
- example usage
```shell
...

debug('started with options %j', options);

// an object to map a server to its stores
server.stores = {};

// back all memory stores with a db
server.db = db.create(options.db);

// use socket io for a session based realtime channel
if (options.socketIo && options.socketIo.sockets) {
  server.sockets = options.socketIo.sockets;
} else {
  var socketIo = require('socket.io').listen(server, {'log level':0});
  server.sockets = socketIo.sockets;
...
```



# <a name="apidoc.module.deployd.internal_client"></a>[module deployd.internal_client](#apidoc.module.deployd.internal_client)

#### <a name="apidoc.element.deployd.internal_client.build"></a>[function <span class="apidocSignatureSpan">deployd.internal_client.</span>build (server, session, stack, ctx)](#apidoc.element.deployd.internal_client.build)
- description and source-code
```javascript
build = function (server, session, stack, ctx) {
  var baseMethods
    , dpd = {};

  baseMethods = {
    request: function(method, options, fn) {
      var promise = new Promise(function(resolve, reject) {
        var req
          , res
          , urlKey
          , recursions
          , recursionLimit;

        req = {
            url: joinPath('/', options.path)
          , method: method
          , query: options.query
          , body: options.body
          , session: session
          , isRoot: session && session.isRoot
          , internal: true
          , headers: (ctx && ctx.req) ? (ctx.req.headers || {}) : {}
          , connection: (ctx && ctx.req) ? (ctx.req.connection || {}) : {}
          , on: function() {}
        };

        var callback = function(data, error) {
          // resolve or reject promise
          if (error) {
            reject(error);
          } else {
            resolve(data);
          }
        };

        urlKey = req.method + ' ' + req.url;

        req.stack = stack || [];
        debug("Stack: %j", stack);

        recursions = req.stack.filter(function(s) { return s === urlKey; }).length;

        recursionLimit = (stack && stack.recursionLimit) || 2;

        if (recursions < recursionLimit) {
          req.stack.push(urlKey);
          debug("Putting %s on stack", urlKey);

          res = {
            setHeader: function() {},
            end: function(data) {
              if (res.statusCode === 200 || res.statusCode === 204) {
                try {
                  callback(JSON.parse(data), null);
                } catch (ex) {
                  callback(data, null);
                }
              } else {
                try {
                  callback(null, JSON.parse(data));
                } catch (ex) {
                  callback(null, data);
                }
              }
            },
            internal: true,
            headers: {},
            on: function() {}
          };

          server.router.route(req, res);
        } else {
          debug("Recursive call detected - aborting");
          callback(null, "Recursive call to " + urlKey + " detected");
        }

      }).bind(this);

      if (typeof fn === 'function') {
        // call our old-style callback for backwards compatibility
        promise
          .then(function (data) {
            fn(data);
          }, function (error) {
            fn(null, error);
          });
      }

      return promise;
    }
  };

  baseMethods.get = function(options, fn) {
    return baseMethods.request.call(this, "GET", options, fn);
  };

  baseMethods.post = function(options, fn) {
    return baseMethods.request.call(this, "POST", options, fn);
  };

  baseMethods.put = function(options, fn) {
    return baseMethods.request.call(this, "PUT", options, fn);
  };

  baseMethods.del = function(options, fn) {
    return baseMethods.request.call(this, "DELETE", options, fn);
  };

  if (server.resources) {
    server.resources.forEach(function(r) {
      if (r.clientGeneration) {
        var jsName = r.path.replace(/[^A-Za-z0-9]/g, '');
        dpd[jsName] = createResourceClient(r, baseMethods);
      }
    });
  }

  return dpd;
}
```
- example usage
```shell
...

if ((this.query && typeof this.query.$limitRecursion !== 'undefined') || (this.body && typeof this.body.$limitRecursion !== 'undefined
')) {
  var recursionLimit = this.query.$limitRecursion || this.body.$limitRecursion || 0;
  req.stack = req.stack || [];
  req.stack.recursionLimit = recursionLimit;
}

this.dpd = internalClient.build(server, req.session, req.stack, ctx);
}

/**
 * Alias for 'ctx.res.end()'
 */
Context.prototype.end = function() {
return this.res.end.apply(this.res, arguments);
...
```



# <a name="apidoc.module.deployd.keys"></a>[module deployd.keys](#apidoc.module.deployd.keys)

#### <a name="apidoc.element.deployd.keys.keys"></a>[function <span class="apidocSignatureSpan">deployd.</span>keys (path)](#apidoc.element.deployd.keys.keys)
- description and source-code
```javascript
function Keys(path) {
  this.path = path || '.dpd/keys.json';
}
```
- example usage
```shell
...
    }
    fn(err, result);
  });
};

function loadTypes(fn) {
  _loadTypes(function(defaults, types) {
    Object.keys(types).forEach(function(key) {
      defaults[key] = types[key];
    });
    types = defaults;
    fn(null, types);
  });
}
...
```



# <a name="apidoc.module.deployd.keys.prototype"></a>[module deployd.keys.prototype](#apidoc.module.deployd.keys.prototype)

#### <a name="apidoc.element.deployd.keys.prototype.create"></a>[function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>create (fn)](#apidoc.element.deployd.keys.prototype.create)
- description and source-code
```javascript
create = function (fn) {
  var key = this.generate()
    , keys = this;

  this.readFile(function(err, data) {
    if(err) return fn(err);

    data[key] = true;
    keys.writeFile(data, function(err) {
      fn(err, key);
    });
  });
}
```
- example usage
```shell
...

debug('started with options %j', options);

// an object to map a server to its stores
server.stores = {};

// back all memory stores with a db
server.db = db.create(options.db);

// use socket io for a session based realtime channel
if (options.socketIo && options.socketIo.sockets) {
  server.sockets = options.socketIo.sockets;
} else {
  var socketIo = require('socket.io').listen(server, {'log level':0});
  server.sockets = socketIo.sockets;
...
```

#### <a name="apidoc.element.deployd.keys.prototype.generate"></a>[function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>generate ()](#apidoc.element.deployd.keys.prototype.generate)
- description and source-code
```javascript
generate = function () {
  return crypto.randomBytes(256).toString('hex');
}
```
- example usage
```shell
...
};

/*!
 * Create a new key and save it in the keys file.
 */

Keys.prototype.create = function(fn) {
  var key = this.generate()
, keys = this;

  this.readFile(function(err, data) {
if(err) return fn(err);

data[key] = true;
keys.writeFile(data, function(err) {
...
```

#### <a name="apidoc.element.deployd.keys.prototype.get"></a>[function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>get (key, fn)](#apidoc.element.deployd.keys.prototype.get)
- description and source-code
```javascript
get = function (key, fn) {
  this.readFile(function(err, data) {
    fn(err, data[key]);
  });
}
```
- example usage
```shell
...

if (/^Bearer$/i.test(scheme)) {
  authToken = credentials;
  usesBearerAuth = true;
}
      }

      server.sessions.createSession(authToken || req.cookies.get('sid'), function(err, session) {

if(err) {
  debug('session error', err, session);
  throw err;
} else {
  if (!usesBearerAuth) {
    // (re)set the session id cookie if we're not using Authorization Bearer
...
```

#### <a name="apidoc.element.deployd.keys.prototype.getLocal"></a>[function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>getLocal (fn)](#apidoc.element.deployd.keys.prototype.getLocal)
- description and source-code
```javascript
getLocal = function (fn) {
  this.readFile(function(err, data) {
    if(err) return fn(err);
    if(data && typeof data == 'object') {
      fn(null, Object.keys(data)[0]);
    } else {
      fn();
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.keys.prototype.readFile"></a>[function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>readFile (fn)](#apidoc.element.deployd.keys.prototype.readFile)
- description and source-code
```javascript
readFile = function (fn) {
  fs.readFile(this.path, 'utf-8', function(err, data) {
    var jsonData
      , error;

    try {
      jsonData = (data && JSON.parse(data)) || {};
    } catch (ex) {
      error = ex;
    }

    fn(error, jsonData);
  });
}
```
- example usage
```shell
...
    async.auto({
types: function(fn) {
  getTypes(fn);
},

configJsonFile: function(fn) {
  debug("reading %s", configPath);
  fs.readFile(configPath, 'utf-8', fn);
},

configJson: ['configJsonFile', function(results, fn) {
  try {
    var settings = JSON.parse(results.configJsonFile);
    fn(null, settings);
  } catch (ex) {
...
```

#### <a name="apidoc.element.deployd.keys.prototype.writeFile"></a>[function <span class="apidocSignatureSpan">deployd.keys.prototype.</span>writeFile (data, fn)](#apidoc.element.deployd.keys.prototype.writeFile)
- description and source-code
```javascript
writeFile = function (data, fn) {
  var str;

  try {
    str = JSON.stringify(data);
  } catch(e) {
    return fn(e);
  }

  fs.writeFile(this.path, str, fn);
}
```
- example usage
```shell
...
 var key = this.generate()
   , keys = this;

 this.readFile(function(err, data) {
   if(err) return fn(err);

   data[key] = true;
   keys.writeFile(data, function(err) {
     fn(err, key);
   });
 });
};

/*!
* Read the contents of the key file as JSON
...
```



# <a name="apidoc.module.deployd.resource"></a>[module deployd.resource](#apidoc.module.deployd.resource)

#### <a name="apidoc.element.deployd.resource.resource"></a>[function <span class="apidocSignatureSpan">deployd.</span>resource (name, options)](#apidoc.element.deployd.resource.resource)
- description and source-code
```javascript
function Resource(name, options) {
  EventEmitter.call(this);
  this.name = name;
  this.path = '/' + name;
  options = this.options = options || {};
  this.config = options.config || {};
  this.events = {};
  var instance = this;
  if(this.constructor.external) {
    instance.external = {};
    Object.keys(this.constructor.external).forEach(function (key) {
      if(typeof instance.constructor.external[key] == 'function') {
        instance.external[key] = function () {
          instance.constructor.external[key].apply(instance, arguments);
        };
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.resource.super_"></a>[function <span class="apidocSignatureSpan">deployd.resource.</span>super_ ()](#apidoc.element.deployd.resource.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.resource.toJSON"></a>[function <span class="apidocSignatureSpan">deployd.resource.</span>toJSON ()](#apidoc.element.deployd.resource.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {
    type: this.name,
    defaultPath: '/my-resource'
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.deployd.resource.prototype"></a>[module deployd.resource.prototype](#apidoc.module.deployd.resource.prototype)

#### <a name="apidoc.element.deployd.resource.prototype.handle"></a>[function <span class="apidocSignatureSpan">deployd.resource.prototype.</span>handle (ctx, next)](#apidoc.element.deployd.resource.prototype.handle)
- description and source-code
```javascript
handle = function (ctx, next) {
  ctx.end();
}
```
- example usage
```shell
...

var doSettle = function (settledState, value) {
    state = settledState;
    // persist for handlers registered after settling
    outcome = value;

    thenHandlers.forEach(function (then) {
        then.handle(state, outcome);
    });

    // Discard all references to handlers to be garbage collected
    thenHandlers = null;
};

var doFulfill = function (value) {
...
```

#### <a name="apidoc.element.deployd.resource.prototype.load"></a>[function <span class="apidocSignatureSpan">deployd.resource.prototype.</span>load (fn)](#apidoc.element.deployd.resource.prototype.load)
- description and source-code
```javascript
load = function (fn) {
  var eventNames = this.constructor && this.constructor.events
    , remaining = eventNames && eventNames.length
    , configPath = this.options && this.options.configPath
    , events = this.events = {};

  if(remaining) {
    eventNames.forEach(function(e) {
      var fileName = e.toLowerCase() + '.js'
        , filePath = path.join(configPath, fileName);

      Script.load(filePath, function (err, script) {
        if (script) {
          events[e] = script;
        }
        remaining--;
        if (remaining <= 0) {
          fn();
        }
      });
    });
  } else {
    fn();
  }
}
```
- example usage
```shell
...
}, fn);
}

function loadResourceExtras(resource, fn) {
async.series([
  function(fn) {
    if (resource.load) {
      resource.load(fn);
    } else {
      fn();
    }
  }
], function(err) {
  fn(err, resource);
});
...
```

#### <a name="apidoc.element.deployd.resource.prototype.parse"></a>[function <span class="apidocSignatureSpan">deployd.resource.prototype.</span>parse (url)](#apidoc.element.deployd.resource.prototype.parse)
- description and source-code
```javascript
parse = function (url) {
  var parsed = parse(url, true)
    , pathname = parsed.pathname
    , parts = parsed.parts = pathname.split('/');

  // remove empty
  parts.shift();
  parsed.basepath = parts[0];

  // remove empty trailing slash part
  if(parts[parts.length - 1] === '') parts.pop();

  // the last part is always the identifier
  if(parts.length > 1) parsed.id = parts[parts.length - 1];

  if(parsed.query.q && parsed.query.q[0] === '{' && parsed.query.q[parsed.query.q.length - 1] === '}') {
    parsed.query.q = JSON.parse(parsed.query.q);
  }

  return parsed;
}
```
- example usage
```shell
...
configJsonFile: function(fn) {
  debug("reading %s", configPath);
  fs.readFile(configPath, 'utf-8', fn);
},

configJson: ['configJsonFile', function(results, fn) {
  try {
    var settings = JSON.parse(results.configJsonFile);
    fn(null, settings);
  } catch (ex) {
    fn(ex);
  }
}],

instance: ['configJson', 'types', function(results, fn) {
...
```



# <a name="apidoc.module.deployd.router"></a>[module deployd.router](#apidoc.module.deployd.router)

#### <a name="apidoc.element.deployd.router.router"></a>[function <span class="apidocSignatureSpan">deployd.</span>router (resources, server)](#apidoc.element.deployd.router.router)
- description and source-code
```javascript
function Router(resources, server) {
  this.resources = resources || [];
  this.server = server;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.deployd.router.prototype"></a>[module deployd.router.prototype](#apidoc.module.deployd.router.prototype)

#### <a name="apidoc.element.deployd.router.prototype.generateRegex"></a>[function <span class="apidocSignatureSpan">deployd.router.prototype.</span>generateRegex (path)](#apidoc.element.deployd.router.prototype.generateRegex)
- description and source-code
```javascript
generateRegex = function (path) {
  if (!path || path === '/') path = '';
  path = path.replace(escapeRegExp, '\\$&');
  return new RegExp('^' + path + '(?:[/?].*)?$');
}
```
- example usage
```shell
...
    , result;

  debug('resources %j', this.resources.map(function(r) { return r.path; }));

  if (!this.resources || !this.resources.length) return [];

  result = this.resources.filter(function(d) {
    return url.match(router.generateRegex(d.path));
  }).sort(function(a, b) {
    return specificness(b) - specificness(a);
  });
  return result;
};

/**
...
```

#### <a name="apidoc.element.deployd.router.prototype.matchResources"></a>[function <span class="apidocSignatureSpan">deployd.router.prototype.</span>matchResources (url)](#apidoc.element.deployd.router.prototype.matchResources)
- description and source-code
```javascript
matchResources = function (url) {
  var router = this
    , result;

  debug('resources %j', this.resources.map(function(r) { return r.path; }));

  if (!this.resources || !this.resources.length) return [];

  result = this.resources.filter(function(d) {
    return url.match(router.generateRegex(d.path));
  }).sort(function(a, b) {
    return specificness(b) - specificness(a);
  });
  return result;
}
```
- example usage
```shell
...
 * @api public
 */

Router.prototype.route = function (req, res) {
var router = this
  , server = this.server
  , url = req.url
  , resources = this.matchResources(url)
  , i = 0;

if (req._routed) {
  return;
}

req._routed = true;
...
```

#### <a name="apidoc.element.deployd.router.prototype.route"></a>[function <span class="apidocSignatureSpan">deployd.router.prototype.</span>route (req, res)](#apidoc.element.deployd.router.prototype.route)
- description and source-code
```javascript
route = function (req, res) {
  var router = this
    , server = this.server
    , url = req.url
    , resources = this.matchResources(url)
    , i = 0;

  if (req._routed) {
    return;
  }

  req._routed = true;

  async.series([function(fn) {
    async.forEach(router.resources, function(resource, fn) {
      if(resource.handleSession) {
        var ctx = new Context(resource, req, res, server);
        resource.handleSession(ctx, fn);
      } else {
        fn();
      }
    }, fn);
  }], function(err) {
    if (err) throw err;
    nextResource();
  });

  //TODO: Handle edge case where ctx.next() is called more than once
  function nextResource() {
    var resource = resources[i++]
      , ctx;

    var handler = doh.createHandler({req: req, res: res, server: server});
    handler.run(function () {
      process.nextTick(function () {
        if (resource) {
          debug('routing %s to %s', req.url, resource.path);
          ctx = new Context(resource, req, res, server);
          ctx.router = router;

          // default root to false
          if(ctx.session) ctx.session.isRoot = req.isRoot || false;

          // external functions
          var furl = ctx.url.replace('/', '');
          if(resource.external && resource.external[furl]) {
            resource.external[furl](ctx.body, ctx, ctx.done);
          } else {
            resource.handle(ctx, nextResource);
          }
        } else {
          debug('404 %s', req.url);
          res.statusCode = 404;
          error404({message: 'resource not found'}, req, res);
        }
      });
    });
  }

}
```
- example usage
```shell
...

var root = req.headers['dpd-ssh-key'] || req.cookies.get('DpdSshKey');

if (server.options.env === 'development') {
  if (root) {
    req.isRoot = true;
  }
  server.route(req, res);
} else if (root) {
  // all root requests
  // must be authenticated
  debug('authenticating', root);
  server.keys.get(root, function(err, key) {
    if(err) throw err;
    if(key) req.isRoot = true;
...
```



# <a name="apidoc.module.deployd.script"></a>[module deployd.script](#apidoc.module.deployd.script)

#### <a name="apidoc.element.deployd.script.script"></a>[function <span class="apidocSignatureSpan">deployd.</span>script (src, path)](#apidoc.element.deployd.script.script)
- description and source-code
```javascript
function Script(src, path) {
  this.scriptSourceCode = src;
  this.path = path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.script.load"></a>[function <span class="apidocSignatureSpan">deployd.script.</span>load (path, fn)](#apidoc.element.deployd.script.load)
- description and source-code
```javascript
load = function (path, fn) {
  fs.readFile(path, 'utf-8', function(err, val) {
    if (val) {
      fn(err, new Script(val, path));
    } else {
      fn(err);
    }
  });
}
```
- example usage
```shell
...
}, fn);
}

function loadResourceExtras(resource, fn) {
async.series([
  function(fn) {
    if (resource.load) {
      resource.load(fn);
    } else {
      fn();
    }
  }
], function(err) {
  fn(err, resource);
});
...
```



# <a name="apidoc.module.deployd.script.prototype"></a>[module deployd.script.prototype](#apidoc.module.deployd.script.prototype)

#### <a name="apidoc.element.deployd.script.prototype.getFunction"></a>[function <span class="apidocSignatureSpan">deployd.script.prototype.</span>getFunction (key)](#apidoc.element.deployd.script.prototype.getFunction)
- description and source-code
```javascript
getFunction = function (key) {
  var cache = memoize.cache;
  var address = '' + (hasher ? hasher.apply(this, arguments) : key);
  if (!_.has(cache, address)) cache[address] = func.apply(this, arguments);
  return cache[address];
}
```
- example usage
```shell
...
Script.prototype.runWithContext = function (context) {
var functionArgs = Object.keys(context);

// remove the argument 'this' from our list of passed arguments, because it is a reserved word
functionArgs.splice(functionArgs.indexOf('this'), 1);

functionArgs.push(this.scriptSourceCode);
var func = this.getFunction(functionArgs);

// pass our arguments from the sandbox to the function
var args = [];
functionArgs.forEach(function (p) {
  args.push(context[p]);
});
return func.apply(context._this || {}, args);
...
```

#### <a name="apidoc.element.deployd.script.prototype.run"></a>[function <span class="apidocSignatureSpan">deployd.script.prototype.</span>run (ctx, domain, fn)](#apidoc.element.deployd.script.prototype.run)
- description and source-code
```javascript
run = function (ctx, domain, fn) {

  if (this.error) { fn(this.error); }

  if(typeof domain === 'function') {
    fn = domain;
    domain = undefined;
  }

  var req = ctx.req
    , session = ctx.session
    , waitingForCallback = false
    , callbackCount = 0
    , isDone = false
    , events;

  var scriptContext = {
    'this': {},
    cancel: function(msg, status) {
      var err;
      if (util.isError(msg)) {
        err = msg;
      } else if (!status && msg && msg.message && (msg.status || msg.statusCode)) {
        // allow chaining this from another response
        err = {message: msg.message, statusCode: msg.status || msg.statusCode};
      } else {
        err = {message: msg, statusCode: status};
      }
      done(err);
      throw err;
    },
    cancelIf: function(condition, msg, status) {
      if (condition) {
        scriptContext.cancel(msg, status);
      }
    },
    cancelUnless: function(condition, msg, status) {
      scriptContext.cancelIf(!condition, msg, status);
    },
    me: session && session.user,
    isMe: function(id) {
      return (scriptContext.me && scriptContext.me.id === id) || false;
    },
    console: console,
    query: ctx.query,
    internal: req && req.internal,
    isRoot: req && req.session && req.session.isRoot,
    emit: function(collection, query, event, data) {
      if(arguments.length === 4) {
        session.emitToUsers(collection, query, event, data);
      } else if(arguments.length === 3) {
        // collection is room name
        if(session.emitToRoom) session.emitToRoom(collection, query, event);
      } else if(arguments.length <= 2) {
        event = collection;
        data = query;
        if(session.emitToAll) session.emitToAll(event, data);
      }
    },
    session: session,
    ctx: ctx
  };

  scriptContext._this = scriptContext['this'];
  scriptContext._error = undefined;

  events = new EventEmitter();

  function done(err) {
    if (isDone) return;
    isDone = true;
    events.removeAllListeners('finishCallback');
    if (fn) fn(err);
  }

  if(domain) {

    events.on('addCallback', function() {
      waitingForCallback = true;
      callbackCount++;
    });

    events.on('finishCallback', function() {
      callbackCount--;
      if (callbackCount <= 0) {
        done(scriptContext._error);
      }
    });

    events.on('error', function (err) {
      done(err);
    });

    domain.$addCallback = function() {
      events.emit('addCallback');
    };

    domain.$finishCallback = function() {
      events.emit('finishCallback');
    };
    domain.dpd = ctx.dpd;

    if(fn) {
      // if a callback is expected, count callbacks
      // and manually merge the domain
      wrapAsyncFunctions(domain, scriptContext, events, done);
    } else {
      // otherwise just merge the domain
      Object.keys(domain).forEach(function (key) {
        scriptContext[key] = domain[key];
      });
    }
    scriptContext['this'] = scriptContext._this = domain.data;
  }

  var err;

  try {
    this.runWithContext(scriptContext);
  } catch(e) {
    err = wrapError(e);
    scriptContext._error = err;
  }
  err = err || scriptContext._error;
  process.nextTick(function () {
    if (!waitingForCallback && callbackCount <= 0) {
      done(err);
    }
  });
}
```
- example usage
```shell
...

  //TODO: Handle edge case where ctx.next() is called more than once
  function nextResource() {
    var resource = resources[i++]
      , ctx;

    var handler = doh.createHandler({req: req, res: res, server: server});
    handler.run(function () {
      process.nextTick(function () {
        if (resource) {
debug('routing %s to %s', req.url, resource.path);
ctx = new Context(resource, req, res, server);
ctx.router = router;

// default root to false
...
```

#### <a name="apidoc.element.deployd.script.prototype.runWithContext"></a>[function <span class="apidocSignatureSpan">deployd.script.prototype.</span>runWithContext (context)](#apidoc.element.deployd.script.prototype.runWithContext)
- description and source-code
```javascript
runWithContext = function (context) {
  var functionArgs = Object.keys(context);

  // remove the argument 'this' from our list of passed arguments, because it is a reserved word
  functionArgs.splice(functionArgs.indexOf('this'), 1);

  functionArgs.push(this.scriptSourceCode);
  var func = this.getFunction(functionArgs);

  // pass our arguments from the sandbox to the function
  var args = [];
  functionArgs.forEach(function (p) {
    args.push(context[p]);
  });
  return func.apply(context._this || {}, args);
}
```
- example usage
```shell
...
  }
  scriptContext['this'] = scriptContext._this = domain.data;
}

var err;

try {
  this.runWithContext(scriptContext);
} catch(e) {
  err = wrapError(e);
  scriptContext._error = err;
}
err = err || scriptContext._error;
process.nextTick(function () {
  if (!waitingForCallback && callbackCount <= 0) {
...
```



# <a name="apidoc.module.deployd.server"></a>[module deployd.server](#apidoc.module.deployd.server)

#### <a name="apidoc.element.deployd.server.server"></a>[function <span class="apidocSignatureSpan">deployd.</span>server (options)](#apidoc.element.deployd.server.server)
- description and source-code
```javascript
function Server(options) {
  var server = process.server = this;
  http.Server.call(this);

  // defaults
  this.options = options = extend({
    port: 2403,
    db: {port: 27017, host: '127.0.0.1', name: 'deployd'}
  }, options);

  debug('started with options %j', options);

  // an object to map a server to its stores
  this.stores = {};

  // back all memory stores with a db
  this.db = db.create(options.db);

  var socketServer = io.listen(this, _.extend({
    'log level': 0
  }, (this.options.socketIo && this.options.socketIo.options) || {}));

  // use socket io for a session based realtime channel
  this.sockets = socketServer.sockets;

  if (this.options.socketIo && this.options.socketIo.adapter) {
    socketServer.adapter(this.options.socketIo.adapter);
  }

  // persist sessions in a store
  this.sessions = new SessionStore('sessions', this.db, this.sockets, options.sessions);

  // persist keys in a store
  this.keys = new Keys();

  this.on('request', server.handleRequest);

  server.on('request:error', function (err, req, res) {
    console.error();
    console.error(req.method, req.url, err.stack || err);
    process.exit(1);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.server.super_"></a>[function <span class="apidocSignatureSpan">deployd.server.</span>super_ (requestListener)](#apidoc.element.deployd.server.super_)
- description and source-code
```javascript
function Server(requestListener) {
  if (!(this instanceof Server)) return new Server(requestListener);
  net.Server.call(this, { allowHalfOpen: true });

  if (requestListener) {
    this.addListener('request', requestListener);
  }

<span class="apidocCodeCommentSpan">  /* eslint-disable max-len */
</span>  // Similar option to this. Too lazy to write my own docs.
  // http://www.squid-cache.org/Doc/config/half_closed_clients/
  // http://wiki.squid-cache.org/SquidFaq/InnerWorkings#What_is_a_half-closed_filedescriptor.3F
  /* eslint-enable max-len */
  this.httpAllowHalfOpen = false;

  this.addListener('connection', connectionListener);

  this.timeout = 2 * 60 * 1000;

  this._pendingResponseData = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.deployd.server.prototype"></a>[module deployd.server.prototype](#apidoc.module.deployd.server.prototype)

#### <a name="apidoc.element.deployd.server.prototype.createStore"></a>[function <span class="apidocSignatureSpan">deployd.server.prototype.</span>createStore (namespace)](#apidoc.element.deployd.server.prototype.createStore)
- description and source-code
```javascript
createStore = function (namespace) {
	return (this.stores[namespace] = this.db.createStore(namespace));
}
```
- example usage
```shell
...

/**
* Create a new 'Store' for persisting data using the database info that was passed to the server when it was created.
*
* Example:
*
*     // Attach a store to the server
*     var todos = server.createStore('todos');
*
*     // Use the store to CRUD data
*     todos.insert({name: 'go to the store', done: true}, ...); // see 'Store' for more info
*
* @param {String} namespace
* @return {Store}
*/
...
```

#### <a name="apidoc.element.deployd.server.prototype.handleRequest"></a>[function <span class="apidocSignatureSpan">deployd.server.prototype.</span>handleRequest (req, res)](#apidoc.element.deployd.server.prototype.handleRequest)
- description and source-code
```javascript
function handleRequest(req, res) {
  var server = this;
  // dont handle socket.io requests
  if(req.url.indexOf('/socket.io/') === 0) return;

  debug('%s %s', req.method, req.url);

  // add utilites to req and res
  setupReqRes(server.options, req, res, function(err, next) {
    if(err) return res.end(err.message);

    var authToken, usesBearerAuth = false;
    if (req.headers && req.headers.authorization) {
      var parts = req.headers.authorization.split(' ');
      var scheme = parts[0]
      , credentials = parts[1];

      if (/^Bearer$/i.test(scheme)) {
        authToken = credentials;
        usesBearerAuth = true;
      }
    }

    server.sessions.createSession(authToken || req.cookies.get('sid'), function(err, session) {
      if(err) {
        debug('session error', err, session);
        throw err;
      } else {
        if (!usesBearerAuth) {
          // (re)set the session id cookie if we're not using Authorization Bearer
          if (session.sid) req.cookies.set('sid', session.sid);
        }
        req.session = session;

        var root = req.headers['dpd-ssh-key'] || req.cookies.get('DpdSshKey');

        if (server.options.env === 'development') {
          if (root) { req.isRoot = true; }
          server.route(req, res);
        } else if (root) {
          // all root requests
          // must be authenticated
          debug('authenticating', root);
          server.keys.get(root, function(err, key) {
            if(err) throw err;
            if(key) req.isRoot = true;
            debug('is root?', session.isRoot);
            server.route(req, res);
          });
        } else {
          // normal route
          server.route(req, res);
        }
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.deployd.server.prototype.listen"></a>[function <span class="apidocSignatureSpan">deployd.server.prototype.</span>listen (port, host)](#apidoc.element.deployd.server.prototype.listen)
- description and source-code
```javascript
listen = function (port, host) {
  var server = this;
  var serverpath = server.options.server_dir || fs.realpathSync('./');

  config.loadConfig(serverpath, server, function(err, resourcesInstances) {
    if (err) {
      console.error();
      console.error("Error loading resources: ");
      console.error(err.stack || err);
      process.exit(1);
    } else {
      server.resources = resourcesInstances;
      var router = new Router(resourcesInstances, server);
      server.router = router;
      http.Server.prototype.listen.call(server, port || server.options.port, host || server.options.host);
    }
  });
  return this;
}
```
- example usage
```shell
...
*
* Example:
*
*   var http = require('http');
*   var express = require('express');
*   var app = express();
*   var server = http.createServer(app);
*   var io = require('socket.io').listen(server, {'log level': 0});
*
*   var deployd = require('deployd')
*   deployd.attach(server, {socketIo: io, env: ENV, db:{host:'localhost', port:27015, name:'my-db'} } );
*   app.use(server.handleRequest);
*
*   server.listen();
*
...
```

#### <a name="apidoc.element.deployd.server.prototype.route"></a>[function <span class="apidocSignatureSpan">deployd.server.prototype.</span>route (req, res)](#apidoc.element.deployd.server.prototype.route)
- description and source-code
```javascript
function route(req, res) {
  var server = this;
  var serverpath = server.options.server_dir || './';

  config.loadConfig(serverpath, server, function(err, resourcesInstances) {
    if (err) throw err;
    var router = new Router(resourcesInstances, server);
    server.router = router;

    server.resources = resourcesInstances;
    router.route(req, res);
  });
}
```
- example usage
```shell
...

var root = req.headers['dpd-ssh-key'] || req.cookies.get('DpdSshKey');

if (server.options.env === 'development') {
  if (root) {
    req.isRoot = true;
  }
  server.route(req, res);
} else if (root) {
  // all root requests
  // must be authenticated
  debug('authenticating', root);
  server.keys.get(root, function(err, key) {
    if(err) throw err;
    if(key) req.isRoot = true;
...
```



# <a name="apidoc.module.deployd.session"></a>[module deployd.session](#apidoc.module.deployd.session)

#### <a name="apidoc.element.deployd.session.SessionStore"></a>[function <span class="apidocSignatureSpan">deployd.session.</span>SessionStore (namespace, db, sockets, options)](#apidoc.element.deployd.session.SessionStore)
- description and source-code
```javascript
function SessionStore(namespace, db, sockets, options) {
  var self = this;

  // unique id for this store in order to identify in a cluster
  this.id = this.createUniqueIdentifier();

  this.sockets = sockets;
  this.options = options || {};
  // sessions inactive for longer than this will be cleaned up:
  this.options.maxAge = this.options.maxAge || 30 * 24 * 60 * 60 * 1000;

  if (this.options.pubClient && this.options.subClient) {
    debug('using pub/sub mode');
    this.pubClient = this.options.pubClient;
    this.subClient = this.options.subClient;
  }

  // socket queue
  var socketQueue = this.socketQueue = new EventEmitter()
    , socketIndex = this.socketIndex = {};

  if (sockets) {
    if (this.subClient) {
      // subscribe to messages regarding sessions joining/leaving rooms
      // need to resync
      this.subClient.subscribe('dpd#session#refreshrooms');
      this.subClient.subscribe('dpd#session#remove');
      this.subClient.on('message', function(channel, message) {
        var data;
        switch (channel) {
          case 'dpd#session#refreshrooms': // another node changed rooms for a session
            data = JSON.parse(message);
            if (data.id !== self.id && data.sid && socketIndex[data.sid]) {
              // if we know about this session, refresh the rooms
              self.refreshSessionRooms(data.sid);
            }

            break;
          case 'dpd#session#remove': // another node removed a session
            data = JSON.parse(message);
            if (data.id !== self.id && data.sid && sessionIndex[data.sid]) {
              // if we know about this session, remove it from memory
              sessionIndex[data.sid]._leaveAllRooms();
              self.removeSessionFromMemory(data.sid);
            }

            break;
        }
      });
    }

    sockets.on('connection', function(client) {
      // NOTE: do not use set here ever, the 'Cookies' api is meant to get a req, res
      // but we are just using it for a cookie parser
      var cookies = new Cookies(client.handshake)
        , sid = cookies.get('sid');

      var getSession = function(sid, fn) {
        // check if we already know about the session
        var session = sessionIndex[sid];
        if (session) { return fn(null, session); }
        // get the session from the store otherwise
        self.createSession(sid, function(err, session) {
          if (session.data.id === sid) return fn(null, session);
          return fn();
        });
      };

      var indexSocket = function(sid, client, session) {
        // index sockets against their session id
        socketIndex[sid] = socketIndex[sid] || {};
        socketIndex[sid][client.id] = client;
        socketQueue.emit('socket', client, session);

        // make sure the list of rooms to join is fresh
        self.refreshSessionRooms(sid);
      };

      if (sid) {
        getSession(sid, function(err, session) {
          if (session) {
            indexSocket(sid, client, session);
          }
        });
      }

      // Alternative way of binding session to socket connection
      // for when the sid cookie is not yet available.
      // This expects that the client emits an event with the sid.
      function setSession(data) {
        if (!data || !data.sid || typeof data.sid !== 'string') { return; }
        var sid = data.sid;

        getSession(sid, function(err, session) {
          if (session) {
            // unassign socket from previous sessions
            _.each(socketIndex, function(val) {
              delete val[client.id];
            });

            indexSocket(sid, client, session);
          }
        });
      }

      client.on('server:setSession', setSession);
      client.on('server:setsession', setSession); // allow lowercase

      client.on('disconnect', function() {
        // unassign socket from previous sessions
        _.each(socketIndex, function(val, sid) {
          delete val[client.id];
        });
      });
    });

    var drainQueue = function drainQueue(method, rawSocket, session) {
      var key = ...
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
