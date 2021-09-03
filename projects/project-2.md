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

## Description: 
This project was our 9th project where we began using C++. We are utilizing the classes in order to make our own pokeon team in the form of a database. This helped us build a better understanding of how C++ can be used to store data in the heap memory and how objects are stored. 

## A sample of the main function

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
