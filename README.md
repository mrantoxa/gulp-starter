# Gulp Build System

This is a Gulp-based build system designed to streamline the development workflow for modern web projects. It includes tasks for compiling SASS/SCSS, Pug templates, optimizing images, processing JavaScript, and more. The system also supports live reloading via BrowserSync for a seamless development experience.

## Features

- **SASS/SCSS Compilation**: Compiles SASS/SCSS files into minified CSS with autoprefixing.
- **Pug to HTML**: Converts Pug templates into HTML files.
- **JavaScript Optimization**: Concatenates and minifies JavaScript files.
- **Image Optimization**: Optimizes images (JPEG, PNG, SVG) and converts them to WebP format.
- **Fonts and Icons**: Copies fonts and icons to the output directory.
- **JSON Processing**: Parses and copies JSON files for use in the project.
- **Live Reload**: Automatically refreshes the browser on file changes using BrowserSync.

## Installation

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd <project-folder>
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Run the build system:**

   ```bash
   gulp
   ```

## How to Run

- **Development Mode:**

  Run the following command to start the development server with live reload:

  ```bash
  gulp
  ```

- **Build for Production:**

  Use this command to build the project without starting the development server:

  ```bash
  gulp build
  ```

- **Run Specific Tasks:**

  You can run individual tasks, such as:

  ```bash
  gulp sass     # Compile SASS/SCSS files
  gulp pug      # Compile Pug templates
  gulp scripts  # Process JavaScript files
  gulp imagemin # Optimize images
  ```

## Folder Structure

- `app/`: Source files.
  - `scss/`: SASS/SCSS files.
  - `views/`: Pug templates.
  - `js/`: JavaScript files.
  - `images/`: Image assets.
  - `fonts/`: Font files.
  - `icons/`: Icon files.
  - `data/`: JSON files.
- `dist/`: Compiled and optimized files (output directory).

## Available Tasks

- `gulp`: Default task. Runs the build process and starts a development server with live reload.
- `gulp build`: Builds the project without starting the development server.
- `gulp sass`: Compiles SASS/SCSS files.
- `gulp pug`: Compiles Pug templates into HTML.
- `gulp scripts`: Processes JavaScript files.
- `gulp imagemin`: Optimizes images and converts them to WebP.
- `gulp fonts`: Copies font files.
- `gulp icons`: Copies icon files.
- `gulp copy-json`: Copies JSON files to the output directory.
- `gulp watch`: Watches for changes in source files and triggers rebuilds.

## Dependencies

- **Gulp**: Task runner.
- **gulp-sass**: SASS/SCSS compilation.
- **gulp-pug**: Pug template compilation.
- **gulp-concat**: Concatenates files.
- **gulp-autoprefixer**: Adds vendor prefixes to CSS.
- **gulp-clean-css**: Minifies CSS.
- **gulp-uglify-es**: Minifies JavaScript.
- **gulp-imagemin**: Optimizes images.
- **gulp-webp**: Converts images to WebP.
- **browser-sync**: Live reload and local server.
- **gulp-debug**: Debugging for Gulp tasks.

## Contributing

Feel free to open issues or submit pull requests for improvements.

## License

This project is open-source and available under the [MIT License](LICENSE).
