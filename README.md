Osmanys Perez
# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 
    
    A: .map takes an array, make a copy and then modify it. should not be used if the aray it return won't be used, or if the value of the callback function is not used.
        you can use .map return an array single key-value pair of the objects inside another array.
        example: arr1 = [
            {name: "Mike", age: 23, location: location}
            {name: "Stuart", age: 18, location: location}
            {name: "Tony", age: 25, location: location}
            ]
            arr1.map(item => item.name) //returns ["Mike", Stuart, Tony]

        .reduce takes an array and uses its values to calculate a new value. it returns a single value.
        you could use .reduce to calculate an average or a total. Takes in 2 parameters(a function and a starting value). The function
        inside filter will also take 2 parameters, the first one is the accumulator that will keep the running total of the operation, the
        second one the current item that the function is working on.
        example: arr1 = [
            {name: "Mike", age: 23, location: location}
            {name: "Stuart", age: 18, location: location}
            {name: "Tony", age: 25, location: location}
            ]
            arr1.reduce((accumulator, current) => (accumulator += current.age) / 2, 0) // Will return the average age of all objects in arr1

        .filter filters the array it receives based on a condition, it will return an array of objects or values that evaluate to true for its condition.
        it can be used to filter out all objects inside an array that do not meet the desired condition.
        example: arr1 = [
            {name: "Mike", age: 23, location: location}
            {name: "Stuart", age: 18, location: location}
            {name: "Tony", age: 25, location: location}
            ]
            arr1.filter(items => item.age > 20) //will filter out all objects whose age value is less than 20, returning an array of objects that met the condition



2. Explain the difference between a callback and a higher order function.
A: A callback is a function that gets passed as an argument to another function, while higher order are functions that take other functions as arguments.
    note that a function can be both a callback function and a higher order function at the same time.

3. Explain what a closure is.
A: A closure happens when a (inner) function is enclosed in a (outter) function, and has access to the outer function data even whe that function has cosed.

4. Describe the four principles of the 'this' keyword.
A:  1 global binding(window binding): when "this" is used in a function in the global scope, it points to the window object.
    2 implicit binding: when a function is called with a preceding dot, "this" points to the object that contains said function.
    3 explicit binding: when call() or apply() are used, "this" is explicitly defined
    4 new binding: in a constructor function, "this" points to the instance that is going to be created by that constructor function(new Keyword)


5. Why do we need super() in an extended class?
A: super() will make sure that the child class inherits the parent class properties.

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Clone your forked version of the repo
3. cd into your repo and create a branch with your first and last name
4. open the terminal in your vs code and type `npm install`
5. next type `npm run test` in your terminal
6. Complete your work making regular commits, once you have all your tests passing and you are ready to submit your work please see canvas for instructions on how to submit

### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://www.notion.so/lambdaschool/Submitting-an-assignment-via-Code-Grade-A-Step-by-Step-Walkthrough-07bd65f5f8364e709ecb5064735ce374)

