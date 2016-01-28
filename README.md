
#Objects
After the Lesson you'll be able to understand:
+ What is an object
+ object notation
+ key:value pairs
+ differences between arrays and objects


JavaScript is an object oriented programming language. Everything can be described by objects, which bundle properties, with methods or actions, and events that impact those objects.


An object is a list of associated data pairs. Unlike arrays, objects do not have numbered indexes. Instead they contain key names and associated values. Where a numbered grocery list is a good metaphor for an array, a birthday list including a person’s name (key) and their birthday date(value) would be a better metaphor for an object.

```
> var birthdays = { "Homer" : "August", "Marge": "October"}
```


It's like a list of pairs of things; or a list of stickers, each of which is stuck to something else. The syntax is different, too.

```
> var fruitColors = { "apple" : "red", "tangerine": "orange", "banana": "yellow"}
```

Each sticker/object pair, also called a key/value pair in computer science, is separated from the next by a comma.
`apple` is the key, and the associated value is `red`

And instead of looking up individual values with an index, we now can use the keys, or stickers.
```
> fruitColors["apple"]
You will get an error if you ask for something that doesn't exist.
> fruitColors["pear"]
```
Javascript also allows you to access the values by using a dot, similar to how you call a method. Try this:
```
> fruitColors.apple
```

You can also reassign values. 

`fruitColors["apple"] = "green"`

Finally, you can use Object.keys() to list all of the keys in an object.
`Object.keys(fruitColors)`

## Student Practice
Create an object called favorites which has keys: book, ice cream flavor, city, and color.

Then use concatenation to make a string that lists all of your favorite items. For example "My favorite things are Lord of the Rings, mint chocolate chip, Chicago and the color green."

You will need to use the bracket or . syntax to access each value. 




## Stretch Example
Let's explore Javascript objects using a real life object.

In real life, a person is an object. A person has **properties** like firstName, surname, age, and gender. A person's ability to express her thoughts can be defined as a **method** _talk_.

Object  | Property Name        | Propery Value                    | Method |
------------------|-------------------------------------|-------------|
person | firstName                | person.firstName = "Jane" |
            | surname                 | person.surname = "Doe"    |
            | age                         | person.age = 24                 |
            | gender                    | person.gender = "Female" |
            |                                |                                            | person.talk();


Using this representation of person, every person will have the same property names (firstName, surname, age, and gender) **BUT** different property values. Each person object would also inherit the **same method** _talk_.

To fill out the profile of our `person object` to match the information in the object table above:
      
```javascript
var person = {
        firstName: "Jane",
        surname: "Doe",
        age: 24,
        gender: "Female",
        talk: function(){console.log('Hello')}}
```

### Challenge
Make a new object called dog, with properites: name, breed, size, and function, bark.
# References
[Site Point JS Objects](http://www.sitepoint.com/back-to-basics-javascript-object-syntax/)

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/cssi-2.8-js-objects' title='Objects'>Objects</a> on Learn.co and start learning to code for free.</p>
