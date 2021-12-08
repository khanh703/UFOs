# UFO Sightings

## Overview 

Dana would like her website to provide a more in-depth analysis of UFO sightings by allowing her visitors additional filter parameters. Dana would like to additional filters for city, state, country, and shape. 
 


## Results 

Dana's UFO website now gives visitors the ability search by city, state, country, and shape in addition to date.
 



## Summary 
The website met Dana's criteria, however with one major drawback. All search results are exact matches only. Meaning if the user misspells a city, state, country, or shape... the search function will not return results. There are two possible solutions:

- Search function uses regex to find partial match. i.e. searching "tuc" will also return "Tucson"
- Setup each text field as a select dropdown and populate options with known Cities, States, Countries, and Shapes.


## Technical

1. An event listener is attached to each input fields and listens for a "change" event. 
2. When a "change" event is detected, function "updateFilters" is called
3. updateFilter checks if a value was entered for that filter Id, that filter will be added to the "filters" object, otherwise remove that filter from the "filters" object"
4. Once the "filters" object has been updated, function "buildTable" is called, passing in the "filters" object
5. The "buildTable" function first clears out the existing HTML table than loops through the data object and appends a table row for each row and table data cell for each property.

*figure 1*   
![Employee Database](https://raw.githubusercontent.com/khanh703/UFOs/main/static/images/input_fields.png)

*figure 2*
![Employee Database](https://raw.githubusercontent.com/khanh703/UFOs/main/static/images/code_image.png)
