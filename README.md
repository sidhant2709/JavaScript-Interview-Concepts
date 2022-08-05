# Object Oriented Programming
## Constructor Function and Prototypes :

```js
Here the comments // are browser console output
```

1. What happens when we call a function with new operator keyword?

    <h4>When we call a function with new operator keyword following thing happens:</h4>
    <ul>
        <li>Step 1. New empty object ({ }) is created.</li>
        <li>Step 2. function is called, this points to new empty object created in step 1 i.e. this = { }.</li>
        <li>Step 3. This empty object ({ }) is linked to prototype.</li>
        <li>Step 4. function automatically returns the empty object.</li>
    </ul>
    <br>

    ```js
    const Person = function (firstName, birthYear) {
        console.log(this); // Person {}
    };
    console.log(new Person('Sidhant', 2000)); //Person {}

    $ node file.js
    Person {}
    Person {}
    ```
2. Let's Play with the Constructor function Person

    ```js
    const Person = function (firstName, birthYear) {
        // ......code
    };

    console.log(Person); //f (firstName, birthYear) {}

    $ node file.js
    [Function: Person]
    ```
    ```js
    console.log(Person.prototype); //{constructor: f}

    $ node file.js
    Person {}
    ```




