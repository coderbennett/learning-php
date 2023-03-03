# Learning PHP
------------------
This repository contains files and notes that Joey Bennett is creating while following along freeCodeCamp's [PHP Programming Language Tutorial - Full Course](https://www.youtube.com/watch?v=OK_JCtrrv-c).

The following are notes from the course:

## installation
make sure to install php on the computer. 

## create path variable
create a new path variable to the php folder

## starting a local server
to start a php server run the command in git bash/terminal `php -S localhost:4000`

## php scripting
use the extension .php
php is very tightly coupled with HTML. In VScode I can do the html5 shortcut and create a simple HTML layout.

when creating php scripts within HTML you use php elements just like html elements

For example:

	<?php
	echo("Hello World");
	?>

The above code will print the words Hello World to the page

## displaying php to localhost
make sure when you run your server on localhost on the command line/terminal that you are in or above the directory you are working in.

For example:

`http://localhost:4000/php-projects/learning/hello_world/site.php`

this will let the local host server display the php page along this file path

## variables
variables are containers to store info

For example:

`$characterName = "John";`
`$characterAge = 35;`

### placing variables in strings
variables can be directly placed into strings with the $ operator

For example:

        echo("There once was a man named $characterName <br>");
        echo("He was $characterAge years old. <br>");
        echo("He really liked the name $characterName. <br>");
        echo("But didn't like being $characterAge. <br>");

### updating variables
variables can be updated by simply giving it a new value the same way it was initialized.

For example:

`$characterName = "Mike";`  

## data types

### strings
when initializing a string, always put double quotes around it.

## numbers
two different types of numbers. This is important to understand because php differentiates the two types of numbers.

### integer
whole numbers, essentially a number without a decimal point

## floating point numbers / decimal point numbers
numbers with a decimal point 

## boolean
true or false value

## null
null value basically means a variable has no value

## Strings
Plain text variables.

### methods
`strtolower();`
This will turn the string into all lowercase letters.

`strtoupper();`
This will turn the string into all uppercase letters.

`strlen();`
This will return the length of the string.

`$phrase[0];`
This is how we can access a particular index of a string.

`$phrase[0] = "B";`
This will change the value at the particular index of the string.

`str_replace("Giraffe", "Panda", $phrase);`
This will replace the string Giraffe with Panda in the variable phrase.

`echo substr($phrase, 8, 4);`
This will return a substring from the variable phrase, starting at index 8, 4 characters forward.

## numbers
### operators
Just like JS, you can use +-/* and % to manipulate numbers.

### incrementors/decrementors
we can use $num++, $num--

there is also 

`$num+= 5;`
`$num -= 5;

The above will add or subtract 5 to the current value of num and update the value.

### methods
`abs($num);`
absolute value

`pow(2, 4);`
this will return 2^4

`sqrt(144);`
this will return the square root of 144

`max(2, 10);`
this function will tell us which of these two numbers is larger

`min(2, 10);`
this function will tell us which of these two numbers is smaller

`round(3.2);`
This will round down to 3 (would round up if it was >3.5)

`floor(3.9);`
This will always round down (to 3 in this case).

`ceil(3.1);`
This will always round up (to 4 in this case).

## user input
If we make a form in our HTML like:

	<form action="site.php" method="get">
	
	        Name: <input type="text" name="name"/>
	
	        <input type="submit"/>
	
	</form>

We can access the input with:

`$_GET["name"];`

## form URL query strings
when using a form in php, variables will be placed into the URL after a ? 

For example:

`http://localhost:4000/basic_calculator/site.php?num1=10&num2=21`

The above example has num1 and num2 stored, and these are being rendered on screen via `$_GET["num1"]`

