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
 4. ```
      ( new Foo ).__proto__ === Foo.prototype
      ( new Foo ).prototype === undefined
    ```
