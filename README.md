# Grupo API Service Bar
![services-bar](http://s18.postimg.org/iw6ho7eah/image.gif)
> Gapi Service Bar is an AngularJS Directive that provide access to different applications and user config.

#### How to Install:

Via bower
``` bower install gapi-service-bar ```

It will include the following structure to your bower's package folder:

```
├── style.css
├── gapi-service-bar.html
├── gapi-service-bar.min.js
├── gapi-service-bar.min.js.map
├── bower.json
├── .bower.json
├── LICENSE
├── README
```

### Adding to your project

Firstly you must have bower already installed to run this command:
```sh
bower install gapi-service-bar
```

Add it to your AngularJS Module as dependency:
``` javascript
angular.module('yourProject', ['gapiServiceBar'];
```

Refer on your html
``` html
<head></head>
```
The following files:

``` html
<link type="text/css" href="vendor/gapi-service-bar/style.css" rel="stylesheet" /> 
<script type="text/javascript" src="vendor/gapi-service-bar/gapi-service-bar.min.js"></script>
```

Include the directive on your HTML:
``` html
<gapi-service-bar></gapi-service-bar>
```

There we go!
