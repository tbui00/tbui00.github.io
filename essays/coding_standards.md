---
layout: essay
type: essay
published: true
title: Why Follow Coding Standards
date: 2021-09-23
labels:
 - Javascript
 - Education
 - ESLint
---
When the words "coding standards" come into a conversation,  it is common to think you have a set of rules to follow to structure your code. We may think of it as something simple, or question whether it's useful in our code. If we did not have coding standards for programming languages, it is more likely that everyone's code will be structurally different, difficult to read and understand, and hard to add to. It may reach a point where the code can be incomprehensible and people may not find it beneficial to read although it may have a solution.

##Are Coding Standards Useful?
When we apply coding standards to a specific programming language that we learn, we are not only creating a good practice in how to properly structure our code but we are allowing for readability. This readability can go a long way in terms of learning the programming language and allowing others to efficiently understand the code. When you can stick to coding standards that are particular to a programming language, you can read it easier and this allows you to direct your attention to understanding the code and language instead of spending your time trying to read it. You get used to the way something is structured, allowing good habits to form. Not only is something easier to read but the programming language is recognized.

##Javascript with ESLint on IntelliJ IDEA
The course ICS 314 is a required software engineering course that has a couple of modules that teach you about the Javascript programming language. To learn Javascript in this course, it is required that the IDE IntelliJ IDEA is used and the only inspection needed is ESLint. ESLint is the coding standard that will be checking the code for any issues that fall out of line with the coding standards. As the code is typed, ESLint will be actively checking for any errors and it will be displayed in the problems tab of your code or you can manually hover the cursor over each squiggly red line to see what the issue is.  If there are no errors, there will be a green checkmark in the top right corner of the screen within the IntelliJ IDEA application. This is a great sign of relief that your code satisfies the coding standards that are particular to the Javascript language in respect to ESLint's standards.

From experience thus far, using ESLint has helped me code with Javascript and further my understanding of the Javascript programming language. Before using IntelliJ IDEA, we used JSFiddle to code Javascript. This was a browser code editor to write and test your Javascript, CSS, HTML, or CoffeeScript code online. Although this does have its respective inspection programs to detect errors in lines of code, it was difficult to pinpoint what the error was. The error messages that showed up in the console would state the number that should indicate the line of code with the error, however, it was confusing as that was not the actual line containing the error. When using ESLint on IntelliJ IDEA, I can pinpoint my errors directly and some suggestions tell you how to make your code better. For example, take a look at the piece of code that I wrote for one of my exercises in the course.

```
1 function zipList(list1, list2) {
2  let finalList = [];
3  for (let i = 0; i < list1.length; i++) {
4    finalList.push(list1[i], list2[i]);
5  }
6  return finalList;
7  }
```

Particularly, take a look at line 2. When first learning Javascript, it is a habit to declare many of your variables with the word "let" rather than "const." It is learned that using "var" is not recommended due to the scope access and declaring variables with "const" normally means you don't want that variable to change its value. ESLint sees line 2 of the code, marks it as an error, and provides an informative message which looks like "ESLint:'finalList' is never reassigned. Use 'const' instead. (prefer-const)" This information was taught at the beginning of the course when I took FreeCodeCamp.org which gives you a basic understanding of the Javascript ES5 language and ES6 language. However, I never got to apply this basic knowledge to my coding until ESLint informed me. Knowing that since the variable is an array list is never reassigned and we are just changing the content inside of the array list helped me better understand the Javascript language and why using "const" is preferred over "let" in such cases. Utilizing the coding standard program ESLint allowed me to further my understanding of the JavaScript programming language on top of gaining a good habit of learning code structure and rules. 
