---
layout: project
type: project
published: true
image: images/project_1.jpg
title: UI/Database Bank Record System
permalink: projects/project-1
date: 2020-11-03
labels:
 - C
 - User Interface
 summary: Created a project using the programming language C to replicate a simple user interface program that stores records of users. 
---

# UI/Database Bank Record System

## Description: 
The UI/Database Bank Record System allows the program to read into record files containing different user's records prior to actually starting up and using the user interface function of the program. The user interface will interact with the user and adjust the database information based on whether they would like to add a record, print all records, find record(s), delete record(s), or quit the program. Based on the commands, the user interface will then tell the database what to do. The user is able to freely navitage through the different commands back and fourth if they wish. The way the database stores the user records is through heaps. When the program is set to quit, the program will store the current records in the database into a file and the memory of the heap will be cleaned up. 

## A portion of the user interface code that deletes record(s)

else if (prefix(option, "delete") || prefix(option, "4"))
        {
            printf("Delete a record option was selected.\n");
            printf("Deleting a record...account # required\n");
            printf("Enter an account #: ");
            scanf("%d", &accNum);

            if (accNum > 0)
            {
                return_Val = -1;

                return_Val = deleteRecord(&start, accNum);

                if (return_Val == 1)
                {
                    printf("Account #: %d does not exist in the list.\n", accNum);
                }
                else if (return_Val == 0)
                {
                    printf("Record(s) with Account # %d was successfully deleted.\n", accNum);
                }
                else if (return_Val == 2)
                {
                    printf("The record list is empty, no records can be deleted.\n");
                }
            }
            else
            {
                printf("ERROR: Account # needs to be greater than 0. Please try again.\n");
            }
        }


