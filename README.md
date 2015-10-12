# elixir-angular-template-cache

Original project by Logan Henson, see https://github.com/loganhenson/laravel-elixir-angular-templatecache

## Installation
----

```sh
$ npm install elixir-angular-template-cache
```

## Usage
----

Require the extension and call it using mix.angulartemplatecache(). 

```javascript
var elixir = require('laravel-elixir');
require('elixir-angular-template-cache');

elixir(function(mix)
{
	mix.angulartemplatecache(
   		{module: 'app', root: 'templates'}, 	//	template cache options
   		'public/app/views/cached/**', 			//	source 
   		'public/app/js', 						//	destination
   		'templates'								//	wrap
	);	
});
```

Run gulp.

```sh
$ gulp
```