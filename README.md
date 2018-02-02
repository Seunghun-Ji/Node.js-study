This project is a making web page using node.js

## Table of Contents
- [Before You Start](#Before-You-Start)
- [Let's Start Your Own Project](# Let's Start Your Own Project)
- [Folder Structure](# Folder Structure)
- [How to use a sample](# How to use a sample)

## Before You Start

you must install 'nvm' program to use node.js

* link '(for windows)': https://github.com/coreybutler/nvm-windows/releases

if you are a Window user, you have to input a command to use nvm.

* nvm use [your-node.js-version]

Then you can check whatever nvm is working or not.

* npm --version

After that, install webpack & yarn.

* npm install -g webpack
* npm install -g yarn

## Let's Start Your Own Project

Now you can make your own project with using node.js

Move to working directory and input a below command.

* yarn add --dev webpack

## Folder Structure

After creation, your project should look like this:

```
.vscode/
    launch
    settings
node_modules/
    ...(236 lists)
package
yarn.lock
```

You can make your own files on root folder.

## How to use a sample

Let's see sample codes.

* `hello.js`
```
module.exports = "Hello";
```

* `world.js`
```
module.exports = "World";
```

* `entry.js`
```
var hello = require("./hello");
var world = require("./world");

document.write(hello + " " + world);
```

Then, input a command to make a file, `bundle.js`

### command: `webpack entry.js bundle.js`

After that, make a `index.html` file to load `bundle.js`.

* `index.html`
```
<html>
    <head>
        <meta charset = 'utf-8'>
    </head>
    <body>
        <script type="text/javascript" src="bundle.js"></script>
    </body>
</html>
```

You can see the result by opening the `index.html` file.
