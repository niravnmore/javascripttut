# Javascript

## Introduction

Javascript is a light-weight cross-platform single threaded object oriented scripting language. All webbrowsers are easily able to interpret javascript and is executed line by line. Javascript is a dynamically typed language and uses same syntax as used by C programming language.

Javascript is used to create and animate dynamic elements on a webpage and has several similar uses such as

- client-side data validation
- dynamic drop-down menu
- displaying date and time
- displaying dialog box, pop-up windows
- displaying date and time (real-time clock)

Here is an example of a simple script to display 'hello world' on a webpage using javascript :

    <!DOCTYPE html>
    <html lang="en">
        <head>
            <title>Javascript Example</title>
        </head>
        <body>
            <script type="text/javascript" src="">
                document.write("hello world!");
            </script>
        </body>
    </html>

There are several other uses of javascript due to the versatility provided such as

- It is used for creating interactive websites, gaming and mobile applications.
- It is used to manage client-side logic for websites and also provides several libraries like react, vue and angular to work with.
- It can also be used for server side login handling with the help of nodejs libraries.
- It also provides libraries to develop and train machine learning models.

#### Advantages

- using javascript a webpage can be made more interactive and responsive.
- less server load and faster page response.
- used to create interactive features.
- it can be used in several applications with the help of external libraries and frameworks.

#### Disadvantages

- Javascript does not provide multi-threading capabilities.
- Javascript is a dynamically typed language and so does not provide strict type checking.
- There are security risks involved and can be exploited for XSS for injecting malacious scripts.

#### Tools

A simple notepad or text editor and a browser is required to create and execute javascript. We are using VS Code as our text editor and Chrome as our browser.

## Adding Javascript to HTML

Javascript can be included within an HTML file in three different ways :

- Inline : placing javascript directly within HTML element of interest.
- Internal : placing javascript code in `<script>` tag and placing it in the head or body of the document.
- External : creating a separate js file and adding a link of the file in HTML document using `<script>` tag.
- Asynchronous and Deferred : using an external js file with async or deferred option to optimise or manipulate webpage structure.

## Comments in Javascript

Comments are used to add information about the code, warnings or suggestions which can help to understand the code and deliver a message.  
Javascript comments are not executed and ignored by Javascript engine.  
Comments can also be used to exclude certain lines of code from being executed.

Single line comments can be added using `//` at the start of the comment. Anything written after `//` will not be executed for that line.

    //This is a single line comment

Multi line comments can be added by using `/*` and `*/`. Any code written between these tags will be consided as comments and will not be executed.

    /*
    This is a
    multi
    line
    comment
    */

## Variables in Javascript

- Variables in javascript should start with (first character) alphabets (`a-z`, `A-Z`), underscore (`_`) or dollar sign (`$`).
- Variable name may contain alphanumeric characters (`a-z`, `A-Z`, `0-9`), underscore (`_`) and dollar sign (`$`).
- Javascript variables are case sensitive so variable `num` will be different from `Num` or `NUM`.
- Reserve keywords as variable name are not valid.

Variables can be defined by the keyword `var`. It has a global-scope behavior. e.g.,

    var a = 10;
    var msg = 'Hello World';

Keyword `var` is optional. Variables can be defined without any keyword and still have same properties as defined through `var`. e.g.,

    myVar = 'This variables is defined without using any keyword';
    newNumber = 108;

Variables can also be defined using `let` keyword for block-scoped characteristics.

    let newvar = 24;
    let temp = 55;

Javascript also provides option to define contants by using `const` keyword. Value of constants cannot be reassigned.

    const PI = 3.14;

## Variables Scope in Javascript

- In Javascript variables can have global (function) scope or local scope.
- Any variable defined through `var` keyword or without it inherites global scope.
- Any variable defined using `let` and `const` keyword will have local scope properties and will not be available anywhere outside the block.
- Variables can also be defined and stored using `window` object and used as a global variable.

        window.myVar = 'Variable through window object.';

- Any variable defined outside function are added internally to `window` object and can be accessed using `window` object. e.g.,

        var myVar = "This is a global variable";
        function myFunc() {
            document.write(window.myVar);
        }
        myFunc(); // prints -> This is a global variable

## Datatypes in Javascript

Javascript provides different datatypes to store data.

- Primitive Datatypes

  1. string - to store text.
  2. number - to store imtegers, float, etc.
  3. boolean - store true or false values.
  4. null - when variable field is empty but not undefined.
  5. undefined - is generated variable value is not assigned.
  6. bigInt
  7. symbol

- Composite Datatypes

  1. Object - collection of data in a key value pattern.
  2. Array - collection or list of elements.
  3. Date - date datatype is used to manipulate date.

- Array example :

        var cars = ["Swift", "XUV", "Alto"];

