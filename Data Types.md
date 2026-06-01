# Data Types

Data is information. Computers can understand many different kinds of information, and we refer to these different kinds as *data types*. In Godot, the four most common data types that we'll interact with are the following:

* float - A floating point number (numbers with decimal places)
* int - An integer. (whole numbers)
* String - A collection of characters (numbers, letters, symbols, etc)
* bool - A boolean value (true or false)

We will use these four data types in every project so it's good to memorize them. Let's go over how we'll see them in code.

## Floats

Floats can be expressed in two ways in GDScript: implicitly or explicity. Often, GDScript will *infer* the if we want an integer or float based on the operations we are performing on a value. However, this is not always the case. For times when we want to make sure a value is a float and not an int we can do this explicitly in one of two ways:

* Casting
* Explicit declaration

Casting involves converting one data type to another. For floats we can do this in code by using the float() function:

```
float(value_to_cast)
```

If we do not need to convert to a float but rather just need to declare a number is a float we can do so by adding a decimal place value (even if the value has a 0 in the decimal place)

```
2.0 #This value is a float!
```

## Integers

Integers can be expressed in the similar ways as floats. We can cast to an integer using the int() function:

```
int(value_to_cast)
```

We can also imply an integer by not adding a decimal place to a number.

```
2 #This value is an int!
```

## Strings

Strings are declared by surrounding characters in quoation marks:

```
"Hello World!" # This value is a String!
```

We can also cast to a string using the str() function

```
str(2) #This value was converted from an int to a String!
```

## Booleans

Bools can either be:

```
true
```
or
```
false
```

We can also cast other values to bools using the bool() function, though the results can be unpredictable.

```
bool(0) # This is false
bool(1) # This is true
bool(-1) # This is also true
```

# Now it's Your Turn!

Answer the following questions

1. What is the name of the data type for numeric values with decimal points
2. What is the name of the data type for whole numbers
3. How do you declare a string?
4. What is it called when you convert one data type into another?
5. Which data type only has two values?

