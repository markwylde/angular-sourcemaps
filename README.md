# angular-sourcemaps
The Mozilla Sourcemap library is a brilliant project from Mozilla to help with sourcemaps in the browser. This project has the compiled distribution files from the official repo, along with an AngularJS app.

# Notes
This will not actually generate SourceMaps for your javascript files. Instead, when an error occurs from with an Angular controller or a TypeScript library, the AngularJS exception report will include the original source mapping.

## How to install
### 1a) Add to bower
    bower install https://github.com/markwylde/angular-sourcemaps.git

** Sorry, I will get this added to bower properly soon

### or 1b) Manually download
	git clone https://github.com/markwylde/angular-sourcemaps.git

### 2) Include the following files in your html file
	<script src="angular-sourcemaps/dist/angular-sourcemaps.min.js"></script>
    <script src="angular-sourcemaps/dist/source-map.min.js"></script>

### 3) Add the dependancy in your AngularJS app
	angular.module('myApp', [
	    'angular-sourcemaps'
	])
