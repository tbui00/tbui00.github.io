---
layout: project
type: project
image: images/project_1.png
title: UI/Database Bank Record System
permalink: projects/ui-database
date: 2020-11-03
labels:
  - C
  - Database
summary: A C program that replicates a simple user interface project that stores records of users in a database. 
---

![bank image](https://tbui00.github.io/images/bank_image.jpg)

## Description:
The UI/Database Bank Record System allows the program to read into record files containing different user's records before actually starting up and using the user interface function of the program. The user interface will interact with the user and adjust the database information based on whether they would like to add a record, print all records, find the record(s), delete record(s), or quit the program. Based on the commands, the user interface will then tell the database what to do. The user can freely navigate through the different commands back and forth if they wish. The way the database stores the user records is through heaps. When the program is set to quit, the program will store the current records in the database into a file and the memory of the heap will be cleaned up. 

## Role:
This was an individual project was created through a series of smaller programs created to work towards this big one that puts everything together. It was a self-learning process where every line of code needed to be unique to ours and as classmates, we could not share code amongst each other. I was responsible for all the work for creating this user interface and storage of the database program. 

## Learned Experience:
This project was weighed heavily because it was one of the two final projects that were counted towards our grade. Before creating the final project, each student needed to work on the individual main components such as understanding how to delete, add, find, and print the information in the heap. After completing each component, the final then requires you to put it all together which allows the program to fully function as a whole. Through this process, I've learned that programming for C was very difficult because we utilized pointers for basically everything to access information within the heap. However, it helped me to understand the structure of heaps better as I was able to see how the information was processed and delivered through the user interface and database.

## A portion of the database code traversing to find a location to insert:

        current = *start;

        /* traverse through list and find location to insert new record */
        while (current != NULL && location == 1)
        {
            /* if location to insert is found correctly */
            if (current->accountno <= new->accountno)
            {
                location = 0;
            }
            else
            {
                /* continue to search */
                prev = current;
                current = current->next;
            }
        }


Here is a link to the github project page for the [UI/Database Bank Record System](https://github.com/tbui00/ui-database-bank).

&nbsp;
&nbsp;

