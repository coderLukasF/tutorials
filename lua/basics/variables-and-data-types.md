# Variables

Variables are used to store data values.


### Rules for naming variables:
* They must start with a letter or underscore.
* They can not start with number
* Case-sensitive, which means **score** would be different than **Score**.

Lua has two types of variables. Local variables, and global variables. 

Local variables are restricted to the current function or block.
Global variables are variables you can use anywhere in the script.

You mainly want to use local variables, but global variables are also a good option for certain use cases too.

We will mainly be **focusing on local** variables on this page.

To create a local variable, simply add local at the start, type your variable name, an equals sign, and the value.
Example:

```lua
local pizzas = 5
```

_Reminder: Lua does **not** require semicolons._


# Data Types
There are many different types of variables you can make in lua. Here are the main three:

## Strings
Strings are basically text. If you don't make your text a string, lua assumes it's a number and then errors, because something like PizzaShop is not a number.

To make your text a string, simply add either ' ' or " " in between your text.
Example:

```lua
local coding = "Fun!"
```

## Numbers/Integers
If you want to add a number/integer, it is very simple. Just type in the number you want.
Example:

```lua
local amount = 17
```

## Booleans (true/false)
Booleans are true or false values. Examples:
```lua
local can_afford = true
local is_raining = false
```


# Printing variables
To print a variable, type in the variable name with no quotation marks.
Example:

```lua
local programming_language = "Lua"
print(programming_language)
```