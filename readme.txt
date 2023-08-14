Difference between var and let:

Scope:
var: Function-scoped. This means that if you declare a variable using var inside a function, it's only available within that function. But if declared outside any function, it's globally scoped.
let: Block-scoped. It's confined to the block, statement, or expression where it's defined, such as within loops or conditionals.
Hoisting:
Both var and let declarations are hoisted to the top of their containing function or block, but with var, the variable is initialized with undefined. With let, the variable is not initialized, leading to a Reference Error if you try to use it before its declaration.
Re-declaration in the same scope:
var: You can re-declare the same variable multiple times.
let: You cannot re-declare the same variable in the same scope.
Difference between var and const:

Mutability:
var: Variables declared with var are mutable, meaning you can change their value after declaration.
const: Variables declared with const are immutable in the sense that you cannot reassign a new value to them. However, if it's an object, you can still modify its properties.
Other differences between var and const are similar to those between var and let (e.g., scope and hoisting).
Difference between let and const:

Mutability:
let: You can reassign a new value to a variable declared with let.
const: You cannot reassign a new value. But, if the variable is an object or array, you can modify its content (e.g., adding properties or items).
Scope and Hoisting: Both let and const share the same behavior in terms of scope and hoisting.
What is hoisting?

Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their containing scope during the compilation phase. This means that you can use a variable before it's declared in the code, and it will not result in an error. However, only the declarations are hoisted, not the initializations. This is why a variable declared with var will return undefined if accessed before its declaration, while a variable declared with let will throw a Reference Error in the same situation. Function expressions and arrow functions, when assigned to a variable, are not hoisted.
