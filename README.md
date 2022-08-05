1. ### What happens when we call a function with new operator keyword?

    <h4>When we call a function with new operator keyword following thing happens:</h4>
    <ul>
        <li>Step 1. New empty object({}) is created.</li>
        <li>Step 2. function is called, this points to new empty object created in step 1 i.e. this = {}.</li>
        <li>Step 3. This empty object({}) is linked to prototype</li>
        <li>Step 4. function automatically returns the empty object</li>
    </ul>
```js
const Person = function (firstName, birthYear) {
    console.log(this);
};
console.log(new Person('Sidhant', 2000));
```
<details><summary>Terminal</summary>
<p>
```
```
    $ node file.js
    Person {}
    Person {}
```
```
</p>
</details>

