![phaser3-snowpack-header](https://user-images.githubusercontent.com/2236153/92626686-7c693d80-f287-11ea-91a1-d54d64be38e4.png)

# Phaser 3 + Snowpack Template
> Modern and fast build tool for making games with Phaser 3 and modern JavaScript

![License](https://img.shields.io/badge/license-MIT-green)

## Prerequisites

You'll need [Node.js](https://nodejs.org/en/) and [npm](https://www.npmjs.com/) installed.

It is highly recommended to use [Node Version Manager](https://github.com/nvm-sh/nvm) (nvm) to install Node.js and npm.

For Windows users there is [Node Version Manager for Windows](https://github.com/coreybutler/nvm-windows).

Install Node.js and `npm` with `nvm`:

```bash
nvm install node

nvm use node
```

Replace 'node' with 'latest' for `nvm-windows`.

## Getting Started

Clone this repository to your local machine:

```bash
git clone https://github.com/ourcade/phaser3-snowpack-template.git
```

This will create a folder named `phaser3-snowpack-template`. You can specify a different folder name like this:

```bash
git clone https://github.com/ourcade/phaser3-snowpack-template.git my-folder-name
```

Go into your new project folder and install dependencies:

```bash
cd phaser3-snowpack-template # or 'my-folder-name'
npm install
```

Start development server:

```
npm run start
```

To create a production build:

```
npm run build
```

Production files will be placed in the `build` folder. Then upload those files to a web server. 🎉

## Project Structure

```
    .
    ├── build
    ├── node_modules
    ├── public
	│   ├── index.html
    ├── src
    │   ├── scenes
    │   │   ├── HelloWorldScene.js
    │   ├── main.js
    ├── package.json
```

The contents of this template is the basic [Phaser3 getting started example](http://phaser.io/tutorials/getting-started-phaser3/part5).

This template assumes you will want to organize your code into multiple files and use modern JavaScript.

JavaScript files are intended for the `src` folder. `main.js` is the entry point referenced by `index.html`.

Other than that there is no opinion on how you should structure your project. There is a `scenes` folder in `src` where the `HelloWorldScene.js` lives but you can do whatever you want.

## Static Assets

Any static assets like images or audio files should be placed in the `public` folder. It'll then be served at http://localhost:8000/images/my-image.png

Example `public` structure:

```
    public
    ├── images
    │   ├── my-image.png
    ├── music
    │   ├── ...
    ├── sfx
    │   ├── ...
```

They can then be loaded by Phaser with `this.image.load('my-image', 'images/my-image.png')`.

# ESLint

This template uses a basic `eslint` set up for code linting to help you find and fix common problems in your JavaScript code.

It does not aim to be opinionated.

[See here for rules to turn on or off](https://eslint.org/docs/rules/).


## Dev Server Port

You can change the dev server's port number by modifying the `snowpack.config.json` file under `devOptions.port`.

## License

[MIT License](https://github.com/ourcade/phaser3-snowpack-template/blob/master/LICENSE)
