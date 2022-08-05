1. ### What happens when we call a function with new operator keyword?

    When we call a function with new operator keyword following thing happens:
        Step 1. New empty object({}) is created.
        Step 2. function is called, this points to new empty object created in step 1 i.e. this = {}.
        Step 3. This empty object({}) is linked to prototype
        Step 4. function automatically returns the empty object

```js
const Person = function (firstName, birthYear) {
    console.log(this);
};
console.log(new Person('Sidhant', 2000))

Person {}
Person {}
```