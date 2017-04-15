# api documentation for  [websocket (v1.0.24)](https://github.com/theturtle32/WebSocket-Node)  [![npm package](https://img.shields.io/npm/v/npmdoc-websocket.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-websocket) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-websocket.svg)](https://travis-ci.org/npmdoc/node-npmdoc-websocket)
#### Websocket Client & Server Library implementing the WebSocket protocol as specified in RFC 6455.

[![NPM](https://nodei.co/npm/websocket.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/websocket)

[![apidoc](https://npmdoc.github.io/node-npmdoc-websocket/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-websocket/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-websocket/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-websocket/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brian McKelvey",
        "url": "https://www.worlize.com/"
    },
    "browser": "lib/browser.js",
    "bugs": {
        "url": "https://github.com/theturtle32/WebSocket-Node/issues"
    },
    "config": {
        "verbose": false
    },
    "contributors": [
        {
            "name": "Iñaki Baz Castillo",
            "url": "http://dev.sipdoc.net"
        }
    ],
    "dependencies": {
        "debug": "^2.2.0",
        "nan": "^2.3.3",
        "typedarray-to-buffer": "^3.1.2",
        "yaeti": "^0.0.6"
    },
    "description": "Websocket Client & Server Library implementing the WebSocket protocol as specified in RFC 6455.",
    "devDependencies": {
        "buffer-equal": "^1.0.0",
        "faucet": "^0.0.1",
        "gulp": "git+https://github.com/gulpjs/gulp.git#4.0",
        "gulp-jshint": "^2.0.4",
        "jshint": "^2.0.0",
        "jshint-stylish": "^2.2.1",
        "tape": "^4.0.1"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "74903e75f2545b6b2e1de1425bc1c905917a1890",
        "tarball": "https://registry.npmjs.org/websocket/-/websocket-1.0.24.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "gitHead": "0e15f9445953927c39ce84a232cb7dd6e3adf12e",
    "homepage": "https://github.com/theturtle32/WebSocket-Node",
    "keywords": [
        "websocket",
        "websockets",
        "socket",
        "networking",
        "comet",
        "push",
        "RFC-6455",
        "realtime",
        "server",
        "client"
    ],
    "license": "Apache-2.0",
    "main": "index",
    "maintainers": [
        {
            "name": "theturtle32"
        }
    ],
    "name": "websocket",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/theturtle32/WebSocket-Node.git"
    },
    "scripts": {
        "gulp": "gulp",
        "install": "(node-gyp rebuild 2> builderror.log) || (exit 0)",
        "test": "faucet test/unit"
    },
    "version": "1.0.24"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module websocket](#apidoc.module.websocket)
1.  [function <span class="apidocSignatureSpan">websocket.</span>client (config)](#apidoc.element.websocket.client)
1.  [function <span class="apidocSignatureSpan">websocket.</span>connection (socket, extensions, protocol, maskOutgoingPackets, config)](#apidoc.element.websocket.connection)
1.  [function <span class="apidocSignatureSpan">websocket.</span>frame (maskBytes, frameHeader, config)](#apidoc.element.websocket.frame)
1.  [function <span class="apidocSignatureSpan">websocket.</span>request (socket, httpRequest, serverConfig)](#apidoc.element.websocket.request)
1.  [function <span class="apidocSignatureSpan">websocket.</span>router (config)](#apidoc.element.websocket.router)
1.  [function <span class="apidocSignatureSpan">websocket.</span>server (config)](#apidoc.element.websocket.server)
1.  [function <span class="apidocSignatureSpan">websocket.</span>w3cwebsocket (url, protocols, origin, headers, requestOptions, clientConfig)](#apidoc.element.websocket.w3cwebsocket)
1.  object <span class="apidocSignatureSpan">websocket.</span>client.prototype
1.  object <span class="apidocSignatureSpan">websocket.</span>connection.prototype
1.  object <span class="apidocSignatureSpan">websocket.</span>deprecation
1.  object <span class="apidocSignatureSpan">websocket.</span>frame.prototype
1.  object <span class="apidocSignatureSpan">websocket.</span>request.prototype
1.  object <span class="apidocSignatureSpan">websocket.</span>router.prototype
1.  object <span class="apidocSignatureSpan">websocket.</span>server.prototype
1.  object <span class="apidocSignatureSpan">websocket.</span>w3cwebsocket.prototype
1.  string <span class="apidocSignatureSpan">websocket.</span>version

#### [module websocket.client](#apidoc.module.websocket.client)
1.  [function <span class="apidocSignatureSpan">websocket.</span>client (config)](#apidoc.element.websocket.client.client)
1.  [function <span class="apidocSignatureSpan">websocket.client.</span>super_ ()](#apidoc.element.websocket.client.super_)

#### [module websocket.client.prototype](#apidoc.module.websocket.client.prototype)
1.  [function <span class="apidocSignatureSpan">websocket.client.prototype.</span>abort ()](#apidoc.element.websocket.client.prototype.abort)
1.  [function <span class="apidocSignatureSpan">websocket.client.prototype.</span>connect (requestUrl, protocols, origin, headers, extraRequestOptions)](#apidoc.element.websocket.client.prototype.connect)
1.  [function <span class="apidocSignatureSpan">websocket.client.prototype.</span>failHandshake (errorDescription)](#apidoc.element.websocket.client.prototype.failHandshake)
1.  [function <span class="apidocSignatureSpan">websocket.client.prototype.</span>succeedHandshake ()](#apidoc.element.websocket.client.prototype.succeedHandshake)
1.  [function <span class="apidocSignatureSpan">websocket.client.prototype.</span>validateHandshake ()](#apidoc.element.websocket.client.prototype.validateHandshake)

#### [module websocket.connection](#apidoc.module.websocket.connection)
1.  [function <span class="apidocSignatureSpan">websocket.</span>connection (socket, extensions, protocol, maskOutgoingPackets, config)](#apidoc.element.websocket.connection.connection)
1.  [function <span class="apidocSignatureSpan">websocket.connection.</span>super_ ()](#apidoc.element.websocket.connection.super_)
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_ABNORMAL
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_EXTENSION_REQUIRED
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_GOING_AWAY
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_INTERNAL_SERVER_ERROR
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_INVALID_DATA
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_MESSAGE_TOO_BIG
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_NORMAL
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_NOT_PROVIDED
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_POLICY_VIOLATION
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_PROTOCOL_ERROR
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_RESERVED
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_TLS_HANDSHAKE_FAILED
1.  number <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_REASON_UNPROCESSABLE_INPUT
1.  object <span class="apidocSignatureSpan">websocket.connection.</span>CLOSE_DESCRIPTIONS

#### [module websocket.connection.prototype](#apidoc.module.websocket.connection.prototype)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>_addSocketEventListeners ()](#apidoc.element.websocket.connection.prototype._addSocketEventListeners)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>clearCloseTimer ()](#apidoc.element.websocket.connection.prototype.clearCloseTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>clearGracePeriodTimer ()](#apidoc.element.websocket.connection.prototype.clearGracePeriodTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>clearKeepaliveTimer ()](#apidoc.element.websocket.connection.prototype.clearKeepaliveTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>close (reasonCode, description)](#apidoc.element.websocket.connection.prototype.close)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>drop (reasonCode, description, skipCloseFrame)](#apidoc.element.websocket.connection.prototype.drop)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>fragmentAndSend (frame, cb)](#apidoc.element.websocket.connection.prototype.fragmentAndSend)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleCloseTimer ()](#apidoc.element.websocket.connection.prototype.handleCloseTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleGracePeriodTimer ()](#apidoc.element.websocket.connection.prototype.handleGracePeriodTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleKeepaliveTimer ()](#apidoc.element.websocket.connection.prototype.handleKeepaliveTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketClose (hadError)](#apidoc.element.websocket.connection.prototype.handleSocketClose)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketData (data)](#apidoc.element.websocket.connection.prototype.handleSocketData)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketDrain ()](#apidoc.element.websocket.connection.prototype.handleSocketDrain)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketEnd ()](#apidoc.element.websocket.connection.prototype.handleSocketEnd)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketError (error)](#apidoc.element.websocket.connection.prototype.handleSocketError)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketPause ()](#apidoc.element.websocket.connection.prototype.handleSocketPause)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketResume ()](#apidoc.element.websocket.connection.prototype.handleSocketResume)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>pause ()](#apidoc.element.websocket.connection.prototype.pause)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>ping (data)](#apidoc.element.websocket.connection.prototype.ping)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>pong (binaryPayload)](#apidoc.element.websocket.connection.prototype.pong)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>processFrame (frame)](#apidoc.element.websocket.connection.prototype.processFrame)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>processReceivedData ()](#apidoc.element.websocket.connection.prototype.processReceivedData)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>resume ()](#apidoc.element.websocket.connection.prototype.resume)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>send (data, cb)](#apidoc.element.websocket.connection.prototype.send)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendBytes (data, cb)](#apidoc.element.websocket.connection.prototype.sendBytes)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendCloseFrame (reasonCode, description, cb)](#apidoc.element.websocket.connection.prototype.sendCloseFrame)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendFrame (frame, cb)](#apidoc.element.websocket.connection.prototype.sendFrame)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendUTF (data, cb)](#apidoc.element.websocket.connection.prototype.sendUTF)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>setCloseTimer ()](#apidoc.element.websocket.connection.prototype.setCloseTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>setGracePeriodTimer ()](#apidoc.element.websocket.connection.prototype.setGracePeriodTimer)
1.  [function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>setKeepaliveTimer ()](#apidoc.element.websocket.connection.prototype.setKeepaliveTimer)

#### [module websocket.deprecation](#apidoc.module.websocket.deprecation)
1.  boolean <span class="apidocSignatureSpan">websocket.deprecation.</span>disableWarnings
1.  [function <span class="apidocSignatureSpan">websocket.deprecation.</span>warn (deprecationName)](#apidoc.element.websocket.deprecation.warn)
1.  object <span class="apidocSignatureSpan">websocket.deprecation.</span>deprecationWarningMap

#### [module websocket.frame](#apidoc.module.websocket.frame)
1.  [function <span class="apidocSignatureSpan">websocket.</span>frame (maskBytes, frameHeader, config)](#apidoc.element.websocket.frame.frame)

#### [module websocket.frame.prototype](#apidoc.module.websocket.frame.prototype)
1.  [function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>addData (bufferList)](#apidoc.element.websocket.frame.prototype.addData)
1.  [function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>throwAwayPayload (bufferList)](#apidoc.element.websocket.frame.prototype.throwAwayPayload)
1.  [function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>toBuffer (nullMask)](#apidoc.element.websocket.frame.prototype.toBuffer)
1.  [function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>toString ()](#apidoc.element.websocket.frame.prototype.toString)

#### [module websocket.request](#apidoc.module.websocket.request)
1.  [function <span class="apidocSignatureSpan">websocket.</span>request (socket, httpRequest, serverConfig)](#apidoc.element.websocket.request.request)
1.  [function <span class="apidocSignatureSpan">websocket.request.</span>super_ ()](#apidoc.element.websocket.request.super_)

#### [module websocket.request.prototype](#apidoc.module.websocket.request.prototype)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>_handleSocketCloseBeforeAccept ()](#apidoc.element.websocket.request.prototype._handleSocketCloseBeforeAccept)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>_removeSocketCloseListeners ()](#apidoc.element.websocket.request.prototype._removeSocketCloseListeners)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>_verifyResolution ()](#apidoc.element.websocket.request.prototype._verifyResolution)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>accept (acceptedProtocol, allowedOrigin, cookies)](#apidoc.element.websocket.request.prototype.accept)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>parseCookies (str)](#apidoc.element.websocket.request.prototype.parseCookies)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>parseExtensions (extensionsString)](#apidoc.element.websocket.request.prototype.parseExtensions)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>readHandshake ()](#apidoc.element.websocket.request.prototype.readHandshake)
1.  [function <span class="apidocSignatureSpan">websocket.request.prototype.</span>reject (status, reason, extraHeaders)](#apidoc.element.websocket.request.prototype.reject)

#### [module websocket.router](#apidoc.module.websocket.router)
1.  [function <span class="apidocSignatureSpan">websocket.</span>router (config)](#apidoc.element.websocket.router.router)
1.  [function <span class="apidocSignatureSpan">websocket.router.</span>super_ ()](#apidoc.element.websocket.router.super_)

#### [module websocket.router.prototype](#apidoc.module.websocket.router.prototype)
1.  [function <span class="apidocSignatureSpan">websocket.router.prototype.</span>attachServer (server)](#apidoc.element.websocket.router.prototype.attachServer)
1.  [function <span class="apidocSignatureSpan">websocket.router.prototype.</span>detachServer ()](#apidoc.element.websocket.router.prototype.detachServer)
1.  [function <span class="apidocSignatureSpan">websocket.router.prototype.</span>findHandlerIndex (pathString, protocol)](#apidoc.element.websocket.router.prototype.findHandlerIndex)
1.  [function <span class="apidocSignatureSpan">websocket.router.prototype.</span>handleRequest (request)](#apidoc.element.websocket.router.prototype.handleRequest)
1.  [function <span class="apidocSignatureSpan">websocket.router.prototype.</span>mount (path, protocol, callback)](#apidoc.element.websocket.router.prototype.mount)
1.  [function <span class="apidocSignatureSpan">websocket.router.prototype.</span>pathToRegExp (path)](#apidoc.element.websocket.router.prototype.pathToRegExp)
1.  [function <span class="apidocSignatureSpan">websocket.router.prototype.</span>unmount (path, protocol)](#apidoc.element.websocket.router.prototype.unmount)

#### [module websocket.server](#apidoc.module.websocket.server)
1.  [function <span class="apidocSignatureSpan">websocket.</span>server (config)](#apidoc.element.websocket.server.server)
1.  [function <span class="apidocSignatureSpan">websocket.server.</span>super_ ()](#apidoc.element.websocket.server.super_)

#### [module websocket.server.prototype](#apidoc.module.websocket.server.prototype)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>broadcast (data)](#apidoc.element.websocket.server.prototype.broadcast)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>broadcastBytes (binaryData)](#apidoc.element.websocket.server.prototype.broadcastBytes)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>broadcastUTF (utfData)](#apidoc.element.websocket.server.prototype.broadcastUTF)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>closeAllConnections ()](#apidoc.element.websocket.server.prototype.closeAllConnections)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleConnectionClose (connection, closeReason, description)](#apidoc.element.websocket.server.prototype.handleConnectionClose)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleRequestAccepted (connection)](#apidoc.element.websocket.server.prototype.handleRequestAccepted)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleRequestResolved (request)](#apidoc.element.websocket.server.prototype.handleRequestResolved)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleUpgrade (request, socket)](#apidoc.element.websocket.server.prototype.handleUpgrade)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>mount (config)](#apidoc.element.websocket.server.prototype.mount)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>shutDown ()](#apidoc.element.websocket.server.prototype.shutDown)
1.  [function <span class="apidocSignatureSpan">websocket.server.prototype.</span>unmount ()](#apidoc.element.websocket.server.prototype.unmount)

#### [module websocket.w3cwebsocket](#apidoc.module.websocket.w3cwebsocket)
1.  [function <span class="apidocSignatureSpan">websocket.</span>w3cwebsocket (url, protocols, origin, headers, requestOptions, clientConfig)](#apidoc.element.websocket.w3cwebsocket.w3cwebsocket)

#### [module websocket.w3cwebsocket.prototype](#apidoc.module.websocket.w3cwebsocket.prototype)
1.  [function <span class="apidocSignatureSpan">websocket.w3cwebsocket.prototype.</span>close (code, reason)](#apidoc.element.websocket.w3cwebsocket.prototype.close)
1.  [function <span class="apidocSignatureSpan">websocket.w3cwebsocket.prototype.</span>send (data)](#apidoc.element.websocket.w3cwebsocket.prototype.send)



# <a name="apidoc.module.websocket"></a>[module websocket](#apidoc.module.websocket)

#### <a name="apidoc.element.websocket.client"></a>[function <span class="apidocSignatureSpan">websocket.</span>client (config)](#apidoc.element.websocket.client)
- description and source-code
```javascript
function WebSocketClient(config) {
    // Superclass Constructor
    EventEmitter.call(this);

    // TODO: Implement extensions

    this.config = {
        // 1MiB max frame size.
        maxReceivedFrameSize: 0x100000,

        // 8MiB max message size, only applicable if
        // assembleFragments is true
        maxReceivedMessageSize: 0x800000,

        // Outgoing messages larger than fragmentationThreshold will be
        // split into multiple fragments.
        fragmentOutgoingMessages: true,

        // Outgoing frames are fragmented if they exceed this threshold.
        // Default is 16KiB
        fragmentationThreshold: 0x4000,

        // Which version of the protocol to use for this session.  This
        // option will be removed once the protocol is finalized by the IETF
        // It is only available to ease the transition through the
        // intermediate draft protocol versions.
        // At present, it only affects the name of the Origin header.
        webSocketVersion: 13,

        // If true, fragmented messages will be automatically assembled
        // and the full message will be emitted via a 'message' event.
        // If false, each frame will be emitted via a 'frame' event and
        // the application will be responsible for aggregating multiple
        // fragmented frames.  Single-frame messages will emit a 'message'
        // event in addition to the 'frame' event.
        // Most users will want to leave this set to 'true'
        assembleFragments: true,

        // The Nagle Algorithm makes more efficient use of network resources
        // by introducing a small delay before sending small packets so that
        // multiple messages can be batched together before going onto the
        // wire.  This however comes at the cost of latency, so the default
        // is to disable it.  If you don't need low latency and are streaming
        // lots of small messages, you can change this to 'false'
        disableNagleAlgorithm: true,

        // The number of milliseconds to wait after sending a close frame
        // for an acknowledgement to come back before giving up and just
        // closing the socket.
        closeTimeout: 5000,

        // Options to pass to https.connect if connecting via TLS
        tlsOptions: {}
    };

    if (config) {
        var tlsOptions;
        if (config.tlsOptions) {
          tlsOptions = config.tlsOptions;
          delete config.tlsOptions;
        }
        else {
          tlsOptions = {};
        }
        extend(this.config, config);
        extend(this.config.tlsOptions, tlsOptions);
    }

    this._req = null;

    switch (this.config.webSocketVersion) {
        case 8:
        case 13:
            break;
        default:
            throw new Error('Requested webSocketVersion is not supported. Allowed values are 8 and 13.');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection"></a>[function <span class="apidocSignatureSpan">websocket.</span>connection (socket, extensions, protocol, maskOutgoingPackets, config)](#apidoc.element.websocket.connection)
- description and source-code
```javascript
function WebSocketConnection(socket, extensions, protocol, maskOutgoingPackets, config) {
    this._debug = utils.BufferingLogger('websocket:connection', ++idCounter);
    this._debug('constructor');

    if (this._debug.enabled) {
        instrumentSocketForDebugging(this, socket);
    }

    // Superclass Constructor
    EventEmitter.call(this);

    this._pingListenerCount = 0;
    this.on('newListener', function(ev) {
        if (ev === 'ping'){
            this._pingListenerCount++;
        }
      }).on('removeListener', function(ev) {
        if (ev === 'ping') {
            this._pingListenerCount--;
        }
    });

    this.config = config;
    this.socket = socket;
    this.protocol = protocol;
    this.extensions = extensions;
    this.remoteAddress = socket.remoteAddress;
    this.closeReasonCode = -1;
    this.closeDescription = null;
    this.closeEventEmitted = false;

    // We have to mask outgoing packets if we're acting as a WebSocket client.
    this.maskOutgoingPackets = maskOutgoingPackets;

    // We re-use the same buffers for the mask and frame header for all frames
    // received on each connection to avoid a small memory allocation for each
    // frame.
    this.maskBytes = new Buffer(4);
    this.frameHeader = new Buffer(10);

    // the BufferList will handle the data streaming in
    this.bufferList = new BufferList();

    // Prepare for receiving first frame
    this.currentFrame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);
    this.fragmentationSize = 0; // data received so far...
    this.frameQueue = [];

    // Various bits of connection state
    this.connected = true;
    this.state = STATE_OPEN;
    this.waitingForCloseResponse = false;
    // Received TCP FIN, socket's readable stream is finished.
    this.receivedEnd = false;

    this.closeTimeout = this.config.closeTimeout;
    this.assembleFragments = this.config.assembleFragments;
    this.maxReceivedMessageSize = this.config.maxReceivedMessageSize;

    this.outputBufferFull = false;
    this.inputPaused = false;
    this.receivedDataHandler = this.processReceivedData.bind(this);
    this._closeTimerHandler = this.handleCloseTimer.bind(this);

    // Disable nagle algorithm?
    this.socket.setNoDelay(this.config.disableNagleAlgorithm);

    // Make sure there is no socket inactivity timeout
    this.socket.setTimeout(0);

    if (this.config.keepalive && !this.config.useNativeKeepalive) {
        if (typeof(this.config.keepaliveInterval) !== 'number') {
            throw new Error('keepaliveInterval must be specified and numeric ' +
                            'if keepalive is true.');
        }
        this._keepaliveTimerHandler = this.handleKeepaliveTimer.bind(this);
        this.setKeepaliveTimer();

        if (this.config.dropConnectionOnKeepaliveTimeout) {
            if (typeof(this.config.keepaliveGracePeriod) !== 'number') {
                throw new Error('keepaliveGracePeriod  must be specified and ' +
                                'numeric if dropConnectionOnKeepaliveTimeout ' +
                                'is true.');
            }
            this._gracePeriodTimerHandler = this.handleGracePeriodTimer.bind(this);
        }
    }
    else if (this.config.keepalive && this.config.useNativeKeepalive) {
        if (!('setKeepAlive' in this.socket)) {
            throw new Error('Unable to use native keepalive: unsupported by ' +
                            'this version of Node.');
        }
        this.socket.setKeepAlive(true, this.config.keepaliveInterval);
    }

    // The HTTP Client seems to subscribe to socket error events
    // and re-dispatch them in such a way that doesn't make sense
    // for users of our client, so we want to make sure nobody
    // else is listening for error events on the socket besides us.
    this.socket.removeAllListeners('error');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.frame"></a>[function <span class="apidocSignatureSpan">websocket.</span>frame (maskBytes, frameHeader, config)](#apidoc.element.websocket.frame)
- description and source-code
```javascript
function WebSocketFrame(maskBytes, frameHeader, config) {
    this.maskBytes = maskBytes;
    this.frameHeader = frameHeader;
    this.config = config;
    this.maxReceivedFrameSize = config.maxReceivedFrameSize;
    this.protocolError = false;
    this.frameTooLarge = false;
    this.invalidCloseFrameLength = false;
    this.parseState = DECODE_HEADER;
    this.closeStatus = -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request"></a>[function <span class="apidocSignatureSpan">websocket.</span>request (socket, httpRequest, serverConfig)](#apidoc.element.websocket.request)
- description and source-code
```javascript
function WebSocketRequest(socket, httpRequest, serverConfig) {
    // Superclass Constructor
    EventEmitter.call(this);

    this.socket = socket;
    this.httpRequest = httpRequest;
    this.resource = httpRequest.url;
    this.remoteAddress = socket.remoteAddress;
    this.remoteAddresses = [this.remoteAddress];
    this.serverConfig = serverConfig;

    // Watch for the underlying TCP socket closing before we call accept
    this._socketIsClosing = false;
    this._socketCloseHandler = this._handleSocketCloseBeforeAccept.bind(this);
    this.socket.on('end', this._socketCloseHandler);
    this.socket.on('close', this._socketCloseHandler);

    this._resolved = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router"></a>[function <span class="apidocSignatureSpan">websocket.</span>router (config)](#apidoc.element.websocket.router)
- description and source-code
```javascript
function WebSocketRouter(config) {
    // Superclass Constructor
    EventEmitter.call(this);

    this.config = {
        // The WebSocketServer instance to attach to.
        server: null
    };
    if (config) {
        extend(this.config, config);
    }
    this.handlers = [];

    this._requestHandler = this.handleRequest.bind(this);
    if (this.config.server) {
        this.attachServer(this.config.server);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server"></a>[function <span class="apidocSignatureSpan">websocket.</span>server (config)](#apidoc.element.websocket.server)
- description and source-code
```javascript
function WebSocketServer(config) {
    // Superclass Constructor
    EventEmitter.call(this);

    this._handlers = {
        upgrade: this.handleUpgrade.bind(this),
        requestAccepted: this.handleRequestAccepted.bind(this),
        requestResolved: this.handleRequestResolved.bind(this)
    };
    this.connections = [];
    this.pendingRequests = [];
    if (config) {
        this.mount(config);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.w3cwebsocket"></a>[function <span class="apidocSignatureSpan">websocket.</span>w3cwebsocket (url, protocols, origin, headers, requestOptions, clientConfig)](#apidoc.element.websocket.w3cwebsocket)
- description and source-code
```javascript
function W3CWebSocket(url, protocols, origin, headers, requestOptions, clientConfig) {
    // Make this an EventTarget.
    yaeti.EventTarget.call(this);

    // Sanitize clientConfig.
    clientConfig = clientConfig || {};
    clientConfig.assembleFragments = true;  // Required in the W3C API.

    var self = this;

    this._url = url;
    this._readyState = CONNECTING;
    this._protocol = undefined;
    this._extensions = '';
    this._bufferedAmount = 0;  // Hack, always 0.
    this._binaryType = 'arraybuffer';  // TODO: Should be 'blob' by default, but Node has no Blob.

    // The WebSocketConnection instance.
    this._connection = undefined;

    // WebSocketClient instance.
    this._client = new WebSocketClient(clientConfig);

    this._client.on('connect', function(connection) {
        onConnect.call(self, connection);
    });

    this._client.on('connectFailed', function() {
        onConnectFailed.call(self);
    });

    this._client.connect(url, protocols, origin, headers, requestOptions);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.client"></a>[module websocket.client](#apidoc.module.websocket.client)

#### <a name="apidoc.element.websocket.client.client"></a>[function <span class="apidocSignatureSpan">websocket.</span>client (config)](#apidoc.element.websocket.client.client)
- description and source-code
```javascript
function WebSocketClient(config) {
    // Superclass Constructor
    EventEmitter.call(this);

    // TODO: Implement extensions

    this.config = {
        // 1MiB max frame size.
        maxReceivedFrameSize: 0x100000,

        // 8MiB max message size, only applicable if
        // assembleFragments is true
        maxReceivedMessageSize: 0x800000,

        // Outgoing messages larger than fragmentationThreshold will be
        // split into multiple fragments.
        fragmentOutgoingMessages: true,

        // Outgoing frames are fragmented if they exceed this threshold.
        // Default is 16KiB
        fragmentationThreshold: 0x4000,

        // Which version of the protocol to use for this session.  This
        // option will be removed once the protocol is finalized by the IETF
        // It is only available to ease the transition through the
        // intermediate draft protocol versions.
        // At present, it only affects the name of the Origin header.
        webSocketVersion: 13,

        // If true, fragmented messages will be automatically assembled
        // and the full message will be emitted via a 'message' event.
        // If false, each frame will be emitted via a 'frame' event and
        // the application will be responsible for aggregating multiple
        // fragmented frames.  Single-frame messages will emit a 'message'
        // event in addition to the 'frame' event.
        // Most users will want to leave this set to 'true'
        assembleFragments: true,

        // The Nagle Algorithm makes more efficient use of network resources
        // by introducing a small delay before sending small packets so that
        // multiple messages can be batched together before going onto the
        // wire.  This however comes at the cost of latency, so the default
        // is to disable it.  If you don't need low latency and are streaming
        // lots of small messages, you can change this to 'false'
        disableNagleAlgorithm: true,

        // The number of milliseconds to wait after sending a close frame
        // for an acknowledgement to come back before giving up and just
        // closing the socket.
        closeTimeout: 5000,

        // Options to pass to https.connect if connecting via TLS
        tlsOptions: {}
    };

    if (config) {
        var tlsOptions;
        if (config.tlsOptions) {
          tlsOptions = config.tlsOptions;
          delete config.tlsOptions;
        }
        else {
          tlsOptions = {};
        }
        extend(this.config, config);
        extend(this.config.tlsOptions, tlsOptions);
    }

    this._req = null;

    switch (this.config.webSocketVersion) {
        case 8:
        case 13:
            break;
        default:
            throw new Error('Requested webSocketVersion is not supported. Allowed values are 8 and 13.');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.client.super_"></a>[function <span class="apidocSignatureSpan">websocket.client.</span>super_ ()](#apidoc.element.websocket.client.super_)
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



# <a name="apidoc.module.websocket.client.prototype"></a>[module websocket.client.prototype](#apidoc.module.websocket.client.prototype)

#### <a name="apidoc.element.websocket.client.prototype.abort"></a>[function <span class="apidocSignatureSpan">websocket.client.prototype.</span>abort ()](#apidoc.element.websocket.client.prototype.abort)
- description and source-code
```javascript
abort = function () {
    if (this._req) {
        this._req.abort();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.client.prototype.connect"></a>[function <span class="apidocSignatureSpan">websocket.client.prototype.</span>connect (requestUrl, protocols, origin, headers, extraRequestOptions)](#apidoc.element.websocket.client.prototype.connect)
- description and source-code
```javascript
connect = function (requestUrl, protocols, origin, headers, extraRequestOptions) {
    var self = this;
    if (typeof(protocols) === 'string') {
        if (protocols.length > 0) {
            protocols = [protocols];
        }
        else {
            protocols = [];
        }
    }
    if (!(protocols instanceof Array)) {
        protocols = [];
    }
    this.protocols = protocols;
    this.origin = origin;

    if (typeof(requestUrl) === 'string') {
        this.url = url.parse(requestUrl);
    }
    else {
        this.url = requestUrl; // in case an already parsed url is passed in.
    }
    if (!this.url.protocol) {
        throw new Error('You must specify a full WebSocket URL, including protocol.');
    }
    if (!this.url.host) {
        throw new Error('You must specify a full WebSocket URL, including hostname. Relative URLs are not supported.');
    }

    this.secure = (this.url.protocol === 'wss:');

    // validate protocol characters:
    this.protocols.forEach(function(protocol) {
        for (var i=0; i < protocol.length; i ++) {
            var charCode = protocol.charCodeAt(i);
            var character = protocol.charAt(i);
            if (charCode < 0x0021 || charCode > 0x007E || protocolSeparators.indexOf(character) !== -1) {
                throw new Error('Protocol list contains invalid character "' + String.fromCharCode(charCode) + '"');
            }
        }
    });

    var defaultPorts = {
        'ws:': '80',
        'wss:': '443'
    };

    if (!this.url.port) {
        this.url.port = defaultPorts[this.url.protocol];
    }

    var nonce = new Buffer(16);
    for (var i=0; i < 16; i++) {
        nonce[i] = Math.round(Math.random()*0xFF);
    }
    this.base64nonce = nonce.toString('base64');

    var hostHeaderValue = this.url.hostname;
    if ((this.url.protocol === 'ws:' && this.url.port !== '80') ||
        (this.url.protocol === 'wss:' && this.url.port !== '443'))  {
        hostHeaderValue += (':' + this.url.port);
    }

    var reqHeaders = headers || {};
    extend(reqHeaders, {
        'Upgrade': 'websocket',
        'Connection': 'Upgrade',
        'Sec-WebSocket-Version': this.config.webSocketVersion.toString(10),
        'Sec-WebSocket-Key': this.base64nonce,
        'Host': hostHeaderValue
    });

    if (this.protocols.length > 0) {
        reqHeaders['Sec-WebSocket-Protocol'] = this.protocols.join(', ');
    }
    if (this.origin) {
        if (this.config.webSocketVersion === 13) {
            reqHeaders['Origin'] = this.origin;
        }
        else if (this.config.webSocketVersion === 8) {
            reqHeaders['Sec-WebSocket-Origin'] = this.origin;
        }
    }

    // TODO: Implement extensions

    var pathAndQuery;
    // Ensure it begins with '/'.
    if (this.url.pathname) {
        pathAndQuery = this.url.path;
    }
    else if (this.url.path) {
        pathAndQuery = '/' + this.url.path;
    }
    else {
        pathAndQuery = '/';
    }

    function handleRequestError(error) {
        self._req = null;
        self.emit('connectFailed', error);
    }

    var requestOptions = {
        agent: false
    };
    if (extraRequestOptions) {
        extend(requestOptions, extraRequestOptions);
    }
    // These options are always overridden by the library.  The user is not
    // allowed to specify these directly.
    extend(requestOptions, {
        hostname: this.url.hostname,
        port: this.url.port,
        method: 'GET',
        path: pathAndQuery,
        headers: reqHeaders
    });
    if (this.secure) {
       for (var key in self.config.tlsOptions) {
           if (self.config.tlsOptions.hasOwnProperty(key)) {
               requestOptions[key] = self.config.tlsOptions[key];
           }
       }
    }

    var req = this._req = (this.secure ? https : http).request(requestOptions);
    req.on('upgrade', function handleRequestUpgrade(response, socket, head) {
        self._req = null;
        req.removeListener('error', handleRequestError);
        self.socket = socket;
        self.response = response;
        self.firstDataChunk = head;
        self. ...
```
- example usage
```shell
...
            connection.sendUTF(number.toString());
            setTimeout(sendNumber, 1000);
        }
    }
    sendNumber();
});

client.connect('ws://localhost:8080/', 'echo-protocol');
'''

Client Example using the *W3C WebSocket API*
--------------------------------------------

Same example as above but using the [W3C WebSocket API](http://www.w3.org/TR/websockets/).
...
```

#### <a name="apidoc.element.websocket.client.prototype.failHandshake"></a>[function <span class="apidocSignatureSpan">websocket.client.prototype.</span>failHandshake (errorDescription)](#apidoc.element.websocket.client.prototype.failHandshake)
- description and source-code
```javascript
failHandshake = function (errorDescription) {
    if (this.socket && this.socket.writable) {
        this.socket.end();
    }
    this.emit('connectFailed', new Error(errorDescription));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.client.prototype.succeedHandshake"></a>[function <span class="apidocSignatureSpan">websocket.client.prototype.</span>succeedHandshake ()](#apidoc.element.websocket.client.prototype.succeedHandshake)
- description and source-code
```javascript
succeedHandshake = function () {
    var connection = new WebSocketConnection(this.socket, [], this.protocol, true, this.config);

    connection.webSocketVersion = this.config.webSocketVersion;
    connection._addSocketEventListeners();

    this.emit('connect', connection);
    if (this.firstDataChunk.length > 0) {
        connection.handleSocketData(this.firstDataChunk);
    }
    this.firstDataChunk = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.client.prototype.validateHandshake"></a>[function <span class="apidocSignatureSpan">websocket.client.prototype.</span>validateHandshake ()](#apidoc.element.websocket.client.prototype.validateHandshake)
- description and source-code
```javascript
validateHandshake = function () {
    var headers = this.response.headers;

    if (this.protocols.length > 0) {
        this.protocol = headers['sec-websocket-protocol'];
        if (this.protocol) {
            if (this.protocols.indexOf(this.protocol) === -1) {
                this.failHandshake('Server did not respond with a requested protocol.');
                return;
            }
        }
        else {
            this.failHandshake('Expected a Sec-WebSocket-Protocol header.');
            return;
        }
    }

    if (!(headers['connection'] && headers['connection'].toLocaleLowerCase() === 'upgrade')) {
        this.failHandshake('Expected a Connection: Upgrade header from the server');
        return;
    }

    if (!(headers['upgrade'] && headers['upgrade'].toLocaleLowerCase() === 'websocket')) {
        this.failHandshake('Expected an Upgrade: websocket header from the server');
        return;
    }

    var sha1 = crypto.createHash('sha1');
    sha1.update(this.base64nonce + '258EAFA5-E914-47DA-95CA-C5AB0DC85B11');
    var expectedKey = sha1.digest('base64');

    if (!headers['sec-websocket-accept']) {
        this.failHandshake('Expected Sec-WebSocket-Accept header from server');
        return;
    }

    if (headers['sec-websocket-accept'] !== expectedKey) {
        this.failHandshake('Sec-WebSocket-Accept header from server didn\'t match expected value of ' + expectedKey);
        return;
    }

    // TODO: Support extensions

    this.succeedHandshake();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.connection"></a>[module websocket.connection](#apidoc.module.websocket.connection)

#### <a name="apidoc.element.websocket.connection.connection"></a>[function <span class="apidocSignatureSpan">websocket.</span>connection (socket, extensions, protocol, maskOutgoingPackets, config)](#apidoc.element.websocket.connection.connection)
- description and source-code
```javascript
function WebSocketConnection(socket, extensions, protocol, maskOutgoingPackets, config) {
    this._debug = utils.BufferingLogger('websocket:connection', ++idCounter);
    this._debug('constructor');

    if (this._debug.enabled) {
        instrumentSocketForDebugging(this, socket);
    }

    // Superclass Constructor
    EventEmitter.call(this);

    this._pingListenerCount = 0;
    this.on('newListener', function(ev) {
        if (ev === 'ping'){
            this._pingListenerCount++;
        }
      }).on('removeListener', function(ev) {
        if (ev === 'ping') {
            this._pingListenerCount--;
        }
    });

    this.config = config;
    this.socket = socket;
    this.protocol = protocol;
    this.extensions = extensions;
    this.remoteAddress = socket.remoteAddress;
    this.closeReasonCode = -1;
    this.closeDescription = null;
    this.closeEventEmitted = false;

    // We have to mask outgoing packets if we're acting as a WebSocket client.
    this.maskOutgoingPackets = maskOutgoingPackets;

    // We re-use the same buffers for the mask and frame header for all frames
    // received on each connection to avoid a small memory allocation for each
    // frame.
    this.maskBytes = new Buffer(4);
    this.frameHeader = new Buffer(10);

    // the BufferList will handle the data streaming in
    this.bufferList = new BufferList();

    // Prepare for receiving first frame
    this.currentFrame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);
    this.fragmentationSize = 0; // data received so far...
    this.frameQueue = [];

    // Various bits of connection state
    this.connected = true;
    this.state = STATE_OPEN;
    this.waitingForCloseResponse = false;
    // Received TCP FIN, socket's readable stream is finished.
    this.receivedEnd = false;

    this.closeTimeout = this.config.closeTimeout;
    this.assembleFragments = this.config.assembleFragments;
    this.maxReceivedMessageSize = this.config.maxReceivedMessageSize;

    this.outputBufferFull = false;
    this.inputPaused = false;
    this.receivedDataHandler = this.processReceivedData.bind(this);
    this._closeTimerHandler = this.handleCloseTimer.bind(this);

    // Disable nagle algorithm?
    this.socket.setNoDelay(this.config.disableNagleAlgorithm);

    // Make sure there is no socket inactivity timeout
    this.socket.setTimeout(0);

    if (this.config.keepalive && !this.config.useNativeKeepalive) {
        if (typeof(this.config.keepaliveInterval) !== 'number') {
            throw new Error('keepaliveInterval must be specified and numeric ' +
                            'if keepalive is true.');
        }
        this._keepaliveTimerHandler = this.handleKeepaliveTimer.bind(this);
        this.setKeepaliveTimer();

        if (this.config.dropConnectionOnKeepaliveTimeout) {
            if (typeof(this.config.keepaliveGracePeriod) !== 'number') {
                throw new Error('keepaliveGracePeriod  must be specified and ' +
                                'numeric if dropConnectionOnKeepaliveTimeout ' +
                                'is true.');
            }
            this._gracePeriodTimerHandler = this.handleGracePeriodTimer.bind(this);
        }
    }
    else if (this.config.keepalive && this.config.useNativeKeepalive) {
        if (!('setKeepAlive' in this.socket)) {
            throw new Error('Unable to use native keepalive: unsupported by ' +
                            'this version of Node.');
        }
        this.socket.setKeepAlive(true, this.config.keepaliveInterval);
    }

    // The HTTP Client seems to subscribe to socket error events
    // and re-dispatch them in such a way that doesn't make sense
    // for users of our client, so we want to make sure nobody
    // else is listening for error events on the socket besides us.
    this.socket.removeAllListeners('error');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.super_"></a>[function <span class="apidocSignatureSpan">websocket.connection.</span>super_ ()](#apidoc.element.websocket.connection.super_)
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



# <a name="apidoc.module.websocket.connection.prototype"></a>[module websocket.connection.prototype](#apidoc.module.websocket.connection.prototype)

#### <a name="apidoc.element.websocket.connection.prototype._addSocketEventListeners"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>_addSocketEventListeners ()](#apidoc.element.websocket.connection.prototype._addSocketEventListeners)
- description and source-code
```javascript
_addSocketEventListeners = function () {
    this.socket.on('error', this.handleSocketError.bind(this));
    this.socket.on('end', this.handleSocketEnd.bind(this));
    this.socket.on('close', this.handleSocketClose.bind(this));
    this.socket.on('drain', this.handleSocketDrain.bind(this));
    this.socket.on('pause', this.handleSocketPause.bind(this));
    this.socket.on('resume', this.handleSocketResume.bind(this));
    this.socket.on('data', this.handleSocketData.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.clearCloseTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>clearCloseTimer ()](#apidoc.element.websocket.connection.prototype.clearCloseTimer)
- description and source-code
```javascript
clearCloseTimer = function () {
    this._debug('clearCloseTimer');
    if (this.closeTimer) {
        this._debug('Clearing close timer');
        clearTimeout(this.closeTimer);
        this.waitingForCloseResponse = false;
        this.closeTimer = null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.clearGracePeriodTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>clearGracePeriodTimer ()](#apidoc.element.websocket.connection.prototype.clearGracePeriodTimer)
- description and source-code
```javascript
clearGracePeriodTimer = function () {
    if (this._gracePeriodTimeoutID) {
        clearTimeout(this._gracePeriodTimeoutID);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.clearKeepaliveTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>clearKeepaliveTimer ()](#apidoc.element.websocket.connection.prototype.clearKeepaliveTimer)
- description and source-code
```javascript
clearKeepaliveTimer = function () {
    if (this._keepaliveTimeoutID) {
        clearTimeout(this._keepaliveTimeoutID);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.close"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>close (reasonCode, description)](#apidoc.element.websocket.connection.prototype.close)
- description and source-code
```javascript
close = function (reasonCode, description) {
    if (this.connected) {
        this._debug('close: Initating clean WebSocket close sequence.');
        if ('number' !== typeof reasonCode) {
            reasonCode = WebSocketConnection.CLOSE_REASON_NORMAL;
        }
        if (!validateCloseReason(reasonCode)) {
            throw new Error('Close code ' + reasonCode + ' is not valid.');
        }
        if ('string' !== typeof description) {
            description = WebSocketConnection.CLOSE_DESCRIPTIONS[reasonCode];
        }
        this.closeReasonCode = reasonCode;
        this.closeDescription = description;
        this.setCloseTimer();
        this.sendCloseFrame(this.closeReasonCode, this.closeDescription);
        this.state = STATE_ENDING;
        this.connected = false;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.drop"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>drop (reasonCode, description, skipCloseFrame)](#apidoc.element.websocket.connection.prototype.drop)
- description and source-code
```javascript
drop = function (reasonCode, description, skipCloseFrame) {
    this._debug('drop');
    if (typeof(reasonCode) !== 'number') {
        reasonCode = WebSocketConnection.CLOSE_REASON_PROTOCOL_ERROR;
    }

    if (typeof(description) !== 'string') {
        // If no description is provided, try to look one up based on the
        // specified reasonCode.
        description = WebSocketConnection.CLOSE_DESCRIPTIONS[reasonCode];
    }

    this._debug('Forcefully dropping connection. skipCloseFrame: %s, code: %d, description: %s',
        skipCloseFrame, reasonCode, description
    );

    this.closeReasonCode = reasonCode;
    this.closeDescription = description;
    this.frameQueue = [];
    this.fragmentationSize = 0;
    if (!skipCloseFrame) {
        this.sendCloseFrame(reasonCode, description);
    }
    this.connected = false;
    this.state = STATE_CLOSED;
    this.clearCloseTimer();
    this.clearKeepaliveTimer();
    this.clearGracePeriodTimer();

    if (!this.closeEventEmitted) {
        this.closeEventEmitted = true;
        this._debug('Emitting WebSocketConnection close event');
        this.emit('close', this.closeReasonCode, this.closeDescription);
    }

    this._debug('Drop: destroying socket');
    this.socket.destroy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.fragmentAndSend"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>fragmentAndSend (frame, cb)](#apidoc.element.websocket.connection.prototype.fragmentAndSend)
- description and source-code
```javascript
fragmentAndSend = function (frame, cb) {
    this._debug('fragmentAndSend');
    if (frame.opcode > 0x07) {
        throw new Error('You cannot fragment control frames.');
    }

    var threshold = this.config.fragmentationThreshold;
    var length = frame.binaryPayload.length;

    // Send immediately if fragmentation is disabled or the message is not
    // larger than the fragmentation threshold.
    if (!this.config.fragmentOutgoingMessages || (frame.binaryPayload && length <= threshold)) {
        frame.fin = true;
        this.sendFrame(frame, cb);
        return;
    }

    var numFragments = Math.ceil(length / threshold);
    var sentFragments = 0;
    var sentCallback = function fragmentSentCallback(err) {
        if (err) {
            if (typeof cb === 'function') {
                // pass only the first error
                cb(err);
                cb = null;
            }
            return;
        }
        ++sentFragments;
        if ((sentFragments === numFragments) && (typeof cb === 'function')) {
            cb();
        }
    };
    for (var i=1; i <= numFragments; i++) {
        var currentFrame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);

        // continuation opcode except for first frame.
        currentFrame.opcode = (i === 1) ? frame.opcode : 0x00;

        // fin set on last frame only
        currentFrame.fin = (i === numFragments);

        // length is likely to be shorter on the last fragment
        var currentLength = (i === numFragments) ? length - (threshold * (i-1)) : threshold;
        var sliceStart = threshold * (i-1);

        // Slice the right portion of the original payload
        currentFrame.binaryPayload = frame.binaryPayload.slice(sliceStart, sliceStart + currentLength);

        this.sendFrame(currentFrame, sentCallback);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleCloseTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleCloseTimer ()](#apidoc.element.websocket.connection.prototype.handleCloseTimer)
- description and source-code
```javascript
handleCloseTimer = function () {
    this._debug('handleCloseTimer');
    this.closeTimer = null;
    if (this.waitingForCloseResponse) {
        this._debug('Close response not received from client.  Forcing socket end.');
        this.waitingForCloseResponse = false;
        this.state = STATE_CLOSED;
        this.socket.end();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleGracePeriodTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleGracePeriodTimer ()](#apidoc.element.websocket.connection.prototype.handleGracePeriodTimer)
- description and source-code
```javascript
handleGracePeriodTimer = function () {
    this._debug('handleGracePeriodTimer');
    // If this is called, the client has not responded and is assumed dead.
    this._gracePeriodTimeoutID = null;
    this.drop(WebSocketConnection.CLOSE_REASON_ABNORMAL, 'Peer not responding.', true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleKeepaliveTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleKeepaliveTimer ()](#apidoc.element.websocket.connection.prototype.handleKeepaliveTimer)
- description and source-code
```javascript
handleKeepaliveTimer = function () {
    this._debug('handleKeepaliveTimer');
    this._keepaliveTimeoutID = null;
    this.ping();

    // If we are configured to drop connections if the client doesn't respond
    // then set the grace period timer.
    if (this.config.dropConnectionOnKeepaliveTimeout) {
        this.setGracePeriodTimer();
    }
    else {
        // Otherwise reset the keepalive timer to send the next ping.
        this.setKeepaliveTimer();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleSocketClose"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketClose (hadError)](#apidoc.element.websocket.connection.prototype.handleSocketClose)
- description and source-code
```javascript
handleSocketClose = function (hadError) {
    this._debug('handleSocketClose: received socket close');
    this.socketHadError = hadError;
    this.connected = false;
    this.state = STATE_CLOSED;
    // If closeReasonCode is still set to -1 at this point then we must
    // not have received a close frame!!
    if (this.closeReasonCode === -1) {
        this.closeReasonCode = WebSocketConnection.CLOSE_REASON_ABNORMAL;
        this.closeDescription = 'Connection dropped by remote peer.';
    }
    this.clearCloseTimer();
    this.clearKeepaliveTimer();
    this.clearGracePeriodTimer();
    if (!this.closeEventEmitted) {
        this.closeEventEmitted = true;
        this._debug('-- Emitting WebSocketConnection close event');
        this.emit('close', this.closeReasonCode, this.closeDescription);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleSocketData"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketData (data)](#apidoc.element.websocket.connection.prototype.handleSocketData)
- description and source-code
```javascript
handleSocketData = function (data) {
    this._debug('handleSocketData');
    // Reset the keepalive timer when receiving data of any kind.
    this.setKeepaliveTimer();

    // Add received data to our bufferList, which efficiently holds received
    // data chunks in a linked list of Buffer objects.
    this.bufferList.write(data);

    this.processReceivedData();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleSocketDrain"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketDrain ()](#apidoc.element.websocket.connection.prototype.handleSocketDrain)
- description and source-code
```javascript
handleSocketDrain = function () {
    this._debug('handleSocketDrain: socket drain event');
    this.outputBufferFull = false;
    this.emit('drain');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleSocketEnd"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketEnd ()](#apidoc.element.websocket.connection.prototype.handleSocketEnd)
- description and source-code
```javascript
handleSocketEnd = function () {
    this._debug('handleSocketEnd: received socket end.  state = %s', this.state);
    this.receivedEnd = true;
    if (this.state === STATE_CLOSED) {
        // When using the TLS module, sometimes the socket will emit 'end'
        // after it emits 'close'.  I don't think that's correct behavior,
        // but we should deal with it gracefully by ignoring it.
        this._debug('  --- Socket \'end\' after \'close\'');
        return;
    }
    if (this.state !== STATE_PEER_REQUESTED_CLOSE &&
        this.state !== STATE_ENDING) {
      this._debug('  --- UNEXPECTED socket end.');
      this.socket.end();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleSocketError"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketError (error)](#apidoc.element.websocket.connection.prototype.handleSocketError)
- description and source-code
```javascript
handleSocketError = function (error) {
    this._debug('handleSocketError: %j', error);
    this.closeReasonCode = WebSocketConnection.CLOSE_REASON_ABNORMAL;
    this.closeDescription = 'Socket Error: ' + error.syscall + ' ' + error.code;
    this.connected = false;
    this.state = STATE_CLOSED;
    this.fragmentationSize = 0;
    if (utils.eventEmitterListenerCount(this, 'error') > 0) {
        this.emit('error', error);
    }
    this.socket.destroy(error);
    this._debug.printOutput();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleSocketPause"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketPause ()](#apidoc.element.websocket.connection.prototype.handleSocketPause)
- description and source-code
```javascript
handleSocketPause = function () {
    this._debug('handleSocketPause: socket pause event');
    this.inputPaused = true;
    this.emit('pause');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.handleSocketResume"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>handleSocketResume ()](#apidoc.element.websocket.connection.prototype.handleSocketResume)
- description and source-code
```javascript
handleSocketResume = function () {
    this._debug('handleSocketResume: socket resume event');
    this.inputPaused = false;
    this.emit('resume');
    this.processReceivedData();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.pause"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>pause ()](#apidoc.element.websocket.connection.prototype.pause)
- description and source-code
```javascript
pause = function () {
    this._debug('pause: pause requested');
    this.socket.pause();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.ping"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>ping (data)](#apidoc.element.websocket.connection.prototype.ping)
- description and source-code
```javascript
ping = function (data) {
    this._debug('ping');
    var frame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);
    frame.opcode = 0x09; // WebSocketOpcode.PING
    frame.fin = true;
    if (data) {
        if (!Buffer.isBuffer(data)) {
            data = new Buffer(data.toString(), 'utf8');
        }
        if (data.length > 125) {
            this._debug('WebSocket: Data for ping is longer than 125 bytes.  Truncating.');
            data = data.slice(0,124);
        }
        frame.binaryPayload = data;
    }
    this.sendFrame(frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.pong"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>pong (binaryPayload)](#apidoc.element.websocket.connection.prototype.pong)
- description and source-code
```javascript
pong = function (binaryPayload) {
    this._debug('pong');
    var frame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);
    frame.opcode = 0x0A; // WebSocketOpcode.PONG
    if (Buffer.isBuffer(binaryPayload) && binaryPayload.length > 125) {
        this._debug('WebSocket: Data for pong is longer than 125 bytes.  Truncating.');
        binaryPayload = binaryPayload.slice(0,124);
    }
    frame.binaryPayload = binaryPayload;
    frame.fin = true;
    this.sendFrame(frame);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.processFrame"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>processFrame (frame)](#apidoc.element.websocket.connection.prototype.processFrame)
- description and source-code
```javascript
processFrame = function (frame) {
    this._debug('processFrame');
    this._debug(' -- frame: %s', frame);

    // Any non-control opcode besides 0x00 (continuation) received in the
    // middle of a fragmented message is illegal.
    if (this.frameQueue.length !== 0 && (frame.opcode > 0x00 && frame.opcode < 0x08)) {
        this.drop(WebSocketConnection.CLOSE_REASON_PROTOCOL_ERROR,
          'Illegal frame opcode 0x' + frame.opcode.toString(16) + ' ' +
          'received in middle of fragmented message.');
        return;
    }

    switch(frame.opcode) {
        case 0x02: // WebSocketFrame.BINARY_FRAME
            this._debug('-- Binary Frame');
            if (this.assembleFragments) {
                if (frame.fin) {
                    // Complete single-frame message received
                    this._debug('---- Emitting \'message\' event');
                    this.emit('message', {
                        type: 'binary',
                        binaryData: frame.binaryPayload
                    });
                }
                else {
                    // beginning of a fragmented message
                    this.frameQueue.push(frame);
                    this.fragmentationSize = frame.length;
                }
            }
            break;
        case 0x01: // WebSocketFrame.TEXT_FRAME
            this._debug('-- Text Frame');
            if (this.assembleFragments) {
                if (frame.fin) {
                    if (!Validation.isValidUTF8(frame.binaryPayload)) {
                        this.drop(WebSocketConnection.CLOSE_REASON_INVALID_DATA,
                          'Invalid UTF-8 Data Received');
                        return;
                    }
                    // Complete single-frame message received
                    this._debug('---- Emitting \'message\' event');
                    this.emit('message', {
                        type: 'utf8',
                        utf8Data: frame.binaryPayload.toString('utf8')
                    });
                }
                else {
                    // beginning of a fragmented message
                    this.frameQueue.push(frame);
                    this.fragmentationSize = frame.length;
                }
            }
            break;
        case 0x00: // WebSocketFrame.CONTINUATION
            this._debug('-- Continuation Frame');
            if (this.assembleFragments) {
                if (this.frameQueue.length === 0) {
                    this.drop(WebSocketConnection.CLOSE_REASON_PROTOCOL_ERROR,
                      'Unexpected Continuation Frame');
                    return;
                }

                this.fragmentationSize += frame.length;

                if (this.fragmentationSize > this.maxReceivedMessageSize) {
                    this.drop(WebSocketConnection.CLOSE_REASON_MESSAGE_TOO_BIG,
                      'Maximum message size exceeded.');
                    return;
                }

                this.frameQueue.push(frame);

                if (frame.fin) {
                    // end of fragmented message, so we process the whole
                    // message now.  We also have to decode the utf-8 data
                    // for text frames after combining all the fragments.
                    var bytesCopied = 0;
                    var binaryPayload = new Buffer(this.fragmentationSize);
                    var opcode = this.frameQueue[0].opcode;
                    this.frameQueue.forEach(function (currentFrame) {
                        currentFrame.binaryPayload.copy(binaryPayload, bytesCopied);
                        bytesCopied += currentFrame.binaryPayload.length;
                    });
                    this.frameQueue = [];
                    this.fragmentationSize = 0;

                    switch (opcode) {
                        case 0x02: // WebSocketOpcode.BINARY_FRAME
                            this.emit('message', {
                                type: 'binary',
                                binaryData: binaryPayload
                            }); ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.processReceivedData"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>processReceivedData ()](#apidoc.element.websocket.connection.prototype.processReceivedData)
- description and source-code
```javascript
processReceivedData = function () {
    this._debug('processReceivedData');
    // If we're not connected, we should ignore any data remaining on the buffer.
    if (!this.connected) { return; }

    // Receiving/parsing is expected to be halted when paused.
    if (this.inputPaused) { return; }

    var frame = this.currentFrame;

    // WebSocketFrame.prototype.addData returns true if all data necessary to
    // parse the frame was available.  It returns false if we are waiting for
    // more data to come in on the wire.
    if (!frame.addData(this.bufferList)) { this._debug('-- insufficient data for frame'); return; }

    var self = this;

    // Handle possible parsing errors
    if (frame.protocolError) {
        // Something bad happened.. get rid of this client.
        this._debug('-- protocol error');
        process.nextTick(function() {
            self.drop(WebSocketConnection.CLOSE_REASON_PROTOCOL_ERROR, frame.dropReason);
        });
        return;
    }
    else if (frame.frameTooLarge) {
        this._debug('-- frame too large');
        process.nextTick(function() {
            self.drop(WebSocketConnection.CLOSE_REASON_MESSAGE_TOO_BIG, frame.dropReason);
        });
        return;
    }

    // For now since we don't support extensions, all RSV bits are illegal
    if (frame.rsv1 || frame.rsv2 || frame.rsv3) {
        this._debug('-- illegal rsv flag');
        process.nextTick(function() {
            self.drop(WebSocketConnection.CLOSE_REASON_PROTOCOL_ERROR,
              'Unsupported usage of rsv bits without negotiated extension.');
        });
        return;
    }

    if (!this.assembleFragments) {
        this._debug('-- emitting frame');
        process.nextTick(function() { self.emit('frame', frame); });
    }

    process.nextTick(function() { self.processFrame(frame); });

    this.currentFrame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);

    // If there's data remaining, schedule additional processing, but yield
    // for now so that other connections have a chance to have their data
    // processed.  We use setImmediate here instead of process.nextTick to
    // explicitly indicate that we wish for other I/O to be handled first.
    if (this.bufferList.length > 0) {
        setImmediateImpl(this.receivedDataHandler);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.resume"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>resume ()](#apidoc.element.websocket.connection.prototype.resume)
- description and source-code
```javascript
resume = function () {
    this._debug('resume: resume requested');
    this.socket.resume();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.send"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>send (data, cb)](#apidoc.element.websocket.connection.prototype.send)
- description and source-code
```javascript
send = function (data, cb) {
    this._debug('send');
    if (Buffer.isBuffer(data)) {
        this.sendBytes(data, cb);
    }
    else if (typeof(data['toString']) === 'function') {
        this.sendUTF(data, cb);
    }
    else {
        throw new Error('Data provided must either be a Node Buffer or implement toString()');
    }
}
```
- example usage
```shell
...

client.onopen = function() {
    console.log('WebSocket Client Connected');

    function sendNumber() {
        if (client.readyState === client.OPEN) {
            var number = Math.round(Math.random() * 0xFFFFFF);
            client.send(number.toString());
            setTimeout(sendNumber, 1000);
        }
    }
    sendNumber();
};

client.onclose = function() {
...
```

#### <a name="apidoc.element.websocket.connection.prototype.sendBytes"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendBytes (data, cb)](#apidoc.element.websocket.connection.prototype.sendBytes)
- description and source-code
```javascript
sendBytes = function (data, cb) {
    this._debug('sendBytes');
    if (!Buffer.isBuffer(data)) {
        throw new Error('You must pass a Node Buffer object to WebSocketConnection.prototype.sendBytes()');
    }
    var frame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);
    frame.opcode = 0x02; // WebSocketOpcode.BINARY_FRAME
    frame.binaryPayload = data;
    this.fragmentAndSend(frame, cb);
}
```
- example usage
```shell
...
    connection.on('message', function(message) {
        if (message.type === 'utf8') {
            console.log('Received Message: ' + message.utf8Data);
            connection.sendUTF(message.utf8Data);
        }
        else if (message.type === 'binary') {
            console.log('Received Binary Message of ' + message.binaryData.length + ' bytes');
            connection.sendBytes(message.binaryData);
        }
    });
    connection.on('close', function(reasonCode, description) {
        console.log((new Date()) + ' Peer ' + connection.remoteAddress + ' disconnected.');
    });
});
'''
...
```

#### <a name="apidoc.element.websocket.connection.prototype.sendCloseFrame"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendCloseFrame (reasonCode, description, cb)](#apidoc.element.websocket.connection.prototype.sendCloseFrame)
- description and source-code
```javascript
sendCloseFrame = function (reasonCode, description, cb) {
    if (typeof(reasonCode) !== 'number') {
        reasonCode = WebSocketConnection.CLOSE_REASON_NORMAL;
    }

    this._debug('sendCloseFrame state: %s, reasonCode: %d, description: %s', this.state, reasonCode, description);

    if (this.state !== STATE_OPEN && this.state !== STATE_PEER_REQUESTED_CLOSE) { return; }

    var frame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);
    frame.fin = true;
    frame.opcode = 0x08; // WebSocketOpcode.CONNECTION_CLOSE
    frame.closeStatus = reasonCode;
    if (typeof(description) === 'string') {
        frame.binaryPayload = new Buffer(description, 'utf8');
    }

    this.sendFrame(frame, cb);
    this.socket.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.sendFrame"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendFrame (frame, cb)](#apidoc.element.websocket.connection.prototype.sendFrame)
- description and source-code
```javascript
sendFrame = function (frame, cb) {
    this._debug('sendFrame');
    frame.mask = this.maskOutgoingPackets;
    var flushed = this.socket.write(frame.toBuffer(), cb);
    this.outputBufferFull = !flushed;
    return flushed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.sendUTF"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>sendUTF (data, cb)](#apidoc.element.websocket.connection.prototype.sendUTF)
- description and source-code
```javascript
sendUTF = function (data, cb) {
    data = new Buffer(data.toString(), 'utf8');
    this._debug('sendUTF: %d bytes', data.length);
    var frame = new WebSocketFrame(this.maskBytes, this.frameHeader, this.config);
    frame.opcode = 0x01; // WebSocketOpcode.TEXT_FRAME
    frame.binaryPayload = data;
    this.fragmentAndSend(frame, cb);
}
```
- example usage
```shell
...
}

var connection = request.accept('echo-protocol', request.origin);
console.log((new Date()) + ' Connection accepted.');
connection.on('message', function(message) {
    if (message.type === 'utf8') {
        console.log('Received Message: ' + message.utf8Data);
        connection.sendUTF(message.utf8Data);
    }
    else if (message.type === 'binary') {
        console.log('Received Binary Message of ' + message.binaryData.length + ' bytes');
        connection.sendBytes(message.binaryData);
    }
});
connection.on('close', function(reasonCode, description) {
...
```

#### <a name="apidoc.element.websocket.connection.prototype.setCloseTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>setCloseTimer ()](#apidoc.element.websocket.connection.prototype.setCloseTimer)
- description and source-code
```javascript
setCloseTimer = function () {
    this._debug('setCloseTimer');
    this.clearCloseTimer();
    this._debug('Setting close timer');
    this.waitingForCloseResponse = true;
    this.closeTimer = setTimeout(this._closeTimerHandler, this.closeTimeout);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.setGracePeriodTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>setGracePeriodTimer ()](#apidoc.element.websocket.connection.prototype.setGracePeriodTimer)
- description and source-code
```javascript
setGracePeriodTimer = function () {
    this._debug('setGracePeriodTimer');
    this.clearGracePeriodTimer();
    this._gracePeriodTimeoutID = setTimeout(this._gracePeriodTimerHandler, this.config.keepaliveGracePeriod);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.connection.prototype.setKeepaliveTimer"></a>[function <span class="apidocSignatureSpan">websocket.connection.prototype.</span>setKeepaliveTimer ()](#apidoc.element.websocket.connection.prototype.setKeepaliveTimer)
- description and source-code
```javascript
setKeepaliveTimer = function () {
    this._debug('setKeepaliveTimer');
    if (!this.config.keepalive  || this.config.useNativeKeepalive) { return; }
    this.clearKeepaliveTimer();
    this.clearGracePeriodTimer();
    this._keepaliveTimeoutID = setTimeout(this._keepaliveTimerHandler, this.config.keepaliveInterval);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.deprecation"></a>[module websocket.deprecation](#apidoc.module.websocket.deprecation)

#### <a name="apidoc.element.websocket.deprecation.warn"></a>[function <span class="apidocSignatureSpan">websocket.deprecation.</span>warn (deprecationName)](#apidoc.element.websocket.deprecation.warn)
- description and source-code
```javascript
warn = function (deprecationName) {
    if (!this.disableWarnings && this.deprecationWarningMap[deprecationName]) {
        console.warn('DEPRECATION WARNING: ' + this.deprecationWarningMap[deprecationName]);
        this.deprecationWarningMap[deprecationName] = false;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.frame"></a>[module websocket.frame](#apidoc.module.websocket.frame)

#### <a name="apidoc.element.websocket.frame.frame"></a>[function <span class="apidocSignatureSpan">websocket.</span>frame (maskBytes, frameHeader, config)](#apidoc.element.websocket.frame.frame)
- description and source-code
```javascript
function WebSocketFrame(maskBytes, frameHeader, config) {
    this.maskBytes = maskBytes;
    this.frameHeader = frameHeader;
    this.config = config;
    this.maxReceivedFrameSize = config.maxReceivedFrameSize;
    this.protocolError = false;
    this.frameTooLarge = false;
    this.invalidCloseFrameLength = false;
    this.parseState = DECODE_HEADER;
    this.closeStatus = -1;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.frame.prototype"></a>[module websocket.frame.prototype](#apidoc.module.websocket.frame.prototype)

#### <a name="apidoc.element.websocket.frame.prototype.addData"></a>[function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>addData (bufferList)](#apidoc.element.websocket.frame.prototype.addData)
- description and source-code
```javascript
addData = function (bufferList) {
    if (this.parseState === DECODE_HEADER) {
        if (bufferList.length >= 2) {
            bufferList.joinInto(this.frameHeader, 0, 0, 2);
            bufferList.advance(2);
            var firstByte = this.frameHeader[0];
            var secondByte = this.frameHeader[1];

            this.fin     = Boolean(firstByte  & 0x80);
            this.rsv1    = Boolean(firstByte  & 0x40);
            this.rsv2    = Boolean(firstByte  & 0x20);
            this.rsv3    = Boolean(firstByte  & 0x10);
            this.mask    = Boolean(secondByte & 0x80);

            this.opcode  = firstByte  & 0x0F;
            this.length = secondByte & 0x7F;

            // Control frame sanity check
            if (this.opcode >= 0x08) {
                if (this.length > 125) {
                    this.protocolError = true;
                    this.dropReason = 'Illegal control frame longer than 125 bytes.';
                    return true;
                }
                if (!this.fin) {
                    this.protocolError = true;
                    this.dropReason = 'Control frames must not be fragmented.';
                    return true;
                }
            }

            if (this.length === 126) {
                this.parseState = WAITING_FOR_16_BIT_LENGTH;
            }
            else if (this.length === 127) {
                this.parseState = WAITING_FOR_64_BIT_LENGTH;
            }
            else {
                this.parseState = WAITING_FOR_MASK_KEY;
            }
        }
    }
    if (this.parseState === WAITING_FOR_16_BIT_LENGTH) {
        if (bufferList.length >= 2) {
            bufferList.joinInto(this.frameHeader, 2, 0, 2);
            bufferList.advance(2);
            this.length = this.frameHeader.readUInt16BE(2, true);
            this.parseState = WAITING_FOR_MASK_KEY;
        }
    }
    else if (this.parseState === WAITING_FOR_64_BIT_LENGTH) {
        if (bufferList.length >= 8) {
            bufferList.joinInto(this.frameHeader, 2, 0, 8);
            bufferList.advance(8);
            var lengthPair = [
              this.frameHeader.readUInt32BE(2, true),
              this.frameHeader.readUInt32BE(2+4, true)
            ];

            if (lengthPair[0] !== 0) {
                this.protocolError = true;
                this.dropReason = 'Unsupported 64-bit length frame received';
                return true;
            }
            this.length = lengthPair[1];
            this.parseState = WAITING_FOR_MASK_KEY;
        }
    }

    if (this.parseState === WAITING_FOR_MASK_KEY) {
        if (this.mask) {
            if (bufferList.length >= 4) {
                bufferList.joinInto(this.maskBytes, 0, 0, 4);
                bufferList.advance(4);
                this.parseState = WAITING_FOR_PAYLOAD;
            }
        }
        else {
            this.parseState = WAITING_FOR_PAYLOAD;
        }
    }

    if (this.parseState === WAITING_FOR_PAYLOAD) {
        if (this.length > this.maxReceivedFrameSize) {
            this.frameTooLarge = true;
            this.dropReason = 'Frame size of ' + this.length.toString(10) +
                              ' bytes exceeds maximum accepted frame size';
            return true;
        }

        if (this.length === 0) {
            this.binaryPayload = new Buffer(0);
            this.parseState = COMPLETE;
            return true;
        }
        if (bufferList.length >= this.length) {
            this.binaryPayload = bufferList.take(this.length);
            bufferList.advance(this.length);
            if (this.mask) {
                bufferUtil.unmask(this.binaryPayload, this.maskBytes);
                // xor(this.binaryPayload, this.maskBytes, 0);
            }

            if (this.opcode === 0x08) { // WebSocketOpcode.CONNECTION_CLOSE
                if (this.length === 1) {
                    // Invalid length for a close frame.  Must be zero or at least two.
                    this.binaryPayload = new Buffer(0);
                    this.invalidCloseFrameLength = true;
                } ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.frame.prototype.throwAwayPayload"></a>[function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>throwAwayPayload (bufferList)](#apidoc.element.websocket.frame.prototype.throwAwayPayload)
- description and source-code
```javascript
throwAwayPayload = function (bufferList) {
    if (bufferList.length >= this.length) {
        bufferList.advance(this.length);
        this.parseState = COMPLETE;
        return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.frame.prototype.toBuffer"></a>[function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>toBuffer (nullMask)](#apidoc.element.websocket.frame.prototype.toBuffer)
- description and source-code
```javascript
toBuffer = function (nullMask) {
    var maskKey;
    var headerLength = 2;
    var data;
    var outputPos;
    var firstByte = 0x00;
    var secondByte = 0x00;

    if (this.fin) {
        firstByte |= 0x80;
    }
    if (this.rsv1) {
        firstByte |= 0x40;
    }
    if (this.rsv2) {
        firstByte |= 0x20;
    }
    if (this.rsv3) {
        firstByte |= 0x10;
    }
    if (this.mask) {
        secondByte |= 0x80;
    }

    firstByte |= (this.opcode & 0x0F);

    // the close frame is a special case because the close reason is
    // prepended to the payload data.
    if (this.opcode === 0x08) {
        this.length = 2;
        if (this.binaryPayload) {
            this.length += this.binaryPayload.length;
        }
        data = new Buffer(this.length);
        data.writeUInt16BE(this.closeStatus, 0, true);
        if (this.length > 2) {
            this.binaryPayload.copy(data, 2);
        }
    }
    else if (this.binaryPayload) {
        data = this.binaryPayload;
        this.length = data.length;
    }
    else {
        this.length = 0;
    }

    if (this.length <= 125) {
        // encode the length directly into the two-byte frame header
        secondByte |= (this.length & 0x7F);
    }
    else if (this.length > 125 && this.length <= 0xFFFF) {
        // Use 16-bit length
        secondByte |= 126;
        headerLength += 2;
    }
    else if (this.length > 0xFFFF) {
        // Use 64-bit length
        secondByte |= 127;
        headerLength += 8;
    }

    var output = new Buffer(this.length + headerLength + (this.mask ? 4 : 0));

    // write the frame header
    output[0] = firstByte;
    output[1] = secondByte;

    outputPos = 2;

    if (this.length > 125 && this.length <= 0xFFFF) {
        // write 16-bit length
        output.writeUInt16BE(this.length, outputPos, true);
        outputPos += 2;
    }
    else if (this.length > 0xFFFF) {
        // write 64-bit length
        output.writeUInt32BE(0x00000000, outputPos, true);
        output.writeUInt32BE(this.length, outputPos + 4, true);
        outputPos += 8;
    }

    if (this.mask) {
        maskKey = nullMask ? 0 : (Math.random()*0xFFFFFFFF) | 0;
        this.maskBytes.writeUInt32BE(maskKey, 0, true);

        // write the mask key
        this.maskBytes.copy(output, outputPos);
        outputPos += 4;

        if (data) {
          bufferUtil.mask(data, this.maskBytes, output, outputPos, this.length);
        }
    }
    else if (data) {
        data.copy(output, outputPos);
    }

    return output;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.frame.prototype.toString"></a>[function <span class="apidocSignatureSpan">websocket.frame.prototype.</span>toString ()](#apidoc.element.websocket.frame.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return 'Opcode: ' + this.opcode + ', fin: ' + this.fin + ', length: ' + this.length + ', hasPayload: ' + Boolean(this.binaryPayload
) + ', masked: ' + this.mask;
}
```
- example usage
```shell
...
'''javascript
#!/usr/bin/env node
var WebSocketClient = require('websocket').client;

var client = new WebSocketClient();

client.on('connectFailed', function(error) {
console.log('Connect Error: ' + error.toString());
});

client.on('connect', function(connection) {
console.log('WebSocket Client Connected');
connection.on('error', function(error) {
    console.log("Connection Error: " + error.toString());
});
...
```



# <a name="apidoc.module.websocket.request"></a>[module websocket.request](#apidoc.module.websocket.request)

#### <a name="apidoc.element.websocket.request.request"></a>[function <span class="apidocSignatureSpan">websocket.</span>request (socket, httpRequest, serverConfig)](#apidoc.element.websocket.request.request)
- description and source-code
```javascript
function WebSocketRequest(socket, httpRequest, serverConfig) {
    // Superclass Constructor
    EventEmitter.call(this);

    this.socket = socket;
    this.httpRequest = httpRequest;
    this.resource = httpRequest.url;
    this.remoteAddress = socket.remoteAddress;
    this.remoteAddresses = [this.remoteAddress];
    this.serverConfig = serverConfig;

    // Watch for the underlying TCP socket closing before we call accept
    this._socketIsClosing = false;
    this._socketCloseHandler = this._handleSocketCloseBeforeAccept.bind(this);
    this.socket.on('end', this._socketCloseHandler);
    this.socket.on('close', this._socketCloseHandler);

    this._resolved = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request.super_"></a>[function <span class="apidocSignatureSpan">websocket.request.</span>super_ ()](#apidoc.element.websocket.request.super_)
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



# <a name="apidoc.module.websocket.request.prototype"></a>[module websocket.request.prototype](#apidoc.module.websocket.request.prototype)

#### <a name="apidoc.element.websocket.request.prototype._handleSocketCloseBeforeAccept"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>_handleSocketCloseBeforeAccept ()](#apidoc.element.websocket.request.prototype._handleSocketCloseBeforeAccept)
- description and source-code
```javascript
_handleSocketCloseBeforeAccept = function () {
    this._socketIsClosing = true;
    this._removeSocketCloseListeners();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request.prototype._removeSocketCloseListeners"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>_removeSocketCloseListeners ()](#apidoc.element.websocket.request.prototype._removeSocketCloseListeners)
- description and source-code
```javascript
_removeSocketCloseListeners = function () {
    this.socket.removeListener('end', this._socketCloseHandler);
    this.socket.removeListener('close', this._socketCloseHandler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request.prototype._verifyResolution"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>_verifyResolution ()](#apidoc.element.websocket.request.prototype._verifyResolution)
- description and source-code
```javascript
_verifyResolution = function () {
    if (this._resolved) {
        throw new Error('WebSocketRequest may only be accepted or rejected one time.');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request.prototype.accept"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>accept (acceptedProtocol, allowedOrigin, cookies)](#apidoc.element.websocket.request.prototype.accept)
- description and source-code
```javascript
accept = function (acceptedProtocol, allowedOrigin, cookies) {
    this._verifyResolution();

    // TODO: Handle extensions

    var protocolFullCase;

    if (acceptedProtocol) {
        protocolFullCase = this.protocolFullCaseMap[acceptedProtocol.toLocaleLowerCase()];
        if (typeof(protocolFullCase) === 'undefined') {
            protocolFullCase = acceptedProtocol;
        }
    }
    else {
        protocolFullCase = acceptedProtocol;
    }
    this.protocolFullCaseMap = null;

    // Create key validation hash
    var sha1 = crypto.createHash('sha1');
    sha1.update(this.key + '258EAFA5-E914-47DA-95CA-C5AB0DC85B11');
    var acceptKey = sha1.digest('base64');

    var response = 'HTTP/1.1 101 Switching Protocols\r\n' +
                   'Upgrade: websocket\r\n' +
                   'Connection: Upgrade\r\n' +
                   'Sec-WebSocket-Accept: ' + acceptKey + '\r\n';

    if (protocolFullCase) {
        // validate protocol
        for (var i=0; i < protocolFullCase.length; i++) {
            var charCode = protocolFullCase.charCodeAt(i);
            var character = protocolFullCase.charAt(i);
            if (charCode < 0x21 || charCode > 0x7E || separators.indexOf(character) !== -1) {
                this.reject(500);
                throw new Error('Illegal character "' + String.fromCharCode(character) + '" in subprotocol.');
            }
        }
        if (this.requestedProtocols.indexOf(acceptedProtocol) === -1) {
            this.reject(500);
            throw new Error('Specified protocol was not requested by the client.');
        }

        protocolFullCase = protocolFullCase.replace(headerSanitizeRegExp, '');
        response += 'Sec-WebSocket-Protocol: ' + protocolFullCase + '\r\n';
    }
    this.requestedProtocols = null;

    if (allowedOrigin) {
        allowedOrigin = allowedOrigin.replace(headerSanitizeRegExp, '');
        if (this.webSocketVersion === 13) {
            response += 'Origin: ' + allowedOrigin + '\r\n';
        }
        else if (this.webSocketVersion === 8) {
            response += 'Sec-WebSocket-Origin: ' + allowedOrigin + '\r\n';
        }
    }

    if (cookies) {
        if (!Array.isArray(cookies)) {
            this.reject(500);
            throw new Error('Value supplied for "cookies" argument must be an array.');
        }
        var seenCookies = {};
        cookies.forEach(function(cookie) {
            if (!cookie.name || !cookie.value) {
                this.reject(500);
                throw new Error('Each cookie to set must at least provide a "name" and "value"');
            }

            // Make sure there are no \r\n sequences inserted
            cookie.name = cookie.name.replace(controlCharsAndSemicolonRegEx, '');
            cookie.value = cookie.value.replace(controlCharsAndSemicolonRegEx, '');

            if (seenCookies[cookie.name]) {
                this.reject(500);
                throw new Error('You may not specify the same cookie name twice.');
            }
            seenCookies[cookie.name] = true;

            // token (RFC 2616, Section 2.2)
            var invalidChar = cookie.name.match(cookieNameValidateRegEx);
            if (invalidChar) {
                this.reject(500);
                throw new Error('Illegal character ' + invalidChar[0] + ' in cookie name');
            }

            // RFC 6265, Section 4.1.1
            // *cookie-octet / ( DQUOTE *cookie-octet DQUOTE ) | %x21 / %x23-2B / %x2D-3A / %x3C-5B / %x5D-7E
            if (cookie.value.match(cookieValueDQuoteValidateRegEx)) {
                invalidChar = cookie.value.slice(1, -1).match(cookieValueValidateRegEx);
            } else {
                invalidChar = cookie.value.match(cookieValueValidateRegEx);
            }
            if (invalidChar) {
                this.reject(500);
                throw new Error('Illegal character ' + invalidChar[0] + ' in cookie value');
            }

            var cookieParts = [cookie.name + '=' + cookie.value];

            // RFC 6265, Section 4.1.1
            // 'Path=' path-value | <any CHAR except CTLs or ';' ...
```
- example usage
```shell
...
if (!originIsAllowed(request.origin)) {
  // Make sure we only accept requests from an allowed origin
  request.reject();
  console.log((new Date()) + ' Connection from origin ' + request.origin + ' rejected.');
  return;
}

var connection = request.accept('echo-protocol', request.origin);
console.log((new Date()) + ' Connection accepted.');
connection.on('message', function(message) {
    if (message.type === 'utf8') {
        console.log('Received Message: ' + message.utf8Data);
        connection.sendUTF(message.utf8Data);
    }
    else if (message.type === 'binary') {
...
```

#### <a name="apidoc.element.websocket.request.prototype.parseCookies"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>parseCookies (str)](#apidoc.element.websocket.request.prototype.parseCookies)
- description and source-code
```javascript
parseCookies = function (str) {
    // Sanity Check
    if (!str || typeof(str) !== 'string') {
        return [];
    }

    var cookies = [];
    var pairs = str.split(cookieSeparatorRegEx);

    pairs.forEach(function(pair) {
        var eq_idx = pair.indexOf('=');
        if (eq_idx === -1) {
            cookies.push({
                name: pair,
                value: null
            });
            return;
        }

        var key = pair.substr(0, eq_idx).trim();
        var val = pair.substr(++eq_idx, pair.length).trim();

        // quoted values
        if ('"' === val[0]) {
            val = val.slice(1, -1);
        }

        cookies.push({
            name: key,
            value: decodeURIComponent(val)
        });
    });

    return cookies;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request.prototype.parseExtensions"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>parseExtensions (extensionsString)](#apidoc.element.websocket.request.prototype.parseExtensions)
- description and source-code
```javascript
parseExtensions = function (extensionsString) {
    if (!extensionsString || extensionsString.length === 0) {
        return [];
    }
    var extensions = extensionsString.toLocaleLowerCase().split(headerValueSplitRegExp);
    extensions.forEach(function(extension, index, array) {
        var params = extension.split(headerParamSplitRegExp);
        var extensionName = params[0];
        var extensionParams = params.slice(1);
        extensionParams.forEach(function(rawParam, index, array) {
            var arr = rawParam.split('=');
            var obj = {
                name: arr[0],
                value: arr[1]
            };
            array.splice(index, 1, obj);
        });
        var obj = {
            name: extensionName,
            params: extensionParams
        };
        array.splice(index, 1, obj);
    });
    return extensions;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request.prototype.readHandshake"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>readHandshake ()](#apidoc.element.websocket.request.prototype.readHandshake)
- description and source-code
```javascript
readHandshake = function () {
    var self = this;
    var request = this.httpRequest;

    // Decode URL
    this.resourceURL = url.parse(this.resource, true);

    this.host = request.headers['host'];
    if (!this.host) {
        throw new Error('Client must provide a Host header.');
    }

    this.key = request.headers['sec-websocket-key'];
    if (!this.key) {
        throw new Error('Client must provide a value for Sec-WebSocket-Key.');
    }

    this.webSocketVersion = parseInt(request.headers['sec-websocket-version'], 10);

    if (!this.webSocketVersion || isNaN(this.webSocketVersion)) {
        throw new Error('Client must provide a value for Sec-WebSocket-Version.');
    }

    switch (this.webSocketVersion) {
        case 8:
        case 13:
            break;
        default:
            var e = new Error('Unsupported websocket client version: ' + this.webSocketVersion +
                              'Only versions 8 and 13 are supported.');
            e.httpCode = 426;
            e.headers = {
                'Sec-WebSocket-Version': '13'
            };
            throw e;
    }

    if (this.webSocketVersion === 13) {
        this.origin = request.headers['origin'];
    }
    else if (this.webSocketVersion === 8) {
        this.origin = request.headers['sec-websocket-origin'];
    }

    // Protocol is optional.
    var protocolString = request.headers['sec-websocket-protocol'];
    this.protocolFullCaseMap = {};
    this.requestedProtocols = [];
    if (protocolString) {
        var requestedProtocolsFullCase = protocolString.split(headerValueSplitRegExp);
        requestedProtocolsFullCase.forEach(function(protocol) {
            var lcProtocol = protocol.toLocaleLowerCase();
            self.requestedProtocols.push(lcProtocol);
            self.protocolFullCaseMap[lcProtocol] = protocol;
        });
    }

    if (!this.serverConfig.ignoreXForwardedFor &&
        request.headers['x-forwarded-for']) {
        var immediatePeerIP = this.remoteAddress;
        this.remoteAddresses = request.headers['x-forwarded-for']
            .split(xForwardedForSeparatorRegExp);
        this.remoteAddresses.push(immediatePeerIP);
        this.remoteAddress = this.remoteAddresses[0];
    }

    // Extensions are optional.
    var extensionsString = request.headers['sec-websocket-extensions'];
    this.requestedExtensions = this.parseExtensions(extensionsString);

    // Cookies are optional
    var cookieString = request.headers['cookie'];
    this.cookies = this.parseCookies(cookieString);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.request.prototype.reject"></a>[function <span class="apidocSignatureSpan">websocket.request.prototype.</span>reject (status, reason, extraHeaders)](#apidoc.element.websocket.request.prototype.reject)
- description and source-code
```javascript
reject = function (status, reason, extraHeaders) {
    this._verifyResolution();

    // Mark the request resolved now so that the user can't call accept or
    // reject a second time.
    this._resolved = true;
    this.emit('requestResolved', this);

    if (typeof(status) !== 'number') {
        status = 403;
    }
    var response = 'HTTP/1.1 ' + status + ' ' + httpStatusDescriptions[status] + '\r\n' +
                   'Connection: close\r\n';
    if (reason) {
        reason = reason.replace(headerSanitizeRegExp, '');
        response += 'X-WebSocket-Reject-Reason: ' + reason + '\r\n';
    }

    if (extraHeaders) {
        for (var key in extraHeaders) {
            var sanitizedValue = extraHeaders[key].toString().replace(headerSanitizeRegExp, '');
            var sanitizedKey = key.replace(headerSanitizeRegExp, '');
            response += (sanitizedKey + ': ' + sanitizedValue + '\r\n');
        }
    }

    response += '\r\n';
    this.socket.end(response, 'ascii');

    this.emit('requestRejected', this);
}
```
- example usage
```shell
...
  // put logic here to detect whether the specified origin is allowed.
  return true;
}

wsServer.on('request', function(request) {
if (!originIsAllowed(request.origin)) {
  // Make sure we only accept requests from an allowed origin
  request.reject();
  console.log((new Date()) + ' Connection from origin ' + request.origin + ' rejected.');
  return;
}

var connection = request.accept('echo-protocol', request.origin);
console.log((new Date()) + ' Connection accepted.');
connection.on('message', function(message) {
...
```



# <a name="apidoc.module.websocket.router"></a>[module websocket.router](#apidoc.module.websocket.router)

#### <a name="apidoc.element.websocket.router.router"></a>[function <span class="apidocSignatureSpan">websocket.</span>router (config)](#apidoc.element.websocket.router.router)
- description and source-code
```javascript
function WebSocketRouter(config) {
    // Superclass Constructor
    EventEmitter.call(this);

    this.config = {
        // The WebSocketServer instance to attach to.
        server: null
    };
    if (config) {
        extend(this.config, config);
    }
    this.handlers = [];

    this._requestHandler = this.handleRequest.bind(this);
    if (this.config.server) {
        this.attachServer(this.config.server);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router.super_"></a>[function <span class="apidocSignatureSpan">websocket.router.</span>super_ ()](#apidoc.element.websocket.router.super_)
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



# <a name="apidoc.module.websocket.router.prototype"></a>[module websocket.router.prototype](#apidoc.module.websocket.router.prototype)

#### <a name="apidoc.element.websocket.router.prototype.attachServer"></a>[function <span class="apidocSignatureSpan">websocket.router.prototype.</span>attachServer (server)](#apidoc.element.websocket.router.prototype.attachServer)
- description and source-code
```javascript
attachServer = function (server) {
    if (server) {
        this.server = server;
        this.server.on('request', this._requestHandler);
    }
    else {
        throw new Error('You must specify a WebSocketServer instance to attach to.');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router.prototype.detachServer"></a>[function <span class="apidocSignatureSpan">websocket.router.prototype.</span>detachServer ()](#apidoc.element.websocket.router.prototype.detachServer)
- description and source-code
```javascript
detachServer = function () {
    if (this.server) {
        this.server.removeListener('request', this._requestHandler);
        this.server = null;
    }
    else {
        throw new Error('Cannot detach from server: not attached.');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router.prototype.findHandlerIndex"></a>[function <span class="apidocSignatureSpan">websocket.router.prototype.</span>findHandlerIndex (pathString, protocol)](#apidoc.element.websocket.router.prototype.findHandlerIndex)
- description and source-code
```javascript
findHandlerIndex = function (pathString, protocol) {
    protocol = protocol.toLocaleLowerCase();
    for (var i=0, len=this.handlers.length; i < len; i++) {
        var handler = this.handlers[i];
        if (handler.pathString === pathString && handler.protocol === protocol) {
            return i;
        }
    }
    return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router.prototype.handleRequest"></a>[function <span class="apidocSignatureSpan">websocket.router.prototype.</span>handleRequest (request)](#apidoc.element.websocket.router.prototype.handleRequest)
- description and source-code
```javascript
handleRequest = function (request) {
    var requestedProtocols = request.requestedProtocols;
    if (requestedProtocols.length === 0) {
        requestedProtocols = ['____no_protocol____'];
    }

    // Find a handler with the first requested protocol first
    for (var i=0; i < requestedProtocols.length; i++) {
        var requestedProtocol = requestedProtocols[i].toLocaleLowerCase();

        // find the first handler that can process this request
        for (var j=0, len=this.handlers.length; j < len; j++) {
            var handler = this.handlers[j];
            if (handler.path.test(request.resourceURL.pathname)) {
                if (requestedProtocol === handler.protocol ||
                    handler.protocol === '*')
                {
                    var routerRequest = new WebSocketRouterRequest(request, requestedProtocol);
                    handler.callback(routerRequest);
                    return;
                }
            }
        }
    }

    // If we get here we were unable to find a suitable handler.
    request.reject(404, 'No handler is available for the given request.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router.prototype.mount"></a>[function <span class="apidocSignatureSpan">websocket.router.prototype.</span>mount (path, protocol, callback)](#apidoc.element.websocket.router.prototype.mount)
- description and source-code
```javascript
mount = function (path, protocol, callback) {
    if (!path) {
        throw new Error('You must specify a path for this handler.');
    }
    if (!protocol) {
        protocol = '____no_protocol____';
    }
    if (!callback) {
        throw new Error('You must specify a callback for this handler.');
    }

    path = this.pathToRegExp(path);
    if (!(path instanceof RegExp)) {
        throw new Error('Path must be specified as either a string or a RegExp.');
    }
    var pathString = path.toString();

    // normalize protocol to lower-case
    protocol = protocol.toLocaleLowerCase();

    if (this.findHandlerIndex(pathString, protocol) !== -1) {
        throw new Error('You may only mount one handler per path/protocol combination.');
    }

    this.handlers.push({
        'path': path,
        'pathString': pathString,
        'protocol': protocol,
        'callback': callback
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router.prototype.pathToRegExp"></a>[function <span class="apidocSignatureSpan">websocket.router.prototype.</span>pathToRegExp (path)](#apidoc.element.websocket.router.prototype.pathToRegExp)
- description and source-code
```javascript
pathToRegExp = function (path) {
    if (typeof(path) === 'string') {
        if (path === '*') {
            path = /^.*$/;
        }
        else {
            path = path.replace(/[-[\]{}()*+?.,\\^$|#\s]/g, '\\$&');
            path = new RegExp('^' + path + '$');
        }
    }
    return path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.router.prototype.unmount"></a>[function <span class="apidocSignatureSpan">websocket.router.prototype.</span>unmount (path, protocol)](#apidoc.element.websocket.router.prototype.unmount)
- description and source-code
```javascript
unmount = function (path, protocol) {
    var index = this.findHandlerIndex(this.pathToRegExp(path).toString(), protocol);
    if (index !== -1) {
        this.handlers.splice(index, 1);
    }
    else {
        throw new Error('Unable to find a route matching the specified path and protocol.');
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.server"></a>[module websocket.server](#apidoc.module.websocket.server)

#### <a name="apidoc.element.websocket.server.server"></a>[function <span class="apidocSignatureSpan">websocket.</span>server (config)](#apidoc.element.websocket.server.server)
- description and source-code
```javascript
function WebSocketServer(config) {
    // Superclass Constructor
    EventEmitter.call(this);

    this._handlers = {
        upgrade: this.handleUpgrade.bind(this),
        requestAccepted: this.handleRequestAccepted.bind(this),
        requestResolved: this.handleRequestResolved.bind(this)
    };
    this.connections = [];
    this.pendingRequests = [];
    if (config) {
        this.mount(config);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.super_"></a>[function <span class="apidocSignatureSpan">websocket.server.</span>super_ ()](#apidoc.element.websocket.server.super_)
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



# <a name="apidoc.module.websocket.server.prototype"></a>[module websocket.server.prototype](#apidoc.module.websocket.server.prototype)

#### <a name="apidoc.element.websocket.server.prototype.broadcast"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>broadcast (data)](#apidoc.element.websocket.server.prototype.broadcast)
- description and source-code
```javascript
broadcast = function (data) {
    if (Buffer.isBuffer(data)) {
        this.broadcastBytes(data);
    }
    else if (typeof(data.toString) === 'function') {
        this.broadcastUTF(data);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.broadcastBytes"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>broadcastBytes (binaryData)](#apidoc.element.websocket.server.prototype.broadcastBytes)
- description and source-code
```javascript
broadcastBytes = function (binaryData) {
    this.connections.forEach(function(connection) {
        connection.sendBytes(binaryData);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.broadcastUTF"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>broadcastUTF (utfData)](#apidoc.element.websocket.server.prototype.broadcastUTF)
- description and source-code
```javascript
broadcastUTF = function (utfData) {
    this.connections.forEach(function(connection) {
        connection.sendUTF(utfData);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.closeAllConnections"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>closeAllConnections ()](#apidoc.element.websocket.server.prototype.closeAllConnections)
- description and source-code
```javascript
closeAllConnections = function () {
    this.connections.forEach(function(connection) {
        connection.close();
    });
    this.pendingRequests.forEach(function(request) {
        process.nextTick(function() {
          request.reject(503); // HTTP 503 Service Unavailable
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.handleConnectionClose"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleConnectionClose (connection, closeReason, description)](#apidoc.element.websocket.server.prototype.handleConnectionClose)
- description and source-code
```javascript
handleConnectionClose = function (connection, closeReason, description) {
    var index = this.connections.indexOf(connection);
    if (index !== -1) {
        this.connections.splice(index, 1);
    }
    this.emit('close', connection, closeReason, description);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.handleRequestAccepted"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleRequestAccepted (connection)](#apidoc.element.websocket.server.prototype.handleRequestAccepted)
- description and source-code
```javascript
handleRequestAccepted = function (connection) {
    var self = this;
    connection.once('close', function(closeReason, description) {
        self.handleConnectionClose(connection, closeReason, description);
    });
    this.connections.push(connection);
    this.emit('connect', connection);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.handleRequestResolved"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleRequestResolved (request)](#apidoc.element.websocket.server.prototype.handleRequestResolved)
- description and source-code
```javascript
handleRequestResolved = function (request) {
    var index = this.pendingRequests.indexOf(request);
    if (index !== -1) { this.pendingRequests.splice(index, 1); }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.handleUpgrade"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>handleUpgrade (request, socket)](#apidoc.element.websocket.server.prototype.handleUpgrade)
- description and source-code
```javascript
handleUpgrade = function (request, socket) {
    var wsRequest = new WebSocketRequest(socket, request, this.config);
    try {
        wsRequest.readHandshake();
    }
    catch(e) {
        wsRequest.reject(
            e.httpCode ? e.httpCode : 400,
            e.message,
            e.headers
        );
        debug('Invalid handshake: %s', e.message);
        return;
    }

    this.pendingRequests.push(wsRequest);

    wsRequest.once('requestAccepted', this._handlers.requestAccepted);
    wsRequest.once('requestResolved', this._handlers.requestResolved);

    if (!this.config.autoAcceptConnections && utils.eventEmitterListenerCount(this, 'request') > 0) {
        this.emit('request', wsRequest);
    }
    else if (this.config.autoAcceptConnections) {
        wsRequest.accept(wsRequest.requestedProtocols[0], wsRequest.origin);
    }
    else {
        wsRequest.reject(404, 'No handler is configured to accept the connection.');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.mount"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>mount (config)](#apidoc.element.websocket.server.prototype.mount)
- description and source-code
```javascript
mount = function (config) {
    this.config = {
        // The http server instance to attach to.  Required.
        httpServer: null,

        // 64KiB max frame size.
        maxReceivedFrameSize: 0x10000,

        // 1MiB max message size, only applicable if
        // assembleFragments is true
        maxReceivedMessageSize: 0x100000,

        // Outgoing messages larger than fragmentationThreshold will be
        // split into multiple fragments.
        fragmentOutgoingMessages: true,

        // Outgoing frames are fragmented if they exceed this threshold.
        // Default is 16KiB
        fragmentationThreshold: 0x4000,

        // If true, the server will automatically send a ping to all
        // clients every 'keepaliveInterval' milliseconds.  The timer is
        // reset on any received data from the client.
        keepalive: true,

        // The interval to send keepalive pings to connected clients if the
        // connection is idle.  Any received data will reset the counter.
        keepaliveInterval: 20000,

        // If true, the server will consider any connection that has not
        // received any data within the amount of time specified by
        // 'keepaliveGracePeriod' after a keepalive ping has been sent to
        // be dead, and will drop the connection.
        // Ignored if keepalive is false.
        dropConnectionOnKeepaliveTimeout: true,

        // The amount of time to wait after sending a keepalive ping before
        // closing the connection if the connected peer does not respond.
        // Ignored if keepalive is false.
        keepaliveGracePeriod: 10000,

        // Whether to use native TCP keep-alive instead of WebSockets ping
        // and pong packets.  Native TCP keep-alive sends smaller packets
        // on the wire and so uses bandwidth more efficiently.  This may
        // be more important when talking to mobile devices.
        // If this value is set to true, then these values will be ignored:
        //   keepaliveGracePeriod
        //   dropConnectionOnKeepaliveTimeout
        useNativeKeepalive: false,

        // If true, fragmented messages will be automatically assembled
        // and the full message will be emitted via a 'message' event.
        // If false, each frame will be emitted via a 'frame' event and
        // the application will be responsible for aggregating multiple
        // fragmented frames.  Single-frame messages will emit a 'message'
        // event in addition to the 'frame' event.
        // Most users will want to leave this set to 'true'
        assembleFragments: true,

        // If this is true, websocket connections will be accepted
        // regardless of the path and protocol specified by the client.
        // The protocol accepted will be the first that was requested
        // by the client.  Clients from any origin will be accepted.
        // This should only be used in the simplest of cases.  You should
        // probably leave this set to 'false' and inspect the request
        // object to make sure it's acceptable before accepting it.
        autoAcceptConnections: false,

        // Whether or not the X-Forwarded-For header should be respected.
        // It's important to set this to 'true' when accepting connections
        // from untrusted clients, as a malicious client could spoof its
        // IP address by simply setting this header.  It's meant to be added
        // by a trusted proxy or other intermediary within your own
        // infrastructure.
        // See:  http://en.wikipedia.org/wiki/X-Forwarded-For
        ignoreXForwardedFor: false,

        // The Nagle Algorithm makes more efficient use of network resources
        // by introducing a small delay before sending small packets so that
        // multiple messages can be batched together before going onto the
        // wire.  This however comes at the cost of latency, so the default
        // is to disable it.  If you don't need low latency and are streaming
        // lots of small messages, you can change this to 'false'
        disableNag ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.shutDown"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>shutDown ()](#apidoc.element.websocket.server.prototype.shutDown)
- description and source-code
```javascript
shutDown = function () {
    this.unmount();
    this.closeAllConnections();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.server.prototype.unmount"></a>[function <span class="apidocSignatureSpan">websocket.server.prototype.</span>unmount ()](#apidoc.element.websocket.server.prototype.unmount)
- description and source-code
```javascript
unmount = function () {
    var upgradeHandler = this._handlers.upgrade;
    this.config.httpServer.forEach(function(httpServer) {
        httpServer.removeListener('upgrade', upgradeHandler);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.w3cwebsocket"></a>[module websocket.w3cwebsocket](#apidoc.module.websocket.w3cwebsocket)

#### <a name="apidoc.element.websocket.w3cwebsocket.w3cwebsocket"></a>[function <span class="apidocSignatureSpan">websocket.</span>w3cwebsocket (url, protocols, origin, headers, requestOptions, clientConfig)](#apidoc.element.websocket.w3cwebsocket.w3cwebsocket)
- description and source-code
```javascript
function W3CWebSocket(url, protocols, origin, headers, requestOptions, clientConfig) {
    // Make this an EventTarget.
    yaeti.EventTarget.call(this);

    // Sanitize clientConfig.
    clientConfig = clientConfig || {};
    clientConfig.assembleFragments = true;  // Required in the W3C API.

    var self = this;

    this._url = url;
    this._readyState = CONNECTING;
    this._protocol = undefined;
    this._extensions = '';
    this._bufferedAmount = 0;  // Hack, always 0.
    this._binaryType = 'arraybuffer';  // TODO: Should be 'blob' by default, but Node has no Blob.

    // The WebSocketConnection instance.
    this._connection = undefined;

    // WebSocketClient instance.
    this._client = new WebSocketClient(clientConfig);

    this._client.on('connect', function(connection) {
        onConnect.call(self, connection);
    });

    this._client.on('connectFailed', function() {
        onConnectFailed.call(self);
    });

    this._client.connect(url, protocols, origin, headers, requestOptions);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.websocket.w3cwebsocket.prototype"></a>[module websocket.w3cwebsocket.prototype](#apidoc.module.websocket.w3cwebsocket.prototype)

#### <a name="apidoc.element.websocket.w3cwebsocket.prototype.close"></a>[function <span class="apidocSignatureSpan">websocket.w3cwebsocket.prototype.</span>close (code, reason)](#apidoc.element.websocket.w3cwebsocket.prototype.close)
- description and source-code
```javascript
close = function (code, reason) {
    switch(this._readyState) {
        case CONNECTING:
            // NOTE: We don't have the WebSocketConnection instance yet so no
            // way to close the TCP connection.
            // Artificially invoke the onConnectFailed event.
            onConnectFailed.call(this);
            // And close if it connects after a while.
            this._client.on('connect', function(connection) {
                if (code) {
                    connection.close(code, reason);
                } else {
                    connection.close();
                }
            });
            break;
        case OPEN:
            this._readyState = CLOSING;
            if (code) {
                this._connection.close(code, reason);
            } else {
                this._connection.close();
            }
            break;
        case CLOSING:
        case CLOSED:
            break;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.websocket.w3cwebsocket.prototype.send"></a>[function <span class="apidocSignatureSpan">websocket.w3cwebsocket.prototype.</span>send (data)](#apidoc.element.websocket.w3cwebsocket.prototype.send)
- description and source-code
```javascript
send = function (data) {
    if (this._readyState !== OPEN) {
        throw new Error('cannot call send() while not connected');
    }

    // Text.
    if (typeof data === 'string' || data instanceof String) {
        this._connection.sendUTF(data);
    }
    // Binary.
    else {
        // Node Buffer.
        if (data instanceof Buffer) {
            this._connection.sendBytes(data);
        }
        // If ArrayBuffer or ArrayBufferView convert it to Node Buffer.
        else if (data.byteLength || data.byteLength === 0) {
            data = toBuffer(data);
            this._connection.sendBytes(data);
        }
        else {
            throw new Error('unknown binary data:', data);
        }
    }
}
```
- example usage
```shell
...

client.onopen = function() {
    console.log('WebSocket Client Connected');

    function sendNumber() {
        if (client.readyState === client.OPEN) {
            var number = Math.round(Math.random() * 0xFFFFFF);
            client.send(number.toString());
            setTimeout(sendNumber, 1000);
        }
    }
    sendNumber();
};

client.onclose = function() {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
