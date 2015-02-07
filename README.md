# onhand
Javascript sourcecode documentation viewer

It saves your time and time of your potential users by simplifying product documentation delivery since it enforces you to focus on commenting your code thus making your library developer-friendly.

It is implemented as a single HTML page capable of extracting whole tree of javascript function declarations and corresponding documentation javadoc comments from specified resource.

Designed with Modern HTML5 compliant browser in mind. Refer to the compatibility table below for more information.

### Applicable for
* javascript library deployment to provide developer-friendly self documented API's
* learning large javascript API's like jQuery, Ace, ExtJS etc.

### Examples
* jQuery doc: http://onhand.googlecode.com/svn/trunk/onhand.html?target=test.js
* Self doc: http://onhand.googlecode.com/svn/trunk/onhand.html?self

### Features
* source syntax highlight with google-code-prettify
* JS beautified (unminified) with jsbeautifier.org
* extracted function definition set can be viewed as columns or tree
* nested function declarations folding
* raw source view

### Usage
The javascript source can be given by
* URL of online resource
* file upload or drag and drop into designated zone
* copy/pasting source code into textarea
* static linking, where each JS script can have his own documentation page, _named exactly the same_ but having html extension like so:
```
 script.js           // your source code
 script.html         // documentation browser page that describes script.js
```
* dynamic linking, where each script can be referenced using single documentation page through `target` URL parameter like that
```
"http://.../onhand.html?target=script1.js"       // documentation for script1.js
"http://.../onhand.html?target=lib/script2.js"   // documentation for script2.js from ./lib directory
```
