# Functions

Functions are like variables, but for multiple lines of code.

Functions can also be local or global, but usually you want them to be global.

## How to define a Function

Simply add function at the start, then the name of the function, and parentheses. Then write the code for the function, and end the function by saying end.
Example:

```lua
function HelloWorld()
    print("Hello World")
end
```

## How to call a Function
To call a function, simply type the function name **exactly** (_Lua is case sensitive_) and add parentheses at the end.
Example:

```lua
HelloWorld()
```

# Parameters
With functions, you can also add parameters. To explain it simply, when you call the function you give it data, and the function uses that data.

## Parameters when defining a function.
If you want to add parameters when defining a function, simply add the parameters you want in the parentheses with the name you want it to be. If you have multiple parameters, seperate them with commas. The parameters will act like variables.
Example:
```lua
function PrintParameters(food, drink)
    print(food)
    print(drink)
end
```

If you called the function PrintParameters with the food being pizza, and the drink being soda, then you would get an output like this:

```shell
Pizza
Soda
```

## Parameters when calling a function
If you want to add parameters when calling a function, simply add the parameter inside of the parentheses. If you have multiple parameters, seperate them with commas.

Example:
```lua
PrintParameters("Pizza", "Soda")
```

## Full example

```lua
function PrintMeal(food, drink, dessert)
    print(food)
    print(drink)
    print(dessert)
end

PrintMeal("Steak", "Lemonade", "Ice Cream")
```

Result of the above sample program is:

```shell
Steak
Lemonade
Ice Cream
```