

Download
Download Bootstrap to get the compiled CSS and JavaScript, source code, or include it with your favorite package managers like npm, RubyGems, and more.

The new generation of project management tools is here and it’s visual.
ads via Carbon
Compiled CSS and JS
Download ready-to-use compiled code for Bootstrap v4.0.0 to easily drop into your project, which includes:

Compiled and minified CSS bundles (see CSS files comparison)
Compiled and minified JavaScript plugins
This doesn’t include documentation, source files, or any optional JavaScript dependencies (jQuery and Popper.js).


Source files
Compile Bootstrap with your own asset pipeline by downloading our source Sass, JavaScript, and documentation files. This option requires some additional tooling:

Sass compiler (Libsass or Ruby Sass is supported) for compiling your CSS.
Autoprefixer for CSS vendor prefixing
Should you require build tools, they are included for developing Bootstrap and its docs, but they’re likely unsuitable for your own purposes.


BootstrapCDN
Skip the download with BootstrapCDN to deliver cached version of Bootstrap’s compiled CSS and JS to your project.

Copy
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
If you’re using our compiled JavaScript, don’t forget to include CDN versions of jQuery and Popper.js before it.

Copy
<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
Package managers
Pull in Bootstrap’s source files into nearly any project with some of the most popular package managers. No matter the package manager, Bootstrap will require a Sass compiler and Autoprefixer for a setup that matches our official compiled versions.

npm
Install Bootstrap in your Node.js powered apps with the npm package:

Copy
npm install bootstrap
require('bootstrap') will load all of Bootstrap’s jQuery plugins onto the jQuery object. The bootstrap module itself does not export anything. You can manually load Bootstrap’s jQuery plugins individually by loading the /js/*.js files under the package’s top-level directory.

Bootstrap’s package.json contains some additional metadata under the following keys:

sass - path to Bootstrap’s main Sass source file
style - path to Bootstrap’s non-minified CSS that’s been precompiled using the default settings (no customization)
RubyGems
Install Bootstrap in your Ruby apps using Bundler (recommended) and RubyGems by adding the following line to your Gemfile:

Copy
gem 'bootstrap', '~> 4.0.0'
Alternatively, if you’re not using Bundler, you can install the gem by running this command:

Copy
gem install bootstrap -v 4.0.0
See the gem’s README for further details.

Composer
You can also install and manage Bootstrap’s Sass and JavaScript using Composer:

Copy
composer require twbs/bootstrap:4.0.0
NuGet
If you develop in .NET, you can also install and manage Bootstrap’s CSS or Sass and JavaScript using NuGet:

Copy
Install-Package bootstrap
Copy
Install-Package bootstrap.sass
