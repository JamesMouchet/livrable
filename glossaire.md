# Glossaire PHP de James


## PHP echo and print Statements

```
echo and print are more or less the same. They are both used to output data to the screen.

The differences are small: echo has no return value while print has a return value of 1 so it can be used in expressions. echo can take multiple parameters (although such usage is rare) while print can take one argument. echo is marginally faster than print.

The echo statement can be used with or without parentheses: echo or echo().
The print statement can be used with or without parentheses: print or print().
```

## PHP Data Types

```
Variables can store data of different types, and different data types can do different things.

PHP supports the following data types:

String
Integer
Float (floating point numbers - also called double)
Boolean
Array
Object
NULL

```

```
PHP String
A string is a sequence of characters, like "Hello world!".

A string can be any text inside quotes. You can use single or double quotes
```

```
PHP Integer
An integer data type is a non-decimal number between -2,147,483,648 and 2,147,483,647.

Rules for integers:

An integer must have at least one digit
An integer must not have a decimal point
An integer can be either positive or negative
Integers can be specified in three formats: decimal (10-based), hexadecimal (16-based - prefixed with 0x) or octal (8-based - prefixed with 0)
```

```
PHP Float
A float (floating point number) is a number with a decimal point or a number in exponential form.
```

```
PHP Boolean
A Boolean represents two possible states: TRUE or FALSE.
```

```
PHP Array
An array stores multiple values in one single variable.

In the following example $cars is an array. The PHP var_dump() function returns the data type and value
```

```
PHP Object
An object is a data type which stores data and information on how to process that data.

In PHP, an object must be explicitly declared.

First we must declare a class of object. For this, we use the class keyword. A class is a structure that can contain properties and methods
```

```
PHP NULL Value
Null is a special data type which can have only one value: NULL.

A variable of data type NULL is a variable that has no value assigned to it.

Tip: If a variable is created without a value, it is automatically assigned a value of NULL.

Variables can also be emptied by setting the value to NULL
```

## PHP String Functions
```
Get The Length of a String
The PHP strlen() function returns the length of a string.
```

```
Count The Number of Words in a String
The PHP str_word_count() function counts the number of words in a string
```

```
Search For a Specific Text Within a String
The PHP strpos() function searches for a specific text within a string.

If a match is found, the function returns the character position of the first match. If no match is found, it will return FALSE.
```

## PHP Operators

```
PHP Arithmetic Operators

+	Addition	$x + $y	Sum of $x and $y
-	Subtraction	$x - $y	Difference of $x and $y
*	Multiplication	$x * $y	Product of $x and $y
/	Division	$x / $y	Quotient of $x and $y
%	Modulus	$x % $y	Remainder of $x divided by $y
**	Exponentiation	$x ** $y	Result of raising $x to the $y'th power (Introduced in PHP 5.6)
```

```
PHP Assignment Operators

x = y	x = y	The left operand gets set to the value of the expression on the right
x += y	x = x + y	Addition	Show it »
x -= y	x = x - y	Subtraction	Show it »
x *= y	x = x * y	Multiplication	Show it »
x /= y	x = x / y	Division	Show it »
x %= y	x = x % y	Modulus
```

```
PHP Comparison Operators

==	Equal	$x == $y	Returns true if $x is equal to $y
===	Identical	$x === $y	Returns true if $x is equal to $y, and they are of the same type
!=	Not equal	$x != $y	Returns true if $x is not equal to $y
<>	Not equal	$x <> $y	Returns true if $x is not equal to $y
!==	Not identical	$x !== $y	Returns true if $x is not equal to $y, or they are not of the same type
>	Greater than	$x > $y	Returns true if $x is greater than $y
<	Less than	$x < $y	Returns true if $x is less than $y
>=	Greater than or equal to	$x >= $y	Returns true if $x is greater than or equal to $y
<=	Less than or equal to	$x <= $y	Returns true if $x is less than or equal to $y
```

```
PHP Increment / Decrement Operators

++$x	Pre-increment	Increments $x by one, then returns $x
$x++	Post-increment	Returns $x, then increments $x by one
--$x	Pre-decrement	Decrements $x by one, then returns $x
$x--	Post-decrement	Returns $x, then decrements $x by one
```

```
PHP Logical Operators

and	And	$x and $y	True if both $x and $y are true
or	Or	$x or $y	True if either $x or $y is true
xor	Xor	$x xor $y	True if either $x or $y is true, but not both
&&	And	$x && $y	True if both $x and $y are true
||	Or	$x || $y	True if either $x or $y is true
!	Not	!$x	True if $x is not true
```

```
PHP String Operators

.	Concatenation	$txt1 . $txt2	Concatenation of $txt1 and $txt2
.=	Concatenation assignment	$txt1 .= $txt2	Appends $txt2 to $txt1
```

