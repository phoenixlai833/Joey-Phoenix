---
layout: default
title: Task 4 | Basic Routing Methods
nav_order: 6
---

# Middleware to Display Static Files
Middleware is anything placed between layers of one software to another. Middleware in Express are functions that can access the request object(req) and response object(res) for each route so are about to execute any code and make changes to those objects. They also have access to the next function in the applications request-response cycle, therefore, middleware can end the cycle or call the next middleware function in the queue. There are various types that have different uses but this document focuses on middleware to display static files such as CSS and images. The function signature is as follows:
> `express.static(root, [options])`
