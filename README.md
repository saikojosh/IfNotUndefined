# IfNotUndefined
A shorthand helper function for the pattern: `const x = (typeof y !== 'undefined' ? y : 'default-value');`

## Usage
```javascript
const ifNotUndefined = require('ifnotundefined');

function MyFunc (options = {}) {
	this.timeout = ifNotUndefined(options.timeout, null);  // the default value for timeout will be null.
	this.encoding = ifNotUndefined(options.encoding, 'utf8');  // the default value for encoding will be 'utf8'.
	...
}
```
