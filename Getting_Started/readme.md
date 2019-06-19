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
- Enter app.js, or whatever you want the name of the main file to be. If you want it to be index.js, hit RETURN to accept the suggested default file name.
- Now install Express in the myapp directory and save it in the dependencies list. For example:<br>
    <pre>
    $ npm install express --save</pre>

### Hello World

- In the myapp directory, create a file named app.js.
- Go to file in app.js in myapp directory.
- Run the app with the following command:<br>
    <pre>
    $ node app.js</pre>
- Then, load http://localhost:3000/ in a browser to see the output.

### Express generator

- Use the application generator tool, express-generator, to quickly create an application skeleton.
- The express-generator package installs the express command-line tool. Use the following command to do so:<br>
    <pre>
    $ npm install express-generator -g</pre>
- Display the command options with the -h option:<br>
    <pre>
    $ express -h</pre>
- To create Express app using genrator give the following comand:<br>
    <pre>
    $ express --view=pug myappgen</pre>
- Then install dependencies and run the app:<br>
    <pre>
    change directory:
     $ cd myappgen

   install dependencies:
     $ npm install

   run the app:
     $ DEBUG=myappgen:* npm start</pre>