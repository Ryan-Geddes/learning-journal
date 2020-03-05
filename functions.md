Borrowed from Taylor Thornton.   You take amazing notes!!!!


<!-- pp. 1-24, 74-79, 88-94  -->

# Chapter 1a Summary: pages 1-24
- A script is a series of instructions that the computer can follow in order to achieve a goal. 
- Eaach time the script runs, it might only use a subset of all the instructions. 
- Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task programmatically. 
- To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task - a flowchart can help. 

**Script is a series of instructions that a computer can follow to achieve a goal, you can compare scripts to recipes, handbooks, and manuals.  A browser may use different parts of the script depending on how the user interacts with the webpage.  Scripts can run different sections of the code inresponse to the situations around them**

## Writing a Script
1. Define the goal: define the task you want to achieve 
1. Design the Script: split the goal into a series of tasks that are going to be involved in solving this puzzle.  This can be represented using a flowchart. 
    * You can then write down steps the computer needs to perform in order to complete each individual task, rather like writing a recipe it can follow 
1. Code each step: Each of the steps needs to be written in a programming language that the computer understands, in our case, this is JavaScript. 

**Computers solve problems *programmatically*; the follow a serious of instructions one after another.**

## Expressions, p 74-79 
**An expression evaluates into, or results in, a single value. Broadly speaking there are two types of expressions** 

1. Expressions that just assign a value to a variable
    * in order for a variable to be useful, it needs to be given a value.  As you have seen, this is done using the assignment operator aka the equals sign `=`
    * when you first declare a variable using the var keyword, it is given a special value of undefined, this will change when you assign a value to i.  Technically, undefined is a data type like anumber, string or boolean. 
1. Expressions that use two or more values to return a single value 
    * You can perform operations on any number of individual values to determiine a single value
    * ex: `var area = 3 * 2;` the value of area is now 6.  
    * here the expression 3 * 2 evaluates into 6.  This example also uses the assignment operator, so the result of the expression 3 * 2 is stored in the variable called area. 
    * another example where an expression uses two values to yield a single value would be whre two strings are joined to create a single string. 

## Operations
**Expressions rely on things called *operators* they allow programmers to create a single value from one or more values**
* Assignment operators: assign a value to a variable for ex, `color = 'beige';`
* Arithemetic operators: perform basic math for ex, `area = 3 * 2` the value of the area is now 6
* String operators: combine two strings. ex, `greeting = 'hi' + 'molly';` the value of greeting is now Hi Molly. 
* Comparison Operators: compara two values and return return true or false. Ex, `buy = 3 > 5` the value of buy is false 
* Logical operators: combine expressionsd and return true or false. Ex, `buy = (5 > 3) && (2 >4)` the value of buy is now true 

## Arithemetic Operators

JavaScript contains the following mathematical operators, which you can use with numbers. 
- Addition `+`
- Subtraction `-`
- Division `/`
- Multiplication `*`
- Increment `++` adds one to the current number
- Decrement `--` subtracts one from the current number 
- Modulus `%` divides two values and returns the remainder 10 % 3 results in 1 
- MDAS applies 

**Using Arithmetic Operators**
- Mathematical operators can use variables that represent numbers, that is, numbers do not need to be written explicitly in code. 

## String Operator 
- There is just one string operator `+` symbol.  It is used to join the strings on either side of it. 
- The process of joining two or more strong to create one new string is called **concatenation**
- Mixing numbers and strings together: when you place quotes around a number it is a string-not numeric data type- and you cannot perform addition operations on strings. 

**Using String Operators** 
- Example used in the book will display a personalized message on the page

## What is a function? 
- Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function-rather than repeating the same set of statements. 
- Calling: when you ask the function it person its task it is called *calling* the function 
- Remember from the last chapter that a code block consists of one or more statements containted within curly braces, and you do not write a semicolon after the closing curly brace like you do after a statement. 
- Parameters: pieces of information passed to a function are known as *parameters* 
- Return value: when you write a function and you expect it to provide you with an answer the response is known as a *return value* 

**Declaring a function** to create a function you give it a name and then write the statements needed to achieve its task inside the curly braces.  This is known as a *function declaration* 
    1. you declare a function using the function keyword 
    1. you give the function a name sometimes called an identifier followed by parentheses 
    1. the statements that perform the task sit in a code block-they are inside curly braces. 

**Calling a function** having declared the function, you can then execute all of the statements between its curly braces with just one line of code this is known as *calling the function*. 
    1. to run the code in the function, you use the function name followed by parentheses
    1. in programmer-speak you would say that this code calls a function 
    1. you can call the same function as many times are  you want within the same js file

**Declaring functions that need information** sometimes a function needs specific infomration to perform its task. In such cases, when you decleare the function you give it parameters.  inside the function, the parameters act like variables. 
    1. if a function needs information to work you indicate what it needs to know in parentheses after the function name. 
    1. the items that appear inside the parentheses areknown as the parameters of the function.  inside the function those words actlike variable names. 

**Calling functions that needs information** when you call a function that has parameters you specifcy the values it should use inthe parentehses that follow its name.  The values are called arguments and they can be provided as values or variables. 
    1. arguments as values p. 93 
    1. arguemnts as variablesp p. 93

**Getting a single value out of a function** some functions return information to the code that called them. For example, when they perform a calculation they return the result 
    1. this calculate function returns the area of a rectangle to the code that called it 
    1. inside the function a variable called area is created.  it holds the calculated area of the box 
    1. the return keyword is used to return a value to the code that called the function
