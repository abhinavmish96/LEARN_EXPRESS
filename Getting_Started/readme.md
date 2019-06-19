# Module 1 : Getting Stated

## This Chapter focuses on the Express basics, installation and set-up.

### Topics covered in this module include:

- **Installing**
- **Hello World**
- **Express generator**
- **Basic routing**
- **Static files**

### Installing

- Assuming [Node.js](https://nodejs.org) is already installed , create a directory to hold your application, and make that your working directory.<br>
    <pre>
    $ mkdir myapp
    $ cd myapp</pre>
- Use the **npm init** command to create a package.json file for your application. For more information on how package.json works, see [Specifics of npm’s package.json handling](https://docs.npmjs.com/files/package.json).<br>
    <pre>
    $ npm init</pre>
- This command prompts you for a number of things, such as the name and version of your application. For now, you can simply hit RETURN to accept the defaults for most of them, with the following exception:<br>
    <pre>
    entry point: (index.js)</pre>
- This command prompts you for a number of things, such as the name and version of your application. For now, you can simply hit RETURN to accept the defaults for most of them, with the following exception:<br>
    <pre>
    entry point: (index.js)</pre>
Enter app.js, or whatever you want the name of the main file to be. If you want it to be index.js, hit RETURN to accept the suggested default file name.
- Now install Express in the myapp directory and save it in the dependencies list. For example:<br>
    <pre>
    $ npm install express --save</pre>