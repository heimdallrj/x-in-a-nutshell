# Node.js in a nutshell.

## Introduction

* [Node.js](https://nodejs.org/en/) is a server-side JavaScript runtime + JavaScript Library
* Built on [Chrome's V8 JavaScript engine](https://code.google.com/p/v8/).
* Developed by [Ryan Dahl](https://en.wikipedia.org/wiki/Ryan_Dahl) in 2009
* MIT Licenced 

#### Features

* Faster code execution
* Asynchronous and Event Driven
* Single Threaded but Highly Scalable
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

### Internals

![Image credit: tutorialspoint.com](https://www.tutorialspoint.com/nodejs/images/nodejs_concepts.jpg)

### REPL

READ - EVAL - PRINT - LOOP.

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
fs.readdir(source, function (err, files) {
  if (err) {
    console.log('Error finding files: ' + err)
  } else {
    files.forEach(function (filename, fileIndex) {
      console.log(filename)
      gm(source + filename).size(function (err, values) {
        if (err) {
          console.log('Error identifying file size: ' + err)
        } else {
          console.log(filename + ' : ' + values)
          aspect = (values.width / values.height)
          widths.forEach(function (width, widthIndex) {
            height = Math.round(width / aspect)
            console.log('resizing ' + filename + 'to ' + height + 'x' + height)
            this.resize(width, height).write(dest + 'w' + width + '_' + filename, function(err) {
              if (err) console.log('Error writing file: ' + err)
            })
          }.bind(this))
        }
      })
    })
  }
})
```
Source: [callbackhell.com](http://callbackhell.com/)

### Event Loop

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