- Object example

        var customer = {
            firstname: "Rahul",
            lastname: "Dravid",
            profession: "cricketer"
        };

## Operators in Javascript

Javascript operators are symbols that are used to perform operations on operands.

<table>
<tr>
<th>Operators</th>
<th>Description</th>
<th>Example</th>
</tr>
<tr>
<th>Arithmetic Operators</th>
</tr>
<tr>
<td>+</td>
<td>Addition</td>
<td>a + b</td>
</tr>
<tr>
<td>-</td>
<td>Substraction</td>
<td>a - b</td>
</tr>
<tr>
<td>*</td>
<td>Multiplication</td>
<td>a * b</td>
</tr>
<tr>
<td>/</td>
<td>Division</td>
<td>a / b</td>
</tr>
<tr>
<td>%</td>
<td>Modulus</td>
<td>a % b</td>
</tr>
<tr>
<td>++</td>
<td>Increment</td>
<td>++i , i++</td>
</tr>
<tr>
<td>--</td>
<td>decrement</td>
<td>--i , i--</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<th>Comparison Operators</th>
</tr>
<tr>
<td>==</td>
<td>Is equal to </td>
<td>a == b</td>
</tr>
<tr>
<td>===</td>
<td>Is equal and of same type</td>
<td>a === b</td>
</tr>
<tr>
<td>!=</td>
<td>Is not equal to</td>
<td>a != b</td>
</tr>
<tr>
<td>!==</td>
<td>Is not equal and of not same type</td>
<td>a !== b</td>
</tr>
<tr>
<td>></td>
<td>Is greater than</td>
<td>a > b</td>
</tr>
<tr>
<td>>=</td>
<td>Is greater than or equal to</td>
<td>a >= b</td>
</tr>
<tr>
<td><</td>
<td>Is less than</td>
<td>a < b</td>
</tr>
<tr>
<td><=</td>
<td>Is less than or equal to</td>
<td>a <= b</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<th>Bitwise Operators</th>
</tr>
<tr>
<td>&</td>
<td>Bitwise AND</td>
<td>a & b</td>
</tr>
<tr>
<td>|</td>
<td>Bitwise OR</td>
<td>a | b</td>
</tr>
<tr>
<td>^</td>
<td>Bitwise XOR</td>
<td>a ^ b</td>
</tr>
<tr>
<td>~</td>
<td>Bitwise NOT</td>
<td>~a</td>
</tr>
<tr>
<td><<</td>
<td>Bitwise left shift</td>
<td>a << b</td>
</tr>
<tr>
<td>>></td>
<td>Bitwise right shift</td>
<td>a >> b</td>
</tr>
<tr>
<td>>>></td>
<td>Bitwise right shift with zero</td>
<td>a >>> b</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<th>Logical Operators</th>
</tr>
<tr>
<td>&&</td>
<td>Logical AND</td>
<td>a && b</td>
</tr>
<tr>
<td>||</td>
<td>Logical OR</td>
<td>a || b</td>
</tr>
<tr>
<td>!</td>
<td>Logical NOT</td>
<td>!a</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<th>Assignment Operators</th>
</tr>
<tr>
<td> = </td>
<td>Value assignment operator</td>
<td>a = 5, b = a</td>
</tr>
<tr>
<td>+=</td>
<td>Add and assign</td>
<td>a += b</td>
</tr>
<tr>
<td>-=</td>
<td>Substract and assign</td>
<td>a -= b</td>
</tr>
<tr>
<td>*=</td>
<td>Multiply and assign</td>
<td>a *= b</td>
</tr>
<tr>
<td>/=</td>
<td>Divide and assign</td>
<td>a /= b</td>
</tr>
<tr>
<td>%=</td>
<td>Modulus and assign</td>
<td>a %= b</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<th>Assignment Operators</th>
</tr>
<tr>
<td>?:</td>
<td>Conditional operator</td>
<td>a == b ? x = true : x = false</td>
</tr>
<tr>
<td>,</td>
<td>Comma operator allows evaluation of multiple expressions in single statement</td>
<td>let a = (1,2,3); a = 3</td>
</tr>
<tr>
<td>delete</td>
<td>delete property deletes an entry from an object</td>
<td>delete x, delete person.lastname</td>
</tr>
<tr>
<td>in</td>
<td>in operator checks if a property exist in the object array</td>
<td>prop in object</td>
</tr>
<tr>
<td>instanceof</td>
<td>checks if the object is an instance of given type</td>
<td>object instanceof objectType</td>
</tr>
<tr>
<td>new</td>
<td>create a new object</td>
<td>var a = new obj();</td>
</tr>
<tr>
<td>typeof</td>
<td>checks the type of object</td>
<td>typeof 5 //"number" </td>
</tr>
<tr>
<td>void</td>
<td>it discards expressions return value</td>
<td>void function(x)</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
</table>
