# remove-value-js

Remove one or more elements from an array by value

## Installation

	// npm
	$ npm install remove-value-js

## Usage

	var removeValue = require('remove-value-js');

	// as a function
	removeValue([ 'apple', 'lemon', 'banana', 'lemon' ], 'lemon'); // [ 'apple', 'banana' ]

	removeValue([ 'apple', 'lemon', 'banana', 'lemon' ], 'lemon', 1); // [ 'apple', 'banana', 'lemon' ]

	// as a method
	Array.prototype.remove = removeValue;

	var list = [ 'apple', 'lemon', 'banana' ];

	list.remove('banana');
	list; // [ 'apple', 'lemon' ]

	Alters the array "by reference" and returns the array.

## License

MIT