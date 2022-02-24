---
layout: default
title: Task 3 | Requiring Express.js
nav_order: 4
---

## Requiring Express.js
*Express.js* is a library that we have installed in Task 1. In order to utilize it in our code, we need to require it.
Task 3 is a walkthrough on how to require express.js. 

We will also be installing a library called *nodemon* which will
automatically restart the localhost server everytime you save a file. This eliminates the need to manually restart the
server to see changes.

### Step 1: Open the *index.js* file and copy and paste the following code into the editor
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

### Step 2: Run the command `npm i -D nodemon` in the terminal to install the nodemon library
Just like in Task 1 when you installed express.js and EJS, wait until the installation has completed. 
If the installation was successful, the prompt `*found 0 vulnerabilities*` will be printed on the terminal.

💭 NOTE: You can confirm the installation of nodemon in the package.json file. `nodemon` should be listed under
a heading called `devDependencies`.

### Step 3: Open the *package.json* file. Under `scripts`, change the `dev` value to "nodemon server.js" 
❗ WARNING: Do not change anything else in the package.json file.
💭 NOTE: Remember to save the file after making changes.

### Step 4: Run the command `npm run dev` in the terminal to start the server
💭 NOTE: Once you have run the command `npm run dev`, the server will automatically refresh with each save, which means
that you do not need to run the command while the server is active. To end the server session, press **[CTRL]** and **[C]** simultaneously
while in the terminal.

### Step 5: Reload the localhost:3000 page on your browser to check your changes
You should be able to see the new HTML text you entered in the index.ejs file from Task 2.

#### You have completed Task 3! 🥳

