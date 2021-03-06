shake.js
=======================================

A custom 'shake' event JavaScript plugin for mobile web browsers using device accelerometer.

Dependencies
---------------------------------------

Your web browser must support the `devicemotion` event for this plugin to work. Shake.js uses built-in feature detection to determine if it can run in your web browser. It will terminate silently on non-supporting browsers.

http://dev.w3.org/geo/api/spec-source-orientation

Setup
---------------------------------------

First, include the main JavaScript file in the `<head>` of your HTML document:

```
<script src="shake.js"></script>
```

Next, listen for the custom 'shake' event:

```
window.addEventListener('shake', shakeEventDidOccur, false);
	
//function to call when shake occurs
function shakeEventDidOccur () {
	
	//put your own code here etc.
	if (confirm("Undo?")) {

	}
}
```

You can stop listening for shake events like so:

```
window.removeEventListener('shake', shakeEventDidOccur, false);
```
	
Supported browsers/devices
---------------------------------------

- Mobile Safari, iOS 4.2.1 (and above)
	
License
---------------------------------------

Copyright (c) 2009-2012 Alex Gibson

http://miniapps.co.uk/

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction except as noted below, including without limitation the rights to use, copy, modify, merge, publish, distribute, and/or sublicense, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE