# React + Redux + Webpack 2 starter project

This project built using [Create React App](https://github.com/facebookincubator/create-react-app) and then modified to allow customizations in it's build process.
All dependencies where updated to work with Webpack 2 as well as configuration files.

## Features

- React + Redux;
- Webpack 2 configured for development and production;
- Live reloading enabled;
- Support for SASS/SCSS styles;
- JavaScript and SASS/SCSS linters;
- Testing;
- Include font-related files (eg.: '.woff', 'woff2' and '.ttf') when building.

### Project description

```
my-app/
  build/
  	- [Auto-generated] Contains the bundled version after `build` process. It can be changed in `config/path.js`.
  config/
    - Centers all configuration and scripts files.
	- `.eslintrc.json` and `.stylelintrc.json` can be customized as needed.
  public/
    - Public files.
  src/
    - The APP's source files (eg.: '.js', '.scss').
```

## Available Scripts

From the project's root directory:

### `npm start`

Runs `config/scripts/start.js`.

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm test`

Runs `config/scripts/tests.js`.

Launches the test runner in the interactive watch mode.  

### `npm run build`

Runs `config/scripts/build.js`.

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>

## Editors

Suggestions of configurations for specifc editors.

### Visual Studio Code

Install [Eslint plugin](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint).

Install [Stylelint plugin](https://marketplace.visualstudio.com/items?itemName=shinnn.stylelint).

**settings.json:**
```
{
	// "Cleans" workspace directory.
	"files.exclude": {
		"**/.git": true,
		"**/.DS_Store": true,
		"**/node_modules/": true
	},
	"emmet.syntaxProfiles": {
		// Enable JSX's HTML syntax when using Emmet expressions in '.js' and '.jsx' files.
		"javascript": "jsx"
	},
	"scss.validate": false,
	"stylelint.enable": true,
	"stylelint.config": {
		// Share same configurations as when building APP for SCSS files.
		"extends": "./config/.stylelintrc"
	},
	"eslint.enable": true,
    "eslint.options": {
		// Share same configurations as when building APP for JavaScript files
        "configFile": "./config/.eslintrc.json"
    }
}
```
