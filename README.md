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