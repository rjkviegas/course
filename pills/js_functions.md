# `function` in JavaScript

As you become familiar with JavaScript, you will see the `function` keyword used in ways that appear roughly equivalent to concepts in Ruby.

While it's convenient to use these analogies, they can lead to an inaccurate picture of how JavaScript really works.  As a language, JavaScript is fundamentally different to Ruby and understanding these differences will make you a better programmer.


The `function` keyword in JavaScript creates an object that can be **called**.  (We say _call_ in JavaScript, but that will make for confusing reading since 'call' has lots of meanings in English; let's use _invoke_ instead).

> In Ruby, we invoke (call) _methods_, not objects (a method belongs to an object).  But imagine that's just semantics.  Can you visualize a method as being just another object?  Perhaps it would help to think of it as an instance of a `Method` class or something similar?  Don't worry if you're only vaguely grasping this; you're already ahead of many JavaScript hobbyists!

## The anatomy of `function`
We've become familiar in Ruby with _literals_.  These are expressions that directly create a new object whenever they are evaluated:
```ruby
"Ben"  # creates a new String object
[]  # creates a new Array object
{}  # creates a new Hash object
```
The `function` keyword in JavaScript creates a new Function object (i.e. an object that can be invoked):
```javascript
var bark = function() {
  return 'Woof';
}

bark();  //invoking the function will return 'Woof'
```
You must include the parentheses when invoking a function, even if there are no arguments.  Can you reason why?  What is `bark;` on its own with no parentheses?

You can declare arguments in functions, as you would expect:
```javascript
var bark = function(name) {
  return name + ' says Woof';
}

bark('Barney');  //will return 'Barney says Woof'
```
> If you want to return a value from a JavaScript function, you must explicitly use `return`, otherwise it will just return `undefined`.


## `function` is like a block

In Ruby, we can pass a block to another method like so:
```ruby
['one', 'two', 'three'].each do |number|
  puts number
end
```
In JavaScript, we can do a very similar thing by passing an **anonymous function**.
> An **anonymous** function is a function without a name.

```javascript
['one', 'two', 'three'].forEach(function(number) {
  console.log(number);
});
```

But don't allow the syntax to confuse you; what are we actually passing to the `forEach` function?  It's just a Function object.  The following is exactly the same:
```javascript
var callback = function(arg) {
  console.log(arg);
};

['one', 'two', 'three'].forEach(callback);
```
> It's common to refer to this use of a function as a **callback**.


## Summary
It takes a while to understand JavaScript and the worst way to start is to try to force your understanding of Ruby onto it.  Once you are comfortable with the idea that a function is an object that can be invoked; and there are different ways to invoke a function, you are well on your way.

*Tip: in Sublime Text, you can type `proto` and hit Tab in a JS file to autocomplete the boilerplate code for defining a function on a prototype*


![Tracking pixel](https://githubanalytics.herokuapp.com/course/pills/js_functions.md)
