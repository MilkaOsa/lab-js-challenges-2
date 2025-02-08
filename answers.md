Challenge 1

Answer: b) "xyz" and "xyz"

Explanation: The variable foo is declared globally. Inside the function bar(), foo is reassigned the value "xyz". Since foo is not redeclared inside bar(), it modifies the global foo. When bar() is called, console.log(foo); prints "xyz". The second console.log(foo); outside bar() also prints "xyz" since foo was modified globally.

Challenge 2

Answer: c) 10 and 1

Explanation: The function example(a) takes a as a parameter, creating a local scope variable a. Inside the function, a = 10; modifies the local a, but does not affect the global a. The first console.log(a); inside the function prints 10. Outside the function, console.log(a); prints 1 since the global a remains unchanged.

Challenge 3

Answer: c) "Hi there!"

Explanation: The function sayHi() is hoisted, meaning its declaration is moved to the top of the scope before execution. This allows the function to be called before its definition appears in the code. Thus, sayHi(); executes without error and prints "Hi there!".

Challenge 4

Answer: c) { num: 90 }

Explanation: The object a is assigned to b, meaning both variables reference the same object in memory. Modifying b.num = 90; also changes a.num since they refer to the same object. Note: The const keyword prevents reassignment of a, but it does not prevent modifying properties of the object.

Bonus: Challenge 5

Answer: c) { name: "Bob", age: 10 } and { name: "Ada", age: 20 }

Explanation: The function magicHat(obj) first modifies obj.age = 10;, which mutates the original object (rabbit1). However, the line obj = { name: "Ada", age: 20 }; creates a new object, and rabbit2 now references this new object. rabbit1 remains modified with age: 10, but keeps its original name "Bob". rabbit2 is a new object with { name: "Ada", age: 20 }.