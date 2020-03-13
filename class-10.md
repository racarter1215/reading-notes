# Error Handling and Debugging

### Order of Execution is important to know so one can work backwards to see where errors exist.

##### Execution content: global content, function contenet, eval context. 

##### Variable scope: global scope, function-level scope.

##### The Stack: JS interprets one line of code at a time. When a statement needs data from another function, it STACKS (or piles) the new function on top of the current task.

##### page. 454 has a great view of this

##### Execution context and Hoisting: Each time a script enters a new execution context, there are two phases of activity:
###### 1.) Prepare and 2.) Execute.

##### Understanding Scope: In the Interpreter, each execution context has its own variables object.  It holds the variables, funcitons, and parameters available within it. Each execution context can also access its parent's variables object.

##### Functions in JS are said to have lexical scope. They are linked to the object they were defined within!!! So, for each execution context, the scope is the current execution context's variables object, PLUS the variables object for each parent execution context.

##### Understanding Errors: If JS generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.

##### Error objects: These can help you find where your mistakes are and browsers have tools to help you read them.

##### Types of errors: Syntax (syntax isn't correct), EvalError (incorrect use of eval() function), Reference Error (variable does not exist), URI Error (Incorrect use of uri functions), type error (value is unexpected data type), error (generic error), range error (number outside of range), NaN (not an error, basically if you do math without numbers, this happens).

##### How to deal with errors: Debug the script to fix erros, handle errors gracefully

##### Debugging Workflow: Where is the problem, what exactly is the problem

### Browser Dev tools and JS console

##### See oage 464-465


