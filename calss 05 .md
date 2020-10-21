# Heroku

### Defining an application
Heroku lets you deploy, run and manage applications written in Ruby, Node.js, Java, Python, Clojure, Scala, Go and PHP.

An application is a collection of source code written in one of these languages, perhaps a framework, and some dependency description that instructs a build system as to which additional dependencies are needed in order to build and run the application.


Git is a powerful, distributed version control system that many developers use to manage and version source code. The Heroku platform uses Git as the primary means for deploying applications (there are other ways to transport your source code to Heroku, including via an API).

When you create an application on Heroku, it associates a new Git remote, typically named heroku, with the local Git repository for your application.

### Dyno manager
Part of the Heroku platform, the dyno manager, is responsible for keeping dynos running. For example, dynos are cycled at least once per day, or whenever the dyno manager detects a fault in the running application (such as out of memory exceptions) or problems with the underlying hardware that requires the dyno be moved to a new physical location.


### Deploy the app
To deploy/create the app fun this command:


`heroku create`


This will generate a random name for your app, then to deploy, enter:


`git push heroku main`


To ensure at least one instance of the app is running, enter:


`heroku ps:scale web=1`


Now yo can visit the app by running:


`heroku open`



# Node .js
We will use Node.js for our project. Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. It's written in JavaScript and can be run within the Node.js runtime on any platform.

So, Node allows you to use the so-called event loop, which works faster because of non-blocking behavior. For example, nginx uses an event loop with asynchronous I/O. That's why it's fast as hell!