```
PHP Array Operators

+	Union	$x + $y	Union of $x and $y
==	Equality	$x == $y	Returns true if $x and $y have the same key/value pairs
===	Identity	$x === $y	Returns true if $x and $y have the same key/value pairs in the same order and of the same types
!=	Inequality	$x != $y	Returns true if $x is not equal to $y
<>	Inequality	$x <> $y	Returns true if $x is not equal to $y
!==	Non-identity	$x !== $y	Returns true if $x is not identical to $y
```

## PHP if...else...elseif Statements

```
PHP - The if Statement
The if statement executes some code if one condition is true.
```

```
PHP - The if...else Statement
The if....else statement executes some code if a condition is true and another code if that condition is false.
```

```
PHP - The if...elseif....else Statement
The if....elseif...else statement executes different codes for more than two conditions.
```

## Switch

```
The PHP switch Statement
Use the switch statement to select one of many blocks of code to be executed.

switch (n) {
    case label1:
        code to be executed if n=label1;
        break;
    case label2:
        code to be executed if n=label2;
        break;
    case label3:
        code to be executed if n=label3;
        break;
    ...
    default:
        code to be executed if n is different from all labels;
}
```

## PHP Loops

```
The PHP while Loop
The while loop executes a block of code as long as the specified condition is true.

while (condition is true) {
    code to be executed;
}
```

```
The PHP do...while Loop
he do...while loop will always execute the block of code once, it will then check the condition, and repeat the loop while the specified condition is true.

do {
    code to be executed;
} while (condition is true);
```

```
The PHP for Loop
The for loop is used when you know in advance how many times the script should run.

for (init counter; test counter; increment counter) {
    code to be executed;
}
```

```
The PHP foreach Loop
The foreach loop works only on arrays, and is used to loop through each key/value pair in an array.

foreach ($array as $value) {
    code to be executed;
}
```

## PHP Arrays

```
An array stores multiple values in one single variable:

<?php
$cars = array("Volvo", "BMW", "Toyota");
echo "I like " . $cars[0] . ", " . $cars[1] . " and " . $cars[2] . ".";
?>
```

```
PHP Indexed Arrays
There are two ways to create indexed arrays:

The index can be assigned automatically (index always starts at 0), like this:

$cars = array("Volvo", "BMW", "Toyota");
or the index can be assigned manually:

$cars[0] = "Volvo";
$cars[1] = "BMW";
$cars[2] = "Toyota";
```

```
Get The Length of an Array - The count() Function
The count() function is used to return the length (the number of elements) of an array
```

```
PHP Associative Arrays
Associative arrays are arrays that use named keys that you assign to them.

There are two ways to create an associative array: 

$age = array("Peter"=>"35", "Ben"=>"37", "Joe"=>"43");
or:

$age['Peter'] = "35";
$age['Ben'] = "37";
$age['Joe'] = "43";
```

## PHP Functions

```
PHP User Defined Functions
Besides the built-in PHP functions, we can create our own functions.

A function is a block of statements that can be used repeatedly in a program.

A function will not execute immediately when a page loads.

A function will be executed by a call to the function.
```

```
Create a User Defined Function in PHP
A user defined function declaration starts with the word "function":

Syntax
function functionName() {
    code to be executed;
}
Note: A function name can start with a letter or underscore (not a number).

Tip: Give the function a name that reflects what the function does!
In the example below, we create a function named "writeMsg()". The opening curly brace ( { ) indicates the beginning of the function code and the closing curly brace ( } ) indicates the end of the function. The function outputs "Hello world!". To call the function, just write its name:

<?php
function writeMsg() {
    echo "Hello world!";
}

writeMsg(); // call the function
?>
```

```
PHP Function Arguments
Information can be passed to functions through arguments. An argument is just like a variable.

Arguments are specified after the function name, inside the parentheses. You can add as many arguments as you want, just separate them with a comma.

The following example has a function with one argument ($fname). When the familyName() function is called, we also pass along a name (e.g. Jani), and the name is used inside the function, which outputs several different first names, but an equal last name:

<?php
function familyName($fname) {
    echo "$fname Refsnes.<br>";
}

familyName("Jani");
familyName("Hege");
familyName("Stale");
familyName("Kai Jim");
familyName("Borge");
?>

The following example has a function with two arguments ($fname and $year):

<?php
function familyName($fname, $year) {
    echo "$fname Refsnes. Born in $year <br>";
}

familyName("Hege", "1975");
familyName("Stale", "1978");
familyName("Kai Jim", "1983");
?>
```

```
PHP Default Argument Value
The following example shows how to use a default parameter. If we call the function setHeight() without arguments it takes the default value as argument:

<?php
function setHeight($minheight = 50) {
    echo "The height is : $minheight <br>";
}

setHeight(350);
setHeight(); // will use the default value of 50
setHeight(135);
setHeight(80);
?>
```

```
PHP Functions - Returning values
To let a function return a value, use the return statement: 

<?php
function sum($x, $y) {
    $z = $x + $y;
    return $z;
}

echo "5 + 10 = " . sum(5, 10) . "<br>";
echo "7 + 13 = " . sum(7, 13) . "<br>";
echo "2 + 4 = " . sum(2, 4);
?>
```