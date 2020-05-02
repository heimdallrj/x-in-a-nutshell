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

NPM Stands fot **Node Package Manager**.

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
}).listen(8080);

// Console will print the message
console.log('Server running at http://127.0.0.1:8080/');
```

**Output:**

![Image credit: tutorialspoint.com](https://www.tutorialspoint.com/nodejs/images/nodejs_sample.jpg)

## Basic Concepts

* Lexical Structure
* Expressions
* Types
* Variables
* Functions
* this
* Arrow Functions
* Loops
* Scopes
* Arrays
* Template Literals
* Semicolons
* Strict Mode
* ECMAScript 6, 2016, 2017

* REPL
* Asynchronous programming and callbacks
* Timers
* Promises
* Async and Await
* Closures
* The Event Loop

### REPL

READ - EVAL - PRINT - LOOP.

### Event Loop

The event loop is what allows Node.js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded.

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

## Core Modules

### Event Emitter

### Buffers

### Streams

### File System

### Global Objects

### Utility Modules

### Web Module

## Frameworks

### Express

## RESTful API

## Scaling Application

## Publish Your First NPM Package

## Credits

* [TutorialsPoint](https://www.tutorialspoint.com/nodejs/)
