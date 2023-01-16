# note-ES6-JavaScript
JavaScript: Understanding ES6 and Beyond
## Block Scoping
1. lexical environment, curly brace
   - var, global
   - let, in the same block or block going up
   - const, similar to let, but the binding is immutable
## Templates
1. concatenation
   - string + string
2. interpolation
   - replace portions of strings with other strings. It described as inserting or injecting strings into another strings
   - dollar sign and curing brace within string
   - ```
      let firstname = Steven;
      let lastname = Jie;
      let fullname = `${firstname} ${lastname}`
     ```
 ## Classes
 1. a structure in a programming language that provides a way to create objects
 2. class, function object
 3. instance, the actual object created from an object creation feature(like a class)
 4. how to understand ```__proto__``` and prototype?
    - everything in JavaScript can be considered as object, any object has property ```__proto__```
    - ```__proto__``` comes from the prototype of constructor
      ```
      ( new Foo ).__proto__ === Foo.prototype
      ```
    - object ( new Foo )'s ```__proto__``` comes from the prototype of Foo constructor
    - JavaScript has a built-in constructor called Object(), and the prototype property of this function points to an empty object
    - thus, we can say
      ```
      ( new Foo ).__proto__.__proto__ === Object.prototype
      ```
      it is true
    - and 
      ```
      ( new Foo ).__proto__.__proto__.__proto__ === null
      ```
      it is true
    - if there is inheritence in it, it would be more fun, assume that Staff extends to Person,
      ```
      let a = new Person('Rick')
      let b = new Staff('Steve')
      ```
      thus, 
      ```
      b.__proto__ === Staff.prototype
      b.__proto__.__proto__ === Person.prototype
      b.__proto__.__proto__.__proto__ === Object.prototype
      b.__proto__.__proto__.__proto__.__proto__ === null
      ```
      there are all true!
  5. 
    
