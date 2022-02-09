## Installation

- Webpack installation `npm i D webpack webpack-cli webpack-dev-server`
- Babel installation `npm install -D babel-loader @babel/core @babel/preset-env @babel/node @babel/register html-webpack-plugin`
- Create into root derectory file `.babelrc`

## Quick Installation JavaScript Project

- Download app `https://createapp.dev/`
- Install webpack dev server `npm i webpack-dev-server`
- change and replace webpack.config.js file

```
  devServer: {
   static: {
     directory: path.join(__dirname, 'src'),
   },
   compress: true,
   port: 9000,
   open: true,
 },

```

- change and replace package.json file

```
    "start": "webpack-dev-server"

```
