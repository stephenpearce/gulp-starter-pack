# Gulp Starter Pack

An optionated gulp environment for serving simple static projects.

## Prerequisites

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

Consider getting these using nvm-windows on Windows, homebrew on macOS and linuxbrew on Linux.


## Setup Instructions

1. Clone this repository:

   ```bash
   git clone https://github.com/stephenpearce/gulp-starter-pack.git
   cd gulp-starter-pack
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

## Available Commands / Tasks

   Run the following command to start a development server with live reloading:

   ```bash
   gulp
   ```

   This default task cleans the `dist/` folder, builds the project, starts a local server, and watches for changes in source files.

   To build the project without starting a development server, run:

   ```bash
   gulp build
   ```

   This task cleans the `dist/` folder and builds the project for production deployment.
 
   ```bash
   gulp clean
   ```
   
   This cleans the `dist/` directory to prepare for a fresh build.

   ```bash
   gulp html
   ```

   This minifies the HTML, replaces references to CSS and JavaScript files with their minified versions, and copies them to `dist/`.

   ```bash
   gulp css
   ```

   This minifies the CSS files, adds a .min suffix to the filename, generates source maps and copies them to `dist/css/`.

   ```bash
   gulp js
   ```

   This minifies the JavaScript files, adds a .min suffix to the filename, generates source maps and copies them to `dist/js/`.

   ```bash
   gulp images
   ```

   This crunches images using imagemin and copies them to the `dist/img/` directory.

   ```bash
   gulp watch
   ```

   This watches for changes in HTML, CSS, JavaScript, and image files, triggers corresponding tasks and reloads the browser.


## Configuration

   * Source Files: Place your HTML, CSS, JavaScript and image files in their respective directories under `src/`. Simple "hello world" examples are given as placeholders.

   * Distribution: Optimized files are output to `dist/`.
