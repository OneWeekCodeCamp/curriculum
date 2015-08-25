# Javascript

## Exercise 1 - Arrays:

You'll do these exercises in repl.it. First, paste the array below into the editor.

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
		people: ['john','nina','jack','liz']
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

* Create a function named *add()*, which takes two variables and returns the sum of them
* Create a function which concatinates two arrays together
* Create an array which takes one argument and returns true if it's and even number and false if it's an odd number
* Create a function - myFunction - which loops through an array and prints out every item to the console
* Modify myFunction so that it only prints the value if the item has got over 5 characters
* Modify myFunction so that it **returns** a new array contrining only the items witch are more than 5 chararacters


## Examples

### Strings

	var myString = "Hello";
	var strLength = myString.length();
	console.log(strLength);
	// prints 5 to the console

Concatentation 

	var x = "1";
	var y = "2";

	var z = x + y;

	console.log(z);

	var x = 1;
	var y = 2;

	var z = x + y;

	console.log(z);

### Arrays

	var fruits = ["apple","banana","kiwi", "pine apple"];
	var foo = fruits[0];
	// foo stores the value "apple";
	var fruitLength = fruits.lengt()
	// fruitLength stores the number 4

	fruits.push("mango");


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


	


