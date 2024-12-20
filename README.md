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
