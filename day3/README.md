# Jquery and Ajax

Download [jQuery](http://code.jquery.com/jquery-1.11.3.js) (scroll down to the uncomressed development version 1.11.3, and click the link). Secondly you'll have to load the jQiery library into your HTML file using the script tag.  

Remember to use the [jQuery docs](https://jquery.com/) if you're unsure of how to do stuff.

##First Exercise
* add an input field with an id of *searchQuery* and a button with the id of *searchButton* to the html file.
* add an event handler for button click which console.log's "clicks".
* when the user clicks the button log the text from the input field to the console.

##Second Exercise

Here is the link to the iTunes URL: 'https://itunes.apple.com/search?term=jack+johnson'.

* create an Ajax request to the variable named itunesURL and console.log() the results.
* navigate through the JSON response object and push the songtitles into a new Array. Console.log the new Array.
* Loop through the new Array and output the songtitles in an unordered list on your webpage.

##Third Exercise
* modify the itunesURL so that it contains the string value of the searchQuery input field instead of Beyonce.
* add the Artists artwork above each song title.
* add a clear button.

##Stretch Goals

* add a link to each of the results in the list


## Exercise 1 examples

### How to link to jQuery

Place the jQuery file in the same folder as your *index.html* and link to it using the follownig script tag:

	<script src="jquery-1.11.3.js" ></script>

### How to register a button click

	$("#searchButton").click(function(){
		// code what you want to happen when the user clicks the button
	});

### How to fetch the value from an input text field

	var mySearchQuery = $("#searchQuery").val():

## Exercise 2 examples

### How to create an Ajax request

	$.ajax({
		url: someRandomUrl,
		dataType: 'jsonp',
		success: function(itunesData){
			// do whatever you want with the data you get back from the API
		} 
	});

### How to fetch the correct data

You'll need to grab the *results* array in your success callback function:

		success: function(itunesData){
			// navigate through the iTunesData to the *results* array
			var myResults = itunesData.results;
		} 

### Looping through an array and fetch your variable of choice

This is how you create a for loop to loop through an array og objects, and fetching the variable you want to grab. In our case, this variable is called *trackName*:

	// the array is called myResults
	var trackNamesArray = []
	for (var i = 0; i < myResults.length; i++){
		var myTrack = myResults.trackName;
		 trackNamesArray.push(myTrack);
	}

	// now, you've stored all the track names in an array called *trackNamesArray*. Hurray!



