# Javascript-Variable-Declarers

1. `var`:

Variables that are declared with the `var` keyword can be accessed in any scope of the file. 

* Variables declared with `var` can be redeclared

* Variables defined with `var` must be declared before use

* Variables defined with `var` are not limited to a block or function scope

* Variables defined with `var` can be reassigned.

```
var name = "Pontsho";

console.log(name);
/// Will print out:
Pontsho

var name = "Themba";

console.log(name);
/// Will print out:
Themba
```

```
var name = "Thando";

function sayName() {
  console.log(`My name called in the function scope is ${name}`);
  {
    console.log(`My name called in the scope nested within the function scope is ${name}`);
  }
}

sayName();
/// Will Print out:
My name called in the function scope is Thando
My name called in the scope nested within the function scope is Thando
```
2. `let`:

Variables that are declared with the `let` keyword are limited within the scope that they are declared in.

* Variables declared with `let` can not be redeclared

* Variables defined with `let` must be declared before use

* Variables defined with `let` are limited to a block or function scope

* Variables defined with `let` can be reassigned.

```
let name = "Pontsho";

let name = "Themba";

///The interpreter will raise an error alerting that you cannot redeclare a block-scoped variable
```

```
let name = "Pontsho";

console.log(name);
/// Will print out:
Pontsho

name = "Themba";

console.log(name);
/// Will print out:
Themba
```
3. `const`:

Variables that are declared with the `const` keyword are limited within 

* Variables declared with `const` can not be redeclared

* Variables defined with `const` must be declared before use

* Variables defined with `const` are limited to a block or function scope

* Variables defined with `const` can not be reassigned.
