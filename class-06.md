#  NODE.JS 
Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine. 

Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi. It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.


Then  ***Node.js*** : is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.

 
**Node comes bundled with a package manager called npm**
To check which version you have installed on your system, type `npm -v`.
npm is also the world’s largest software registry



### The `package.json` File

If you look at the contents of the `test` directory, you’ll notice a folder entitled `node_modules`. 
This is where npm has saved lodash and any libraries that lodash depends on.
 The `node_modules` folder shouldn’t be checked in to version control, and can, in fact, be re-created at any time by running `npm install` from within the project’s root.


## What Is Node.js Used For? 

These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.


##The Node.js Execution Model:

In very simplistic terms, when you connect to a traditional server, such as Apache, it will spawn a new thread to handle the request. In a language such as PHP or Ruby, any subsequent I/O operations (for example, interacting with a database) block the execution of your code until the operation has completed. That is, the server has to wait for the database lookup to complete before it can move on to processing the result. If new requests come in while this is happening, the server will spawn new threads to deal with them. This is potentially inefficient, as a large number of threads can cause a system to become sluggish — and, in the worst case, for the site to go down. The most common way to support more connections is to add more servers


![ image depicts Node’s execution model](https://uploads.sitepoint.com/wp-content/uploads/2012/10/1516152673node_event_loop.png)


## What Kind of Apps Is Node.js Suited To?

Node is particularly suited to building applications that require some form of real-time interaction or collaboration — for example, chat sites, or apps such as CodeShare, where you can watch a document being edited live by someone else. It’s also a good fit for building APIs where you’re handling lots of requests that are I/O driven (such as those needing to perform operations on a database), or for sites involving data streaming, as Node makes it possible to process files while they’re still being uploaded. If this real-time aspect of Node is something you’d like to look into more, check out our tutorial on Building a Real-time Chat App

## What Are the Advantages of Node.js? 

![ the Advantages of Node.js](https://www.simform.com/wp-content/uploads/2020/06/Node.js-Advantages-1.jpg)


