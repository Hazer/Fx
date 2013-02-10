#Fx.js

A super lightweight, high performance, cross-browser, dependency-free animation library for the modern web.

##Features:

- **Super lightweight**: Just 3kb minified
- **High performance**: Uses requestAnimationFrame and hardware-accelerated CSS transforms, degrades gracefully in older browsers
- **Cross browser**: Tested in Chrome, Safari, Firefox, Opera, iOS, Android, and IE6+
- **Dependency-free**: No jQuery, no MooTools, no YUI, no Closure
- **Supports module loaders**: CommonJS and AMD

##Usage

```javascript

var fx = new Fx(DOMElement, property, options);

fx.get();		// get current value of the property

fx.set(value);	// immediately set value

fx.to(value);	// animate to value
```

##Example

```javascript

var element = document.getElementById('myElement');
var fx = new Fx(element, 'top', {
	duration: 1000
}).to(100);
```

##Options

- `duration` (Number) The animation duration (in milliseconds)
- `animationStart` (Function) Animation start hook
- `animationEnd` (Function) Animation end hook

##To do:

- Unit tests
- Support for more units
- Support for more transitions
- Support for transitioning multiple properties
- Support for class transitions