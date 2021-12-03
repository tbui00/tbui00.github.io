---
layout: essay
type: essay
published: true
title: Design Patterns Help Us Design Solutions
date: 2021-12-02
labels:
 - Design Patterns
 - Singleton
 - Software Engineering
---

Let’s start by talking about what is a “design pattern”? Design patterns in a simple sense, is something that is a pattern that helps 
newcomers gain the knowledge and experience that skillful people have. In a more technical sense, we can take a look at the quote by 
Christoper Alexander which states that a design pattern.. 

> _Describes a problem that occurs over and over again in our environment, and then describes the core of the solution to that problem, 
in such a way that you can use this solution a million times over, without ever doing it the same way twice._

>                                                                               -_Christoper Alexander, 1977_

## Understanding Design Patterns with Real World Examples
To try and understand this in other words, design patterns allow us to understand a commonly occurring problem with a reusable solution. 
This reusable solution can be used in different ways. These problems are commonly occurring so often that there are principles we can use 
and follow to solve future problems. To grasp this concept a little better, let’s think about a real-life analogy to design patterns. 

Think of the problem of how you would make a cup of a drink. This can be any drink like tea, coffee, or even milk tea. To make coffee, 
you need various ingredients (components) to end up with a cup of coffee. These ingredients include milk, water, sugar, coffee. 
To make a cup of tea, you need milk, water, sugar, and tea leaves. To make milk tea, you need milk, water, sweetener, and brewed tea. 
We can see a pattern here where the process of making the drink is essentially the same where you need to heat up or brew a certain ingredient 
and mix it all together. The only difference between these different drinks is the ingredients themselves. If we observe this in a design pattern sense, 
we’ve come up with a generic process that allows us to make different drinks. I hope that after reading this example you were able to 
understand design patterns a little bit better. 

## My Experience with Design Patterns
To name a few design patterns that are commonly known in the computer science realm there is a singleton, factory method, observer, 
builder, adapter, MVC (Model-View-Controller), and AntiPatterns. There are many more out there and I will not be explaining all of them 
in this essay but I will go over one pattern, as it relates to a previous project that I am learning about in my current computer science course. 

The design pattern I will go over today is the singleton. The singleton is extremely common and it intends to be able to support a global 
variable in an object-oriented language that may not have the option to declare global variables. To essentially create a singleton, you 
create a class and ensure that only a single instance of that class is available. There are pros and cons to a singleton. 
The pros are that it can provide a “global state” in an object-oriented manner and has easy implementation. The con is that it is not 
thread-safe unless taken care of cautiously and globe states are not generally not good to have. An example of a singleton that I have 
used in my class is in the BowFolios application. The BowFolios application has a MongoDB collection called “ProfileCollection” and is 
accessible by the class “ProfileCollection.” We create a single instance of the ProfileCollection class called “Profiles” which is 
accessible by the rest of the application. Different methods within this application can call upon the single instance of the ProfileCollection 
and manipulate it. I hope that reading about a real application in software development for a web application helps you understand what 
a singleton design pattern is.

&nbsp;
&nbsp;
