Exercise 4: Fun with Handlebars

Do you know the game Cards Against Humanity? It's a game where players need to fill blanks in a sentence to make the funniest joke. For example, in the photo below:

cards against humanity

The resulting phrase reads as: Hope is a slippery slope that leads to a disappointing birthday party.

Inspired by the game you want to write a Node.js function that simulates playing the game. You'll do this with help of Handlebars.js, the templating engine we've been using to build this module's project.

Inside of this function you want to do several things:

    It needs to randomly select 2 words needs to fill in the blanks in the phrase _______ is great to ________ and print the result to the console.

Follow the steps:

    Install and require Handlebars. Note that it's just handlebars, not express-handlebars
    Create 2 functions, 1 called drawCard and 1 called getRandomWord
    The getRandomWord function returns a random array position from an array of 7 items. To get a random number between 0 and 6 use Math.floor(Math.random()*7)
    The drawCard function should first define a variable (called cardData), which contains an object with 2 keys: subject and punchline.
    Randomly assign to these keys values, taken from the following 2 arrays (make use of the getRandomWord function!):

For the key subject, select a random word from the following array:

const subjects = [
  'shark',
  'popcorn',
  'poison',
  'fork',
  'cherry',
  'toothbrush',
  'cannon',
];

For the key punchline, select a random word from the following array:

const punchlines = [
  'watch movie with',
  'spread some love',
  'put on cake',
  'clean toilets',
  'go to the moon',
  'achieve world piece',
  'help people learn programing',
];

    Create a variable, called card, that contains a template literal with the following: _______ is great to ________. Replace the ___ with the Handlebars placeholders
    Compile the card using the compile method
    Combine the compiled template with the cardData
    Log the result to the console!

Hints:

If you don't know how to use Handlebars, the documentation has a nice example!