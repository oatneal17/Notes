# Functions
A function is a group of statements that can be called multiple times, and can be stored in a variable or passed around.

To put it another way: A function is an object that contains JavaScript code that is run when I call the function.

## Function declaration
A function declaration is a complete statement that can stand on its own. It creates a function with the name you specify.

```js
function coolFunction(thing) {
  alert(thing);
}
```

## Function expression
A function expression cannot stand on its own, but we can assign it to a variable or pass it to another function.

```js
var aFunction = function(thing) {
  alert(thing);
}

document.getElementById(id).addEventListener('click', function(){
  alert("Hay");
});
```


## Sass

#### Installing Sass

Documentation - http://sass-lang.com/

[Node Sass](https://github.com/sass/node-sass)

```sh
$ npm install -g node-sass
$ node-sass -v
```

## Sass Demo

#### Processing Sass

```sh
# Compile once
$ node-sass <input.scss> <output.css>

# Or Watch your files
$ node-sass -w <input.scss> <output.css>
```

#### Variables (like JS Variables)
```css
$font-stack:    Helvetica, sans-serif;
$primary-color: #333;

body {
  font: 100% $font-stack;
  color: $primary-color;
}
```

#### Nesting

```css
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { display: inline-block; }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```

#### Partials & Imports

`_reset.scss` - Normalize?

```css
@import 'reset';

body {
  font-size: 100% Helvetica, sans-serif;
  background-color: #efefef;
}
```

#### Lighten / Darken

```css
$green: rgba(98,178,70,1);
a {
  color: $green;
}

a:hover {
  color: lighten($green, 20%);
}
```

#### Mixins (like JS Functions)

```css
@mixin border-radius($radius) {
  border-radius: $radius;
}

.box { @include border-radius(10px); }
```

#### Operators

```css
.container { width: 100%; }

article[role="main"] {
  float: left;
  width: 600px / 960px * 100%;
}

aside[role="complimentary"] {
  float: right;
  width: 300px / 960px * 100%;
}
```
