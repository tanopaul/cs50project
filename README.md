# Pokedex!

## Video Demo

## Description

Scroll through the Pokemon directory, view each Pokemon description, and build your team. This project was made by fetching data from the Pokemon API. Users have the ability to scroll through a list of Pokemon. Once the user clicks on a specific card, the Pokemon's image and their information will be displayed.
Users can build their personal Pokemon deck team by adding the Pokemon to their team inventory(team limit is set to 6).Users can delete a Pokemon from their team as well as search for specific Pokemon.
The index.js file is where the functionality of the app comes into play. A fetch statement that calls the PokeAPI url returns a response that is to be translated into JSON format, stored in a variable as an array of objects, and then sent through to the renderPokedex function.
The renderPokedex function receives each pokemon and creates new elements within the DOM. Event listeners are also dynamically created and assigned to every pokemon that is rendered in the pokedex list.
The "click" event listener sends a fetch request to the pokeAPI for the specific character that was clicked and returns all of the information about that pokemon to be displayed in the two boxes on the right. Getting the correct weight and height of each pokemon was a challenge because the data that the API was sending back was in decimeters and hectograms, so I needed to convert the weight into inches and pounds.
Lastly, once a pokemon that is selected is added to your team with the "add to team" button, it will be displayed in one of the boxes below. There is an event listener to add pokemon to your team and a listener to delete pokemon from your team while shifting all pokemon to left so that no empty spaces occur in the center.
