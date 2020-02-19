# Objects

You can think of object as containers for data. It can have multiple kinds of data - strings, integers, booleans, functions, arrays, etc. One of the powerful features of an object - that you can't do with an array - is to label the data inside the container.

For example, the number `1` has no meaning in an application by itself. You have no idea what that integer represents until assign it a name. On objects, those are called keys.

```js
/*
    Basic object representing my friend Angus.
    - The object itself is labeled with the variable of `angus`
    - The integer of 50 is labeled with the key of `age`
*/
const angus = {
    age: 50
}

// Another object representing his brother Malcom
const malcom = {
    age: 53
}
```

Now the number 50 and 53 have meaning, or *context*, when assigned to a key on these objects.

> Everything in JavaScript is an object and *objects* are the basis of *Object Oriented Programming (OOP)*

### What does an Object Literal Look Like?

Until you get to more advanced JavaScript, you can recognize an object literal because it follows this pattern.

* Curly braces surround the properties of an object literal
* The *properties* are the key/value pairs separated by a colon
* Properties of the object are separated by a comma

An example of an 'album' object literal:

```js
const album = {
    name: "The Battle of Los Angeles",
    release_date: 1999,
    band: "Rage Against the Machine"
}
```

> ADD IMAGE LABELED KEY/VALUES

The same data stored as below is not an object.

```js
const food = ["The Battle of Los Angeles", "1999", "Rage Against the Machine"]
```
The array above doesn't represent a singular thing. It also has no curly braces, or key/value pairs. When using an array to store these strings, they have now lost their *context*.

### How are Objects Different from Arrays?

Arrays are collections of similiar *things*. Objects are ways to define details of a *single* thing. Both an array and an object can be assigned to a variable.

Here you define two separate objects. One represents a cat, and the other represents a dog. Each has their own properties _(key/value pairs)_ separated by commas.

```js
const cat_dog = {
    species: "Cat",
    name: "Cat Dog",
    age: 4,
    color: "Calico"
}

const elvis = {
    species: "Dog",
    name: "Elvis",
    age: 11,
    color: "Brown"
}
```

Developers never describe two things with a single object.

```js
// DON'T do this
const theAnimals = {
    catName: "Jingles",
    catAge: 4,
    catColor: "Black",
    dogName: "Denver",
    dogAge: 7,
    dogColor: "Brown"
}
```

If you want to store both animals inside of a single data structure, use an array. 

```js
// This array is a collection of animals
const animals = [cat, dog]
```

### Object Practice

> **Exercise 1:** Given two options of data structures - array or object - which should you use? You need to represent a red 2015 Ford Mustang in your code.

> **Exercise 2:** Given two options of data structures - array or object - which should you use? You need to store list of animal names in a shelter. The names are "Kippers", "Jack", "Gypsy", "Angus", "Seymour Bouts", and "Sharky".

> **Exercise 3:** Define an object for four family members, and put each object in an array named `familyMembers`. Each family member object that you create should have the same keys on them, but the values will be different.

### Setting and Accessing Values on Objects

There are two ways to access the values stored inside of an object. One is called dot notation, and the other is square bracket notation.

#### Dot Notation

To obtain the value inside an object, and you know the name of the key, you can use dot notation. Here's the pattern.

```js
variableContainingTheObject.keyName
```

Given the following object...

```js
const lassie = {
    age: 7,
    breed: "Collie",
    color: "White and Brown"
}
```

To output the string "Collie" to the console, you would use the following code.

```js
console.log(`Lassie's breed is ${lassie.breed}`)
```

To output the integer 7 to the console, you would use the following code.

```js
console.log(`Lassie's age is ${lassie.age}`)
```

> **Practice:** Given the object below, output each of the values to the console using dot notation.

```js
const wardrobe = {
    height: 80,
    manufacturer: "Killibrew & Sons",
    contents: ["Dress shirt", "Jeans", "Suit", "Skirt", "Tennis shoes"],
    depth: 38,
    width: 50
}
```

You can also use dot notation to create a new key on an object if you need to.

```js
wardrobe.material = "Cedar"
```

You just added a new key to the object stored in the `wardrobe` variable. If you output it to the console, you will see it along with the others that were already defined.

```js
console.log(wardrobe)

