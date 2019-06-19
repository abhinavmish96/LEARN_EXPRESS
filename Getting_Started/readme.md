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

### Basic routing

- **Routing** refers to determining how an application responds to a client request to a particular endpoint, which is a URI (or path) and a specific HTTP request method (GET, POST, and so on).
- Each route can have one or more handler functions, which are executed when the route is matched. Route definition takes the following structure:<br>
    <pre>
    app.METHOD(PATH, HANDLER)</pre>
- Where:
    - app is an instance of express.
    - METHOD is an [HTTP request method](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol#Request_methods), in lowercase.
    - PATH is a path on the server.
    - HANDLER is the function executed when the route is matched.

### Static Files

- To serve static files such as images, CSS files, and JavaScript files, use the express.static built-in middleware function in Express.
- The function signature is:<br>
    <pre>
    express.static(root, [options])</pre>
- The root argument specifies the root directory from which to serve static assets.
- For example, use the following code to serve images, CSS files, and JavaScript files in a directory named public:<br>
    <pre>
    app.use(express.static('public'))</pre>
- To use multiple static assets directories, call the express.static middleware function multiple times.<br>
    <pre>
    app.use(express.static('public'))
    app.use(express.static('files'))</pre>
- Express looks up the files in the order in which you set the static directories with the express.static middleware function.
- However, the path that you provide to the express.static function is relative to the directory from where you launch your node process. If you run the express app from another directory, it’s safer to use the absolute path of the directory that you want to serve:<br>
    <pre>
    app.use('/static', express.static(path.join(__dirname, 'public')))</pre>