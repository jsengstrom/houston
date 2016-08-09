# Houston - Yet Another Web Boilerplate
*Version 0.1.0 - **Beta***

Houston is a simple web boilerplate built to help get projects off the ground quickly. It tries to make as few assumptions as possible, while still providing enough of a head-start to make it worthwhile.

Houston is made mostly as a CSS boilerplate, however there are (a few) scripts wrapped up in it too. It's been built to run with grunt, although you could use [Codekit 2](https://incident57.com/codekit/index.html) if you really wanted.

A few things you'll need:
- [Node.js](https://nodejs.org)
- [Sass](http://sass-lang.com)
- [Grunt.js](http://gruntjs.com)

## Getting Started

1. Clone this repo, and name it ```$ git clone {{url}} my-folder-name```
-  Change directory into the project folder ```$ cd my-folder-name```
-  Install Node Package Manager (and all the packages) ```$ npm install```
-  Start grunt with a static server (http://localhost:8888) ```$ grunt serve &``` or just watch the sass/js files without a server ```$ grunt watch &```

That's all.

## Usage

### Sass/SCSS

Everything is set up to concatenate and compile partial files as you add them to the ```components``` and ```layouts``` folders. The boilerplate code is contained within ```_houston``` as is the config file (```_config.scss```). This will guide you though setting up all the base styles for your project.

All files within the ```scss``` folder are watched, providing grunt watch has been initiated using either of the commands in Step 4 above.

Include ```<link src='/build/css/global.css' />``` in your head.

### JS Usage

The ```global.js``` file has any partials imported to it that are required by Houston (currently only for the cookies message). It is then minified to the build folder.

All files within the ```js``` folder are watched, providing grunt watch has been initiated using either of the commands in Step 4 above.

Include ```<script src='/build/css/global.min.js'></script>``` before your closing ```<body>``` tag.

### Images

Save images into the ```img``` folder, and run ```$ grunt minify``` to compress an optimise them for the web. Link to files will be placed within ```build/img/```.

## Features

**Coming soon:** A full (and detailed) list of everything Houston can do. Once I get round to it.

## Help & Support

If you have any issues or questions about Houston, tweet me for support [@jsengstrom](https://twitter.com/jsengstrom).
