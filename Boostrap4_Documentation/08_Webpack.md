

Webpack
Learn how to include Bootstrap in your project using Webpack 3.

Try DigitalOcean today and get a free $100 credit.
ads via Carbon
Installing Bootstrap
Install bootstrap as a Node.js module using npm.

Importing JavaScript
Import Bootstrap’s JavaScript by adding this line to your app’s entry point (usually index.js or app.js):

Copy
import 'bootstrap';
Alternatively, you may import plugins individually as needed:

Copy
import 'bootstrap/js/dist/util';
import 'bootstrap/js/dist/dropdown';
...
Bootstrap is dependent on jQuery and Popper, these are defined as peerDependencies, this means that you will have to make sure to add both of them to your package.json using npm install --save jquery popper.js.

Notice that if you chose to import plugins individually, you must also install exports-loader

Importing Styles
Importing Precompiled Sass
To enjoy the full potential of Bootstrap and customize it to your needs, use the source files as a part of your project’s bundling process.

First, create your own _custom.scss and use it to override the built-in custom variables. Then, use your main sass file to import your custom variables, followed by Bootstrap:

Copy
@import "custom";
@import "~bootstrap/scss/bootstrap";
For Bootstrap to compile, make sure you install and use the required loaders: sass-loader, postcss-loader with Autoprefixer. With minimal setup, your webpack config should include this rule or similar:

Copy
  ...
  {
    test: /\.(scss)$/,
    use: [{
      loader: 'style-loader', // inject CSS to page
    }, {
      loader: 'css-loader', // translates CSS into CommonJS modules
    }, {
      loader: 'postcss-loader', // Run post css actions
      options: {
        plugins: function () { // post css plugins, can be exported to postcss.config.js
          return [
            require('precss'),
            require('autoprefixer')
          ];
        }
      }
    }, {
      loader: 'sass-loader' // compiles Sass to CSS
    }]
  },
  ...
Importing Compiled CSS
Alternatively, you may use Bootstrap’s ready-to-use css by simply adding this line to your project’s entry point:

Copy
import 'bootstrap/dist/css/bootstrap.min.css';
In this case you may use your existing rule for css without any special modifications to webpack config except you don’t need sass-loader just style-loader and css-loader.

Copy
  ...
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ['style-loader', 'css-loader']
      }
    ]
  }
  ...
  