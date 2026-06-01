# Functions



Functions are powerful tools for organizing code (and many other things!). A function is a reusable block of code that can take inputs and either return an output or not. This allows for sectioning off blocks of code that you may use many times in your project, or for better maintainability. Let's look at the basics of a function.



## Anatomy of Functions



A function is made up of four components: a name, arguments, a return data type, and the body. We can tell the computer that we are declaring a new function by using the "func" keyword:



```

func

```



We then give the function a name, this can be anything we want but it is best to name it something that describes what the function does. For example, if we had a function that added two numbers together and returned the product we may call the function "add":



```

func add

```



We can then assign arguments to the function (though this is optional). An argument is a value that a user will pass into the function. Think of these as inputs:



```

func add(x, y)

```



Next, we can tell the computer if the function will return a value or not. We do this by providing the *data type* that the function should return. For our addition function we want to return a *float*. Note that we do this using the -> arrow operator. If we do not want to return a value we can use the "void" data type. We then end the function declaration with a colon (":")



```

func add(x, y) -> float:

```



Once we've finished the declaration we can tell the computer what *happens* when the function is called by including a body. This will be written at the 1-indent level.



```

func add(x, y) -> float:

	#The body of the function

```



We can reference the arguments (the user inputs) by using the argument name as a placeholder. We can also declare a *local* variable inside the function itself. Below we add both arguments together and store them in a new local variable named "sum".



```

func add(x, y) -> float:

	var sum = x + y

```



For this example we must return a value. We can do this by using the "return" keyword



```

func add(x, y) -> float:

	var sum = x + y

	return sum

```



Now let's give some examples of how this function might be used in code.



# Calling Functions



Whenever we use a function in code we will refer to it as "calling" the function. A function will always end with parentheses, and if the function takes arguments (inputs) we will put values in the parentheses. Our add function takes two arguments: x and y. Here's an example of calling the add function in the \_ready() function:



```

func _ready() -> void:

	add(1, 3) # Returns 4



```



Our add function *returns* a value, meaning that we can use that value later by storing it in a variable. Here's the same code modified to store the output.



```
func _ready() -> void:

	var result = add(1, 3) # Returns 4

```



We can then use the returned value. Here's an example where we use the returned value in another add function!



```

func _ready() -> void:

	var  result = add(1, 3) # Returns 4

	add(result, result) # Returns 8

```

You may have noticed that we can call a function inside of another function. This is a very common approach to organizing code. While our add function is short, imagine a function with 15 lines of code. By putting those 15 lines of code in a function we do not need to rewrite them every time we want to perform that specific calculation.

# Now You Try!

Answer the following questions as True or False:

1. A function can only be used once
2. A function is made up of a name, arguments, a return type, and body
3. A function can take zero arguments
4. Functions can be called from inside other functions
5. Functions cannot return data

Now, in a GDScript file do the following:

1. Create a function that takes two arguments. Make it subtract the *second* argument from the *first* and return the result as an integer.
2. Call the subtraction function in the _ready() function with the values 5 and 3 as the arguments. Store the result in a variable
3. Print the variable to the console using the print() function
4. Create another function that takes 3 arguments. Make it multiply the first two arguments together and then divide the product by the third argument and return the result as a float.
5. Call the multiply and divide function in the _ready() funciton with the values 2, 20, and 4 as arguments. Print the result to the console (you can do this without using a variable!)