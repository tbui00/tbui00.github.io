---
layout: project
type: project
image: images/project_1.jpg
title: UI/Database Bank Record System
permalink: projects/ui-database
date: 2021-11-03
labels:
  - C
  - Database
summary: Created a project using the programming language C to replicate a simple user interface project that stores records of users in a database. 
---

# UI/Database Bank Record System

## Description: 
The UI/Database Bank Record System allows the program to read into record files containing different user's records prior to actually starting up and using the user interface function of the program. The user interface will interact with the user and adjust the database information based on whether they would like to add a record, print all records, find record(s), delete record(s), or quit the program. Based on the commands, the user interface will then tell the database what to do. The user is able to freely navitage through the different commands back and fourth if they wish. The way the database stores the user records is through heaps. When the program is set to quit, the program will store the current records in the database into a file and the memory of the heap will be cleaned up. 

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


