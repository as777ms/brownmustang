*In JavaScript, hoisting and scope are two fundamental concepts that govern how variables and functions behave in your code.*
#### In JavaScript, hoisting refers to the behavior of moving variable and function declarations to the top of their containing scope during the compilation phase. Here's a detailed breakdown of hoisting for different types of declarations and functions:
- [ ]1.var, let, and const declarations:
``` diff
+Hoisting: All var, let, and const declarations are hoisted to the top of their containing scope (global, function, or block scope).
+Initialization: However, the initialization of variables (assignment to a value) is not hoisted. The variables are accessible but uninitialized until their initialization code is executed.
+Temporal Dead Zone (TDZ): For let and const, there's a "temporal dead zone" between the declaration and initialization where the variables cannot be accessed. Accessing them in this zone results in a ReferenceError.
```
- [ ] 2.Function declarations:
``` bash
Hoisting: Function declarations are hoisted to the top of their containing scope.
Function expressions and arrow functions: These are not hoisted like function declarations. They are only hoisted if they are assigned to a variable or declared within a block scope.
```
  - [ ] 3.Immediately Invoked Function Expressions (IIFE):
> [!IMPORTANT]
> Hoisting: IIFEs are hoisted to the top of their containing scope, but they are executed immediately when the script is loaded, so they don't interfere with other code above them.
- [ ] 4.Scoping:
>~~Global scope~~: Variables and functions declared outside any function or block have global scope and are accessible from anywhere in your code.Local scope: Variables and functions declared inside a function or block have local scope and are only accessible within that function or block.Block scope: Introduced with let and const, block scope limits variable and function accessibility to the block they are declared in (e.g., loops, conditionals).