> contents: (5) ["Dress shirt", "Jeans", "Suit", "Skirt", "Tennis shoes"]
depth: 38
height: 80
manufacturer: "Killibrew & Sons"
material: "Cedar"
width: 50
```

#### Square Bracket Notation

Square bracket notation is most often used when the key name is stored in a variable. The basic mechanics of it are similar to dot notation, you just use square brackets with the key name inside.

Above you saw how to access the `breed` key on the object below with dot notation.

```js
const lassie = {
    age: 7,
    breed: "Collie",
    color: "White and Brown"
}
```

Using square bracket notation, here's the syntax.

```js
// Square bracket notation for key access
lassie["breed"]
> "Collie"

// Dot notation for key access
lassie.breed
> "Collie"
```

That's the basics, but you need to see how square is actually used in an application. Here's what it looks like when using a variable to look up a key on an object.

```js
// Breed is the key you want to get the value of in the object below
const keyToLookup = "breed"

// First, make JavaScript evaluate the variable and give us its value
console.log(keyToLookup)
> "breed"
```

Now that you know that `keyToLookup` evaluates to `"breed"`, you can use the variable to lookup the value with square bracket notation.

```js
const lassie = {
    age: 7,
    breed: "Collie",
    color: "White and Brown"
}

// Use the value of `keyToLookup` to get the value you want
const lassiesBreed = lassie[keyToLookup]
> "Collie"
```

> **Instructor Note:** Talk about how expressions get evaluated from right to left, instead of the other way.

#### Practice

Time to practice dot and square-bracket notation. Use the following object to complete the exercises below.

```js
const empireStateBuilding = {
    stories: 103,
    height: 1453,
    address: "350 Fifth Avenue, Manhattan, New York 10118",
    squareFeet: 2768591,
    constructionDate: 1931,
    cost: 40948900,
    owner: "Empire State Realty Trust",
    eastWestLength: 424,
    northSouthLength: 187,
    architect: "Shreve, Lamb & Harmon"
}
```

> **Exercise 1:** Use dot notation to output all of the dimensions of the Empire State Building to the console.

> **Exercises 2:** Use square bracket notation to output the remaining 5 properties to the console. Create 5 variables first with the keys as their values. Use those variables to look up the values.

### Arrays as Object Properties

So far, you've been largely accessing string and integer values in an object. However, values can be anything in the JavaScript language - including arrays. Consider this example.

```js
const kennel = {
    name: "Sunny Meadows Safe Haven-Pets",
    address: "4066 New Getwell Rd,",
    capacity: 50,
    currentAnimals: ["Jet", "Snickers", "Blue", "Jacks", "Flap", "Barnum"]
}
```

If you want to display all of the animals that are currently being boarded, you first have to access the array. You can use *dot* notation to get that value.

```js
const boardedAnimals = kennel.currentAnimals

for (let i = 0; i < boardedAnimals.length; i++) {
    console.log(boardedAnimals[i])
}

> "Jet"
> "Snickers"
> "Blue"
> "Jacks"
> "Flap"
> "Barnum"
```

If you wanted to pull a single animal form the array, and display it, you can use the index value. To show the fourth animals in that array, you would use the following code.

```js
console.log(kennel.currentAnimals[3])

> "Jacks"
```

#### Practice

Examine the object below.

```js
const code_school = {
    founded: 2018,
    director: "Meka",
    instructors: {
        fullTime: ["Autumn", "Kenn", "Kevin"],
        partTime: ["PJ", "Thomas"]
    },
    address: "80 Union Ave."
}
```
## Practice:

> **Exercise 1:** Output the names of the part-time instructors followed by the names of the full-time instructors in the console.

> **Exercise 2:** Output only Autumn and Thomas in the console.

### Practice: Accessing Property Values

Given the following object...

```js
const beatles = {
    albums: ["Abbey Road", "Sgt Peppers Lonely Heart's Club Band", "Revolver", "Magical Mystery Tour", "Something New"],
    history: {
        formed: 1960,
        disbanded: 1970
    },
    members: [
        {
            name: "George Harrison",
            birth: 1943,
            death: 2001
        },
        {
            name: "Paul McCartney",
            birth: 1942,
            death: null
        },
        {
            name: "John Lennon",
            birth: 1940,
            death: 1980
        },
        {
            name: "Ringo Starr",
            birth: 1940,
            death: null
        }
    ]
}
```

Output the following value to the console.

```text
Paul McCartney was in the Beatles from 1960 to 1970. He was born in 1942. He contributed heavily to the Magical Myster Tour Album.
```

## Additional Information
- [Variables vs. Arrays vs. Objects video](https://www.youtube.com/watch?v=FjSCdXd04Cs)