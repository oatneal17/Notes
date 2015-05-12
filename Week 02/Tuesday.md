# JS Day 2

#### Type Coercion

When comparing values in Javascript using the double equals `==`, it will implictly convert the types and then compare the values only. So the values `Number(5)` and `String("5")` would be consider equal.

When comparing values in Javascript using the triple equals `===` it will not implicitly convert the types, if the values are of differnt types they will not be considered equal.

Implicit type coercion can lead to bugs so always use the triple equals `===` when comparing values.


#### Functions

functions are mini programs inside the the main program that can be invoked at any time.

The syntax to declare a function is:

```javascript
function doSomething() {
  // do stuff...
}
```

The syntax to invoke a function is:

```javascript
doSomething();
```

when invoking these sub programs we call functions you can pass data in and get data back out.

To pass data in, you use parameters:

```javascript
function doSomething(parameter1, parameter2) {
  // do stuff...
}

doSomething("foo", 5);
```

To get data back, the function must `return` a value:

```javascript
function doSomething() {
  // do stuff...
  return 5;
}

var response = doSomthing();
```


#### The Math Object

* __Math.PI__ evaluates to 3.141592653589793
* __Math.round__ rounds a number
* __Math.ceil__ always rounds a number up
* __Math.floor__ always rounds a number down
* __Math.random__ return a random decimal between 0 and 1


#### DOM

The _Document Object Model_ is the Javascript interface provided by the broweser to programmatically interact with the HTML on the webpage.


#### Dom Manipulation

__Document.querySelector__

Allows you to select DOM elements to manipulate or get data from. The elements can be selected the same was css selectors work. for example `document.querySelector(".foo")` will select the first element with the css class "foo".

Once you have selected a DOM element, there are several methods and properties that can be used on them, some of which are:

* `textContent` get the text from the element
* `getAttribute` get the value for a specific attribute


#### Resources

* [Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
* [Math](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math)
* [DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
* [Document.querySelector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)
* [Equality comparisons and sameness](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness)
