# blaupause

> Build process & application architecture for web projects

## Installation

 1. `git clone https://github.com/felics/blaupause myApp`
 2. `cd myApp`
 3. `npm install`
 4. `gulp`

## What's in the box...

 - [BrowserSync](http://www.browsersync.io/)
 - [SASS](http://sass-lang.com/) with [Autoprefixer](https://github.com/postcss/autoprefixer) & Minification
 - [Webpack](http://webpack.github.io) - ES6/ AMD / JSX-support & easy bundling
 - [EditorConfig](http://editorconfig.org/)
 - [HTML5 Boilerplate](https://html5boilerplate.com/) + [Modernizr](http://modernizr.com/)
 - (Optional) [Express](http://expressjs.com/)-server with automatic restarts
 - Sourcemaps for JS & CSS files

## Available Tasks:

 - `gulp` - Builds the project files, starts BrowserSync and server(if wanted) and watches for changes to project files.
 - `gulp build` - Only rebuilds project
 - `gulp clean` - Cleans destination folder. Can clean views only if "views.root" is false
 - `gulp styles` - Builds styles
 - `gulp scripts` - Builds scripts
 - `gulp images` - Optimize images
 - `gulp modernizr` - Build a custom Modernizr (Add tests in './gulp/config.js')
 - `gulp views` - Copies static files in "\_src" to dest. For more elaborate view-tasks (templating / nested folder / SSG), modify the task

### Adding tasks:

You can add tasks by creating a .js-file in `./gulp/tasks` that contain a task and a reference to `gulp` anf the `gulp`-modules you want to use.
