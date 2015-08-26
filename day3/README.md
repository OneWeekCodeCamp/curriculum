# Jquery and Ajax

Download [jQuery](http://code.jquery.com/jquery-1.11.3.js) (scroll down to the uncomressed development version 1.11.3, and click the link). Secondly you'll have to load the jQiery library into your HTML file using the script tag.  

Remember to use the [jQuery docs](https://jquery.com/) if you're unsure of how to do stuff.

##First Exercise
* add an input field with an id of *searchQuery* and a button with the id of *searchButton* to the html file.
* add an event handler for button click which console.log's "clicks".
* when the user clicks the button log the text from the input field to the console.

##Second Exercise
* create an Ajax request to the variable named itunesURL and console.log() the results.
* navigate through the JSON response object and push the songtitles into a new Array. Console.log the new Array.
* Loop through the new Array and output the songtitles in an unordered list on your webpage.

##Third Exercise
* modify the itunesURL so that it contains the string value of the searchQuery input field instead of Beyonce.
* add the Artists artwork above each song title.
* add a clear button.

##Stretch Goals

* add a link to each of the results in the list


## Examples

### How to link to jQuery

Place the jQuery file in the same folder as your *index.html* and link to it using the follownig script tag:

	<script src="jquery-1.11.3.js" ></script>

## How to register a button click

	$("#searchButton").click(function(){
		// code what you want to happen when the user clicks the button
	});