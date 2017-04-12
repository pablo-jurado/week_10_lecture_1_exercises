1.A closure relies on what kind of scope to isolate variables?

***answer A. Lexical***

B. Block

C. Dynamic

D. Adjustable

---

2.Outer functions have access to the variables declared in nested functions. This statement is:

A. False

***answer B. True***

C. Sometimes true

D. Only false in strict mode

---

3.The statement "variable can share the same name when used in different function" refers to:

***answer A. Local scope***

B. Global scope

C. Both global and local scopes

---

4.In global scope, variables can:

***answer A. Be accessed and modified from any other scope.***

B. Be accessed and modified only from the global scope

C. Be accessed only from any other scope.

---

5.In a constructor invocation, this is the value of:

***answer A. The newly created object.***

B. The parent object.

C. The window.

---

6.this is the value of the first argument in:

A. .call(), .apply(), and .bind().

B. .call() and .apply().

C. .bind() and .call().

---

7.When using const, the value of a variable:

A. cannot be reassigned after assignment, unless the value is stored in an array or an object.

B. can always be reassigned after assignement.

***answer C. cannot be reassigned after assignment, ever.***

---

8.Function definition hoisting:

***answer A. Only occurs for function declarations.***

B. Only occurs for function expressions.

C. Occurs for function declaration and expressions.

---

9.In which mode will an error occur when a variable is assigned a value without first declaring the variable?

***answer A. Strict mode***

B. Non-strict mode

C. Both strict mode and non-strict mode

---

10.In variable hoisting, what gets hoisted to the top of the function?

A. Only the variable declaration

B. Only the variable assignment

***answer C. Both the variable declaration and assignment***

---

# short answer

#### (1) Describe a closure in JavaScript.
We use Closures to encapsulate data. We accomplish this nesting functions.
Our inner function will have access to the outer function's variables,
but we wont have access to those variables from the global scope.

#### (2) Returning an inner function does not call the function when the outer function is called. How can this be resolved?


#### (3) In the example below, why does the global variable get reassigned?
```
var reassignmentExample = "Global variable";

function testAssignment() {
  reassignmentExample = "Local variable";

  console.log(reassignmentExample);
}

console.log(reassignmentExample); // Logs: Global variable

testAssignment(); // Logs: Local variable

console.log(reassignmentExample); // Logs: Local variable (the global variable is reassigned)
```

#### (4) When would it be necessary to store the value of this in a variable?

#### (5) Describe the difference between function scoping and block scoping.

#### (6) In this example, why does logging 'hoistedVar' return 'undefined'?
```
function hoistingExample() {
  console.log(hoistedVar);
  var hoistedVar = "Hoist me!";
}
```
