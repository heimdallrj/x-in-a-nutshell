# Node.js in a nutshell.

## Introduction

* [Node.js](https://nodejs.org/en/) is a server-side JavaScript runtime + JavaScript Library
* Built on [Chrome's V8 JavaScript engine](https://code.google.com/p/v8/).
* Developed by [Ryan Dahl](https://en.wikipedia.org/wiki/Ryan_Dahl) in 2009
* MIT Licenced 

#### Features

* Faster code execution
* Asynchronous and Event Driven
* Single Threaded but highly scalable
* No Buffering

#### Where to Use

* I/O bound Applications
* Data Streaming Applications
* Data Intensive Real-time Applications (DIRT)
* JSON APIs based Applications
* Single Page Applications

#### Where Not to Use

* CPU intensive applications

## Node.js Echosystem

### NPM

[NPM](https://nodejs.dev/an-introduction-to-the-npm-package-manager) Stands fot **Node Package Manager**.

* [NPM Registry](https://www.npmjs.com/) - Online Repository for NPM Packages/modules
* NPM Command-line Utility

## Hello World!

```js
console.log('Hello World!');
```

**hello-world.js**
```js
var http = require('http');

http.createServer(function (request, response) {
   // Send the HTTP header 
   // HTTP Status: 200 : OK
   // Content Type: text/plain
   response.writeHead(200, {'Content-Type': 'text/plain'});
   
   // Send the response body as "Hello World"
   response.end('Hello World\n');
}).listen(8081);

// Console will print the message
console.log('Server running at http://127.0.0.1:8081/');
```

**Output:**

![Image credit: tutorialspoint.com](https://www.tutorialspoint.com/nodejs/images/nodejs_sample.jpg)

## Basic Concepts

- [Lexical Structure](https://javabeginnerstutorial.com/javascript-2/javascripts-lexical-structure/)
- [Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
- Types
- Variables
- Functions
- this
- Arrow Functions
- Loops
- [Scopes](https://scotch.io/tutorials/understanding-scope-in-javascript)
- Arrays
- [Template Literals](https://flaviocopes.com/javascript-template-literals/)
- Semicolons
- [Strict Mode](https://love2dev.com/blog/javascript-strict-mode/)
- [ECMAScript 6, 2016, 2017](https://codeburst.io/javascript-wtf-is-es6-es8-es-2017-ecmascript-dca859e4821c)

* REPL: READ - EVAL - PRINT - LOOP.
* [Asynchronous programming and callbacks](https://nodejs.dev/javascript-asynchronous-programming-and-callbacks)
* Timers
* [Promises](https://nodejs.dev/understanding-javascript-promises)
* [Async and Await](https://nodejs.dev/modern-asynchronous-javascript-with-async-and-await)
* Closures
* [The Event Loop](https://nodejs.dev/the-nodejs-event-loop)

### Callbacks

* Callback is an asynchronous equivalent for a function.
* A callback function is called at the completion of a given task.
* This makes Node.js highly scalable by allowing run processes in non-blocking way.

**Example Code**
```js
var fs = require("fs");

console.log("Begin");

fs.readFile('input.txt', function (err, data) {
   if (err) return console.error(err);
   console.log("Task Completed");
});

console.log("EOF.");
```

Output:
```text
Begin
EOF.
Task Completed
```

#### Callback Hell

Callback hell is where there are many numbers of nested callbacks.

```js
users.get(5, function(err, data){
	messges.get(data.userId, function(err, data){
		replies.get(data.messageId, function(err, data) {
        	...
        });
    });
})
```
Source: [quora.com](https://www.quora.com/What-is-callback-hell)

##### Avoiding Callback hell

> Sometimes it might not be possible to avoid callback hell in every case. So one thing you can do in such cases is; adding meaningful and organize comments in the code.

1. Split the callbacks into different functions
2. Use promises
3. Use asynchronous functions (Async/Await)

### Event Loop

[The event loop](https://nodejs.dev/the-nodejs-event-loop) is what allows Node.js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded.

## Core Modules

* [console](https://nodejs.dev/output-to-the-command-line-using-nodejs)
* [Event Emitter](https://nodejs.dev/the-nodejs-events-module)
* [http](https://nodejs.dev/the-nodejs-http-module)
* [Buffers](https://nodejs.dev/nodejs-buffers)
* [Streams](https://nodejs.dev/nodejs-streams)
* [fs - File System](https://nodejs.dev/the-nodejs-path-module)
* [os](https://nodejs.dev/the-nodejs-os-module)
* [path](https://nodejs.dev/the-nodejs-path-module)

## Debugging

## Deployment

## Appendix-

* [Publish your own NPM package](https://hackernoon.com/publish-your-own-npm-package-946b19df577e)
* [Build a JavaScript Command Line Interface (CLI) with Node.js](https://www.sitepoint.com/javascript-command-line-interface-cli-node-js/)

## Credits

* [TutorialsPoint](https://www.tutorialspoint.com/nodejs/)
* [Node.js Dev](https://nodejs.dev/)
* [Node.js API Reference](https://nodejs.org/api/)
* [katacoda - Node.js Playground](https://www.katacoda.com/courses/nodejs/playground)
