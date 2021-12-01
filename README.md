# UFO Sitings

## Overview 

Dana would like her website to provide a more in-depth analysis of UFO sightings by allowing her visitors additional filter parameters. Dana would like to additional filters for city, state, country, and shape. 
 


## Results 

Dana's UFO website now gives visitors the ability search by city, state, country, and shape in addition to date.
 



## Summary 
The website met Dana's criteria, however with one major drawback. All search results are exact matches only. Meaning if the user misspells a city, state, country, or shape... the search function will not return results. There are two possible solutions:

- Search function uses regex to find partial match. i.e. searching "tuc" will also return "Tucson"
- Setup each text field as a select dropdown and populate options with known Cities, States, Countries, and Shapes.
