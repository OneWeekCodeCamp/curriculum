# Javascript

You'll do these exercises in [repl.it](https://repl.it/), and online coding editor.

## Exercise 1 - Arrays:

First, paste the array below into the editor.

	var fruits = ["apple","banana","kiwi", "pine apple"];

* Print the fruits array out in the console.
* Store the length of the array in a variable called fruitLength
* Add a fifth fruit to the array using the push() method
* Loop through the modified array, and print the following to the console:  

	*I like apples*  
	*I like bananas*  
	*I like lemons*  
	*etc etc...* 
* Loop through the modified array, creating a new array which only contain the fruits which have below six letters in them.


## Exercise 2 - Objects:

	var image = {
		url: 'www....',
		width: '200px',
		height: '200px',
		people: ['john','nina','jack','liz'],
		photographer: {
			firstName: 'John',
			lastName: 'Smith'
		}
	}

* Loop through the object an print the values to the console
* Change the value of the *width* key to '300px'
* Add a new key called *date* and give it the value '22/08/15'
* Loop through the array in the people value and print out the names to the console
* Print the photographers last name to the console


## Exercise 3 - Functions

* Create a function named *add()*, which takes two variables and returns the product of the two
* Create a function which [concatinates](http://www.w3schools.com/jsref/jsref_concat_array.asp) two arrays together
* Create a function which takes one argument and returns true if the argument is a number and false if the argument is a string. (hint, check out [typeof](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/typeof))
* Create a function - myFunction - which loops through an array and prints out every item to the console
* Modify myFunction so that it only prints the value if the item has got over 5 characters
* Modify myFunction so that it **returns** a new array contrining only the items witch are more than 5 chararacters


## Examples

### Strings

	var myString = "Hello";
	var strLength = myString.length();
	console.log(strLength);
	// prints 5 to the console 

	var x = "1";
	var y = "2";

	var z = x + y;

	console.log(z);

### Numbers

	var x = 1;
	var y = 2;

	var z = x + y;

	console.log(z);

### Arrays

	var fruits = ["apple","banana","kiwi", "pine apple"];
	var foo = fruits[0];
	// foo stores the value "apple";

	var fruitLength = fruits.length;
	// fruitLength stores the number 4

	fruits.push("mango");
	// adding the "mango" to the fruits array


### Looping 

	for(var i = 0; i < fruitLength; i++){
		console.log(fruits[i]);
	}

### if else 

	for(var i = 0; i < fruitLength; i++){
			if(fruits[i] === "mango"){
			console.log("I found the" + fruits[i]);
		}
	}


### Objects

Here is an example object: 

	var image = {
		url: 'www....',
		width: '300px',
		height: '200px',
		people: ['john','nina','jack','liz'],
		photographer: {
			firstName: 'John',
			lastName: 'Smith'
		}
	}

**Dot notation**	 
	
	var h = image.height;
	console.log(h);
	// prints '200px' to the console
	
**Bracket notation**  
	
	var w = image["width"];
	console.log(w);
	// prints '300px' to the console

**Fetching deep values**  
	
	var firstN = image.photographer.firstName;
	console.log(firstN);
	// prints John to the console

**Looping through objects**

	for (var key in image) {
		console.log(image[key]);
	}

	// prints out the values

**Adding a property to an object**

	image.cameraType = 'Canon 500D';
	// now, the image object  has got a key cameraType which takes on the value 'Canon 500D'

### Functions

A JavaScript function is a block of code designed to perform a particular task.

**Creating a function**

There are two ways of creating a function:

	// Function expression
	var foo = function(){
		console.log('This is a function')
	}
	
	// Function declaration
	function foo(){
		console.log('This is a function')
	}

	// You call a function by stating its name followed by parenthesis. Like this:

	foo();
	// prints out "This is a function" to the console.

**Arguments**

Within the functions parenthesis, you can add *arguments*. These are values which the function can access in the function body.
	
	var myFunc = function(a,b){
		console.log('my first argument is ', a);
		console.log('my secondd argument is ', b);
	}

	myFunc('hello', 123);

Very often, you'll want your function to return a value, after its executed some code (e.g. calculations).

	var add = function(a,b){
		return a+b;
	}

	add(5,6);
	//returns 11





