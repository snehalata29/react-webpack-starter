npm init
git init
create public and src folder
and index.html file into public folder
<body>
  <div id="root"></div>
  <noscript>
    You need to enable JavaScript to run this app.
  </noscript>
  <script src="../dist/bundle.js"></script>
</body>
npm install --save-dev @babel/core@7.1.0 @babel/cli@7.1.0 @babel/preset-env@7.1.0 @babel/preset-react@7.0.0
babel code ---- main babel package
babel-cli  ---- allows you to compiles file from command line
preset env ---- allows to  transform es6 into more traditional javascript
preset react ---- allows to transform jsx into javascript

create .babelrc file at the root folder telling babel we are using pesets
add 
{
    "presets": ["@babel/env", "@babel/preset-react"]
}

now need webpack

npm install webpack webpack-cli webpack-dev-server
npm install style-loader css-loder babel-loader
 
add webpack.config.js

entry : starting point in app
module           : object helps define how your exported javascript modules are transformed and which ones 
                    are included according to the given array of rules.
test and exclude : The  and  properties are conditions to match file against.
loader and use   : loader is a shorthand for the use property, when only one loader is being utilized.
                 :  The resolve property allows us to specify which extensions Webpack will resolve —  this       allows us to import modules without needing to add their extensions
resolve          : The resolve property allows us to specify which extensions Webpack will 
                    resolve — this allows us to import modules without needing to add their extensions.

