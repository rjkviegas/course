# Classes in JavaScript

The `class` keyword was introduced in ES6.


### Defining a class
In Ruby, we define and instantiate a class like this:
```ruby
class Dog

end

dog = Dog.new
```

In JavaScript, this looks like:
```javascript
class Dog {

}

var dog = new Dog();
```
Under the hood, JavaScript classes are actually types of functions. Try running `alert(typeof Dog);` The `class` syntax creates a function which is called `Dog`.


### Initialization code
In Ruby, we have an `initialize` method, which is called when a new object is created:
```ruby
class Dog
  def initialize(breed)
    @breed = breed
  end
end
```

In JavaScript, the `constructor` method is called.
```javascript
class Dog {
  constructor(breed) {
    this.breed = breed;
  }
}

var barney = new Dog('Pug');
```
> inside the function, `this` will be the newly created object.


## Defining methods

In Ruby, we define a method like so:
```ruby
class Dog
  def bark(name)
    "#{name} says Woof!"
  end
end
```

In Javascript, this would look like:
```javascript
class Dog {
  bark(name) {
    console.log(name + ' says Woof!');
  }
}
```
The `bark` method is stored in `Dog.prototype`. You can see this for yourself. Try running the following in the Web Console:
```javascript
var fido = new Dog();
console.log(fido);
```
By expanding the `Dog {}` that's returned, you can see that `bark` is found under the `__proto__`.

It's easy to think of `bark` as being a method of `Dog`.  But it isn't.  Objects in JavaScript are just bags of properties.  So `fido` is just a bag of properties, some of which it inherits from the prototype of `Dog`.


We can then call the `bark` method on any instance of `Dog` like so:
```javascript
fido = new Dog('Basset Hound');
fido.bark('Fido');
```


![Tracking pixel](https://githubanalytics.herokuapp.com/course/pills/js_classes.md)
