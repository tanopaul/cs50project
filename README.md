# Pokedex!

#### Video Demo: https://youtu.be/ginEpWqBJsQ

#### Description

Explore the Pokemon directory, peruse each Pokemon's description, and assemble your dream team. This project was crafted by extracting data from the Pokemon API. Users can easily navigate a comprehensive list of Pokemon. When a specific card is clicked, the Pokemon's image and details will be showcased.

Users can curate their own personalized Pokemon squad by adding them to their team inventory (with a maximum limit of 6). They also have the option to remove a Pokemon from their team and search for specific Pokemon.

The index.js file houses the core functionality of the app. A fetch statement is employed to call the PokeAPI URL, which yields a response to be converted into JSON format. This data is then stored as an array of objects, subsequently passed to the renderPokedex function.

The renderPokedex function handles the creation of new DOM elements for each Pokemon. Event listeners are dynamically generated and linked to every Pokemon featured in the Pokedex list.

Upon a "click" event, a fetch request is dispatched to the PokeAPI for the specific character that was selected. This request retrieves all pertinent information about the chosen Pokemon, which is then displayed in the two boxes on the right-hand side.

Accurately determining the weight and height of each Pokemon presented a challenge, as the API's data was provided in decimeters and hectograms. Consequently, a conversion was necessary to express the weight in inches and pounds.

Lastly, when a selected Pokemon is added to the team using the "add to team" button, it will be visibly displayed in one of the boxes below. There are event listeners in place for both adding and removing Pokemon from the team. These listeners ensure a seamless transition, shifting all Pokemon to the left to prevent any empty spaces in the center.
