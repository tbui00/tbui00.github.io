---
layout: project
type: project
image: images/project_2.png
title: Pokemon Pokedex
permalink: projects/pokedex
date: 2020-12-10
labels:
  - C++
  - Database
summary: A C++ program that will create instances of the child classes in the heap memory, creating two data containers. 
---

![pokemon image](https://tbui00.github.io/images/pokemon_image.jpg)

## Description: 
This project was our 9th project where we began using C++. We are utilizing the classes in order to make our own pokemon team in the form of a database. This helped us build a better understanding of how C++ can be used to store data in the heap memory and how objects are stored.

## Role:
This project is individual and the code is all written by me. The project gave us a description of what the program needed to fulfill and a basis amount of code necessary to complete the project. We needed to use the ideas learned from class, understand how the structure works, and use C++ language in order to complete this project.

## Learned Experience:
This project was one of the many assignments done in the course ICS 212. Since this was one of the few C++ projects done, it was interesting to see how C and C++ can be different and also similar. I find that C was a lot more concrete in its structure and felt very traditional. While C++ was easier to maneuver with knowing the basis of C. After completing this course (ICS 212) I found that there is much more simplicity in C/C++ in comparision to Java. It made me appreciate the differences in these programming languages and helped me narrow down which languages I would prefer coding in. I would like to work more with C++ in future to create games.

## A sample of the main function:

    int main(int argc, char *argv[])
    {
    vector<Pokemon*> poke_vec;
    map<string, Pokemon*> poke_map;

    /* creates instance of all child classes in heap memory */
    Pokemon *P1 = new Lugia;
    Pokemon *P2 = new Lapras;
    Pokemon *P3 = new Lucario;

    /* stores addresses of objects into vector poke_vec */
    poke_vec.push_back(P1);
    poke_vec.push_back(P2);
    poke_vec.push_back(P3);

    /* stores addresses of objects into map poke_map */
    poke_map["lugia"] = P1;
    poke_map["lapras"] = P2;
    poke_map["lucario"] = P3;

    /* calls checkPokedex function by each element of the containers */
    cout << "\nVector Data Container: \n";
    cout << "-----------------------------\n";
    checkPokedex(poke_vec[0]);
    checkPokedex(poke_vec[1]);
    checkPokedex(poke_vec[2]);
    cout << "-----------------------------\n";
    
Here is a link to the github project page for the [Pokemon Database]( https://github.com/tbui00/pokemon-database).

&nbsp;
&nbsp;
