# Webpack

Create React app manually.

1. Setup NPM

   Run `npm init -y`

2. Create the file structure

```
- dist
  -- index.html
  -- bundle.js
- webpack.config.js
-src
  -- index.js
- .eslintrc.json
```

- in the file `dist/index.html`

  a. add title

  b. create a div which will be the entry point for the React app

  c. create a script tag pointing to the source `bundle.js`

3. Install Webpack

   Run `npm i --save-dev webpack webpack-dev-server webpack-cli`

   `webpack` will be a module bundler and a building tool

   `webpack-dev-server` serves this bundled js up that it is possible to test the app locally.

   `webpack-cli` to configure webpack setup

4. Add start script in `package.json` file

   Add `webpack-dev-server --config <config.js path> --mode development` on the start script.

   `--mode development` adds default webpack configurations

   `webpack-dev-server --config ./webpack.config.js --mode development`

5. Config `webpack.config.js` file

   Export the entry and output points.

   Export the development server which tells where to serve the content from.

6. Install Babel

   Run `npm i --save-dev @babel/core babel-loader @babel/preset-env`

   `babel-core` is the main babel package

   `babel-loader` compiles code. It is used in webpack. The webpack takes the JS and take it to the babel compiler

   `babel-present-env` checks which version the browser runs and coverts the features the browser does not understand

7. Add Babel in `package.json`

   You can also create a `.babelrc` file and add the configurations.

   ```
   {
      "babel": {
         "presets": [ ... ],
         "plugins": [ ... ],
      }
   }
   ```

   Run `npm i --save-dev babel-preset-react`

8. Add Babel in `webpack.config.js`

9. Install `react` and `react-dom`

10. Install `eslint` and `eslint-loader`

Run `npm i --save-dev eslint eslint-loader`

Config `.eslintrc.json` file

11. Add `eslint-loader` in `webpack.config.js`

12. Install `babel-eslint`

Run `npm i --save-dev babel-eslint`

Config `.eslintrc.json` file

13. Install `eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y`

Run `npm i --save-dev eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx-a11y`

`eslint-config-airbnb` for airbnb configurations

`eslint-plugin-import` for import and export

`eslint-plugin-jsx-a11y` for accessibility

Config `.eslintrc.json` file

```

```
