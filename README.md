# jQueryCreate
	
>	"Why haven't anyone done this before?" **-  Future You**

No learning curve - The jQueryCreate plugin is simple, intuitive and extremely useful. Just plug and play.

The jQuery creator plugin Allows you to create your elements using CSS selectors syntax.
Don't use javascript with different syntaxes when it comes to dynamic DOM element creation. 
Use the same syntax for element querying and creation.

## Details
* **Author**: EZSlaver (Erez Zinman)
* **Date**: 05.02.2013
* **Current Version**: 0.9.0
* **License**: MIT License

## Usage
Add the plugin to your HTML page, and do this only after you add the jQuery reference.

Now, you can use the $c() command to create your elements.

## Remarks
* The plugin doesn't support the 'style' attribute. Yet...

## Code Examples:
```javascript
	// Returns a wrapped element to be used directly via jQuery.
	var $newDiv = $c('div#New').append($c('input[type=text].shows-default-value'));
	$('body').append($newDiv).append($c('div.seperator'));
```
### Usages:
```javascript
var $div = $c("div");
$div = $c("div#foo");
$div = $c("div.bar");
$div = $c("div#foo.bar");
$div = $c("div.bar#foo");
$div = $c("div.bar#foo.foo");
$div = $c("div.bar.foo#foo");
$div = $c("div[disabled=disabled]");
$div = $c("div[disabled=disabled].bar");
$div = $c("div[disabled=disabled]#foo");
$div = $c("div[disabled=disabled]#foo.bar");
$div = $c("div[disabled=disabled][selected=true]#foo.bar");
$div = $c("div[disabled=disabled][selected=\"true\"]#foo.bar");
$div = $c("div[disabled=disabled][selected=\"very true\"]#foo.bar");
$div = $c("div[disabled=disabled][selected=\"very:true\"]#foo.bar");
```

## Licensing
Copyright (C) 2010-2013 [Erez Zinman](mailto://EZSlaver@gmail.com)
 * Licensed under the MIT License
 * http://www.opensource.org/licenses/mit-license.php
