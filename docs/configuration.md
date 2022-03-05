---
layout: default
title: Task 1 | Installing Express.js & EJS
nav_order: 2
---
# Installing Express.js & EJS
### Overview
Your first task is to install the *Express.js* and *EJS* libraries for your project.


In order to install *Express.js* and *EJS*, we first need to create a **Workspace** on VSCode.


After setting up your Workspace, we need to initialize our project directory which will create a new file called *package.json*. We will be checking the *package.json* file later to make sure that we have successfully installed the *Express.js* and *EJS* libraries.


💭 NOTE: If you already have a designated folder for this project set up on VSCode, you may skip to step 4.

---

### Install Express from the VS Code Terminal

**1.** Open the Visual Studio Code software.

**2.** Create a designated folder to store your project files.

**3.** Open the project folder in Mac or Windows.

>**(macOS)** Drag your folder into the Workspace column on the left of the VS Code interface
You will be greeted with a pop up. Select "Yes, I trust the authors".

![Workspace popup message](../assets/images/step-3.png)

>**(Windows)** Go under the 'File' tab on the navigation bar and select "Open folder". Select your designated folder.
You will be greeted with a pop up. Select "Yes, I trust the authors".

![Workspace popup message](../assets/images/step-3.png)

**4.** Hit **[CTRL]** and **[~]** simultaneously on your keyboard to open the terminal.
The terminal should open up at the bottom of the application.

![Screenshot of terminal](../assets/images/task-1-terminal.png)


💭 **NOTE** : Make sure that the directory in the terminal matches the directory of your project folder.

**5.** Type `npm init` in the terminal and hit **[Enter]** to run the command


Some prompts will appear in the terminal. Hit **[Enter]** for each prompt to use the default settings. Once you see the prompt *`Is this OK? (yes)`*, hit **[Enter]** once more. You should see a new file listed in your project directory in the Workspace column called *package.json*.


❗ **CAUTION** : Do not delete or alter the package.json file at this point!
![Screenshot of workspace after initialization](../assets/images/task-1-init.png)


**6.** Type `npm install express` in the terminal and hit **[Enter]** to run the command


You can watch the installation process in the terminal. The installation has succeeded when you see the prompt *`found 0 vulnerabilities`*. You may see some WARNING prompts but don't worry about these.


![Screenshot of workspace after install express](../assets/images/task-1-install-express.png)

**7.** Type `npm install ejs express` in the terminal and hit **[Enter]** to run the command


You can watch the installation process in the terminal. The installation has succeeded when you see the prompt *`found 0 vulnerabilities`*. You may see some WARNING prompts but don't worry about these.


![Screenshot of ejs command](../assets/images/task-1-install-ejs.png)

**8.** Confirm that the installations have succeeded by checking the *package.json* file


`express.js` and `ejs` should now be listed under `dependencies`.


![Screenshot of package.json file](../assets/images/task-1-package-json.png)

---

### Conclusion
You have successfully installed *EJS* and *Express.js*! That means the libraries are ready to be used in your project and you are ready to move on to the next step.

#### Congratulations! Continue to the next step and learn how to [Build the File Structure](step-2.md). 🚀 
