# Morning exercise.

Solve this exercise on repl.it.

This is an example of a JSON object you will typically get back from an AJAX call. We want you to navigate into it and fetch the dog names. Store them in an array called dogNames.

Finally, loop through the dogNames array, and log the names to the console, using console.log.


	results = {
		"site": "flickr",
		"tags": "dogs",
		"dogs":[{"name": "figo", "size": "l"},
			    {"name": "pluto","size": "s"},
			    {"name": "fia","size": "m"},
			    {"name": "alfred","size": "s"},
			    {"name": "rose","size": "m"}] 
	}


## Solution:

	var dogsArray = results.dogs;
	var dogNames = [];
	for (var i=0;i<dogsArray.length; i++){
	   dogNames.push(dogsArray[i].name)
	}
	console.log(dogNames);



# JQUERY AND AJAX 2nd Day

## First Exercise
* Create a html file link to the jquery library (local or cdn) and make sure jquery has loaded.
* Create 3 buttons each with the name of an animal so when the user clicks the name of the animal will be logged in the console.
* Create an AJAX request to the flickr api to fetch the value of the button clicked.
* Render the animal Images on the page.

## Stretch Goals
* Clear the content when a new button is clicked.
* Allow the user to be able to choose between viewing 5, 10, 20 images on the page.
* Styling your application.