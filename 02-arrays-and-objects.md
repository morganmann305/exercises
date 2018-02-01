# 02 Arrays & Objects

Open your JavaScript Console in Google Chrome and enter the following examples. If your console becomes too cluttered with commands or errors, remember you can type `clear()` for a fresh start.

Type in the command as it is next to the number, then go through the modifications below.

You may want to write down your findings during this exploration for future reference.

If a solution or answer to a question eludes you, ask!

---

## Arrays

1. Create a variable called `fruit` to store an array. Use an array literal to build an array of the following strings: apple, banana, clementine.

   Use bracket notation to call each of these items individually in the console.

2. Create a variable called `vegetables` to store a new array. Use an array constructor to build an array of the following strings: asparagus, broccoli, carrot.

  Use bracket notation to call each of these items individually in the console.

3. Enter the following into the console: `var number = parseInt(Math.random() * 100);` DO NOT peek at what `number` contains! (If you cheat, re-enter the statement.)

  Create a variable called `emptyArray` to store a new array. Using an array constructor, pass in `number` as the value to create an empty array with the unknown number of spaces.

  What **array property** can you use to determine how big the array is?  (Think you are correct? *Now* you may look at the value contained in number.)


## Objects

Enter the following object (do not copy-paste; type it in so you become familiar with building an object!):

```javascript
var flynn = {
  species: "cat",
  paws: 4,
  colors: ["black", "brown", "gray", "white"],
  shy: false,
  cuddly: true,
}
```
1. Using bracket notation, add the following properties:
  - `favoriteCatNipStrain` with a value of `Bastet Mau`
  - `favoriteToy` with a value of `Mr. Fish`
2. Using dot notation, add the following properties:
  - `pickyEater` with a value of `false`
  - `born` with a value of `2011`
3. Using either bracket or dot notation (maybe mix it up)? Return a value which answers the following questions:
  - What species is Flynn?
  - Is Flynn shy?
  - What is Flynn's favorite strain of cat nip?
  - What colors are in Flynn's coat? (List each individually... or produce a comma-delimited string.)
  - What type of value is stored in the property `paws`?
  - What type of value is stored in the property `colors`?
  - What type of value is stored in the property `cuddly`?


## Array Methods

The next two sections will be *significantly* easier if you use the template(s) contained within the [`web-template`](https://github.com/umiami-js/web-template) repo.

Clone the repo from GitHub. Copy the `array.js` and `objects.js` files to the `js` folder. Use the `script.html` file. Include the `array.js` and `objects.js` files using the script tag. You may erase the contents of `js/example.js` and write your code within that file.

Do not modify the contents of `js/array.js`.

1. `console.log(numbers);`

  Use a method to determine how many numbers are in this array.

  Add the following line to your code:

  `var splicedArray = numbers.splice(27, 7);`

  How long is the `numbers` array now?

  What is the last number in the `numbers` array?

  What numbers are in `splicedArray`?

2. Store a new array in the variable `moreNumbers`. You may use either an array literal or an array constructor. The items in the array should be as follows.

  `5, 7, 6, 8, 2, 1, 6, 8, 9, 0`

  Use the `concat` method to add the `moreNumbers` array to the `numbers` array. Store the result in a new variable (`newNumbersArray`) as `concat` does not permanently modify the original array.

  Add the following line to your code:

  `newNumbersArray.reverse();`

  How long is the `newNumbersArray` array?

  What is the index of the first appearance of the number 5?  

  What is the index of the last appearance of the number 5?

3. Create a new array stored in the variable `topPets`.

  Add the following using bracket notation: `fish, cat, dog, elephant`.

  Add the following using the `push` method: `giraffe, alligator, bat, hippo`.

  Use `console.log` to display the contents of `topPets` to see your array is complete and correct.

4. `console.log(veggies);`

  Use two methods to transform the array so its order becomes:

  `eggplant, carrot, banana, apple`

  Use `console.log` to display the contents of `veggies`.

5. `console.log(message);`

  Use a method to turn the contents of this array into a string. Store the result in a variable, `newMessage`.

  Use the `typeof` keyword to prove `newMessage` is a string.

6. `console.log(threeNumbers)`

   `console.log(threeMoreNumbers)`

   Use a single method to combine these arrays into a single array and to produce the order: `1, 2, 3, 4, 5, 6`.


### More Objects

Use `objects.js` to store your data. Open the file `pixar-movies.txt` stored in the `03-arrays-and-objects` directory. You will be transforming this file into a data structure which can be referred to using JavaScript. You will later query this object to answer questions.

Be sure you use the correct data type for each property value! Do not forget to include a title among each film's properties.

**HINT:** For the Steps 2 and 3, you will need to create a new object for a film, fill in the data, *then* add the object to `pixarMovies`. Set your new property in `pixarMovies` equal to the object you created.

Example: `pixarMovies["movieTitle"] = movieTitle;`

1. An object `pixarMovies` has already been created and contains two more objects, `toyStory` and `aBugsLife`. Fill in the data for these films.

2. Build out the next two films in the list using bracket notation.

3. Build out the last two films in the list using dot notation.

4. Use the object you have built to answer the following questions using the console. You may use bracket or dot notation to return the correct values from `pixarMovies`.

For example: Did 'A Bugs Life' win an Oscar? `pixarMovies.aBugsLife.award;`

  - What is the Rotten Tomatoes rating for 'Monsters Inc.'?
  - What is 'Cars' about?
  - Who starred in 'The Incredibles'?
  - Who was the supporting actor in 'A Bugs Life'?
  - Which movies won Oscars? (three answers)
  - Which film has the most stars?  How many?
  - Which movies have Rotten Tomatoes ratings over 98? (two answers)
