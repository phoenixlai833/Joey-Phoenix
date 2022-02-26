---
layout: default
title: Task 4 | Basic Routing Methods
nav_order: 5
---

# Basic Routing Methods
### Overview
*Routing* is an essential part of back-end development and it determines how the application responds to client requests to a *URI(path)* and a specific *HTTP request method*. Express simplifies this process by easily controlling what *callback function* gets invoked when a user navigates to a particular URL. The application then listens for requests that match a specific route and executes the associated code.

Routes in Express are defined using *methods* of the Express app object which correspond to HTTP methods such as GET and POST requests. The *function signature* is as follows:

>`app.METHOD(PATH, HANDLER)`
> - `app`: is an instance of Express
> - `METHOD`: is the Express route method(eg. `get`, `post`)
> - `PATH`: is a path on the server
> - `HANDLER`: is the callback function that executes when the METHOD and PATH matches the client HTTP request

---

### Routing GET Requests

**1.**  In app.js, in the home route(“/”), change `res.send('Hello World!')` to `res.render(‘index’)`. The edited code should look like this:

![render index.ejs](../assets/images/render_index.png)

**2.**  In order to use ejs files, install the **Embedded Javascript Templates(ejs)** module with the command:

`npm install ejs`

**3.**  Save the files and refresh the browser. The index.ejs file contents should show up and look like this. Yay!
![index working](../assets/images/index1.png)

💭 NOTE: Please remember to save in VScode before refreshing the browser. If the page is still not loading, see the [troubleshooting](troubleshooting.md) for possible solutions.

**4.**  Make a new file in views called user.ejs. Add the boilerplate HTML code and a heading 1 with “this is the user page” ad the text. Alternatively, copy and paste this code:
 











