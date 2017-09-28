JavaScript Starter
==================

Welcome to the wonderful world of **JavaScript**!

As with most programming languages, JavaScript projects require a little bit of *boilerplate* to get started. That is, a JavaScript project requires a few predefined files to initialize the system that runs your program.

This repository of files is exactly that: _The starter files needed to begin a JavaScript project._

(The words you're reading right now are in a file called **README.md**. The "md" file extension stands for "Markdown", but that is not an important detail. This file itself is not really vital boilerplate for JavaScript projects. It's just included as an explanation of the vital files.)

---

## Boilerplate

The vital files are:

### package.json

**package.json** contains information about your program:

- Your program's name
- A brief description of your program
- Your name (so you can get credit for your work!)
- Other details that help the system run your program

### package-lock.json

Whereas the file above (**package.json**) is meant for _you_ to record your project's details, this file (**package-lock.json**) is meant for the _system_ to record details, based on what you define in **package.json**.

So you should never modify or remove **package-lock.json**. It's meant only for the system to read and modify. In fact, it's fine if you get in the habit of ignoring **package-lock.json** completely.

### main.js

**main.js** is your program! It's the file into which you will write your code.

If you look at **main.js** now, you will see a line of code at the top of the file:

```js
var ask = require('readline-sync');
```

Strictly speaking, this line of code is not vital. We have included it to make your start with coding in JavaScript easier. This line lets you write code like this:

```js
var favorite_color = ask.question("What is your favorite color?")
```

That line of code will ask your user what their favorite color is. And it will store their reply inside of a "variable" named `favorite_color`.

(Asking users for their input is a pretty common, fundamental requirement when building programs. That's the only reason why we've included this line of code to start off. If you were building something that didn't need to ask users for their input, then this line would not be necessary.)

### .gitignore

The **.gitignore** file is a bit hard to explain. It's not important for a brand new developer to understand this file's purpose, so we're choosing to skip its explanation. If you're curious, you can always ask someone to explain. But it's safe to ignore this file for now.

---

## Instructions

Now that you know what the files are for, how do you use these starter files to make a JavaScript program?

### 1. Setup

First, if you haven't already, you need to copy these files into a folder in your workspace.

Once you are able to access the files, open up **package.json** and add real information for your project's name, description, and your name. Don't forget to save! :)

### 2. Install System Tools

Next, run the following command in the _terminal_:

```
npm install
```

This will install any system tools that are needed to run your JavaScript program. You do not need to run this command again later, unless you change the **package.json** file.

#### Notes

There are two things that will happen when you run `npm install`, which you should _ignore_:

##### 1. Warnings

You might see some warnings like this:

```
npm WARN my-project@1.0.0 No repository field.
npm WARN my-project@1.0.0 No license field.
```

These warnings are 100% okay, and it is safe to ignore them.

##### 2. node_modules/

You might see a new folder called **node_modules/** appear in your files. This is the folder where the system tools you just installed are stored. It is best to ignore this folder completely.

### 3. Start Program

To start your program, run the following command in the _terminal_:

```
npm start
```

This will run the **main.js** program. Since there's almost nothing in that file yet, this command doesn't do much of interest. But it should output some system messages like this:

```bash
> my-project@1.0.0 start /username/project
> node main.js
```

Your actual might be a little bit different, but essentially this is the system telling you that it received your instructions to start the program and is running the **main.js** file.

### 4. Have fun!

Now you can begin coding a program! Add your code to **main.js** and–after saving the file–run `npm start` to see what your program does. Repeat this process until you're satisfied or have a question to ask.