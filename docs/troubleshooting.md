---
layout: default
title: Troubleshooting
nav_order: 8
---

# Troubleshooting

<div class="code-example" markdown="1">

| Symptoms       | Probable Cause          | Action |
|:-------------|:------------------|:------|
| Unable to load the page in local host           | The URL does not match the port number | Double check what port you set in *server.js* and if your browser URL is localhost:PORT, PORT being the number you set  |
|  | Missing the express app listen code.   | Make sure this code is in app.js: `app.listen(port, () => {})`  |
|        | There is another app running on the same port number      | Make sure the port in `app.listen(port, () => {})` is at an available port, anything above 1024 to 65535, some sample port numbers to try are 8000, 3000, 8080.   |
|         | file changes were not saved | Save and retry  |
|         | Nodemon crashed | Type `rs` in the terminal to restart nodemon |
|`npm init` does not create the package.json file | The terminal path is pointing to the wrong directory | Use the `cd` <folder> command in terminal to locate to the correct directory |

</div>




