---
layout: default
title: Task 3 | Requiring Express.js
nav_order: 4
---

# Requiring Express.js
### Overview
In [Task 1](configuration.md), we installed the *Express.js* library. In order to actually use *Express.js* in our code, we need to require it.
In this task, we will be adding code to our *index.js* file to require the *Express.js* library. 

We will also be installing a library called *nodemon* which will
automatically restart the localhost server every time you save a file. This eliminates the need to manually restart the
server to see changes.

By the end of this task, you will be able to see "Hello World!" printed in your browser on localhost.

---

### Requiring Express.js, installing nodemon, and sending "Hello World"

**1.** Open the *index.js* file and copy and paste the following code into the editor.
```
const express = require('express')
const app = express()
const port = 3000

app.set('view engine', 'ejs')


app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Now listening on port ${port}`)
})
```


Notice in the codeblock above, we have this line:

```
app.get('/', (req, res) => {
  res.send('Hello World!')
})
```
The line that reads `res.send('Hello World!')` tells *Express.js* to send out text that reads "Hello World!" to the browser when the page loads. We will check to see if "Hello World!" successfully prints in the browser in a few steps.

**2.** Run the command `npm i -D nodemon` in the terminal to install the nodemon library.

Just like in Task 1 when you installed *Express.js* and *EJS*, wait until the installation has completed. 
If the installation was successful, the prompt *`found 0 vulnerabilities`* will be printed on the terminal.


![Screenshot of nodemon installation in the terminal](../assets/images/task-3-nodemon-install.png)


💭 NOTE: You can confirm the installation of *nodemon* in the *package.json* file. `nodemon` should be listed under
a heading called `devDependencies`.

**3.** Open the *package.json* file. Under `scripts`, add a comma after `"test": "echo \"Error: no test specified\" && exit 1"` then add `"dev": "nodemon server.js"` under it


❗ WARNING: Do not change anything else in the *package.json* file.


![Screenshot of package.json with nodemon listed](../assets/images/task-3-nodemon-package-json.png)


💭 NOTE: Remember to save the file after making changes.

**4.** Run the command `npm run dev` in the terminal to start the server


Once you have run the command `npm run dev`, the server will automatically refresh with each save, which means
that you do not need to run the command while the server is active. 


💭 NOTE: To end the server session, press **[CTRL]** and **[C]** simultaneously
while in the terminal. Closing VSCode will also automatically end your server session.



![Screenshot of nodemon working in terminal](../assets/images/task-3-nodemon.png)


Test that *nodemon* works by saving the file. You should see messages in the terminal of the server restarting.

**5.** Open up your browser and enter `localhost:3000` in the URL and hit **[Enter]**


You should be able to see "Hello World!".

![Screenshot of Hello World in browser](../assets/images/task-3-hello-world.png)

---

### Conclusion
That is the end of task three! You have successfully required *Express.js* in your project, installed the nodemon library, and used *Express.js* to send text onto your localhost browser page.


Remember the block of code that told *Express.js* to send 'Hello World!'? Try replacing "Hello World!" with your own message!

💭 NOTE: Make sure to enclose your message in quotation marks! Either single or double quotation marks will work.


For example:
```
app.get('/', (req, res) => {
  res.send('Your new message here')
})
```


#### 🥳 Amazing! Now you can move on to [Basic Routing Methods](step-4.md). 

