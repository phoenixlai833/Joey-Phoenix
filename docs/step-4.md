---
layout: default
title: Task 4 | Basic Routing Methods
nav_order: 5
---

# Basic Routing Methods
*Routing* is an essential part of back-end development and it determines how the application responds to client requests to a *URI(path)* and a specific *HTTP request method*. Express simplifies this process by easily controlling what *callback function* gets invoked when a user navigates to a particular URL. The application then listens for requests that match a specific route and executes the associated code.

Routes in Express are defined using *methods* of the Express app object which correspond to HTTP methods such as GET and POST requests. The *function signature* is as follows:

>`app.METHOD(PATH, HANDLER)`
> - `app`: is an instance of Express
> - `METHOD`: is the Express route method(eg.`get`, `post`)
> - `PATH`: is a path on the server
> - `HANDLER`: is the callback function that executes when the METHOD and PATH matches the client HTTP request


