# js-cheatsheet

<<<<<<< HEAD
## debounce
```
// Returns a function, that, as long as it continues to be invoked, will not
// be triggered. The function will be called after it stops being called for
// N milliseconds. If `immediate` is passed, trigger the function on the
// leading edge, instead of the trailing.
function debounce(func, wait, immediate) {
	var timeout;
	return function() {
		var context = this, args = arguments;
		var later = function() {
			timeout = null;
			if (!immediate) func.apply(context, args);
		};
		var callNow = immediate && !timeout;
		clearTimeout(timeout);
		timeout = setTimeout(later, wait);
		if (callNow) func.apply(context, args);
	};
};
```
```
var myEfficientFn = debounce(function() {
	// All the taxing stuff you do
}, 250);

window.addEventListener('resize', myEfficientFn);
```
Source: [JavaScript Debounce Function](https://davidwalsh.name/javascript-debounce-function)
=======
## Links
* [es6 cheatsheet](https://github.com/DrkSephy/es6-cheatsheet)
>>>>>>> c60b0b60be582452f508b7b29f7f5d35fcecfaaa
