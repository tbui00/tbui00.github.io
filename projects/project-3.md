---
layout: project
type: project
image: images/poroSpriteSheet.png
title: The League of Snakes
permalink: projects/league-snake
date: 2019-12-09
labels:
  - Java
summary: A final group project utilizing Java language where we created an alternative way of playing the classic Snake game. 
---

![Image of background](https://tbui00.github.com/images/summonersRift.jpg)

## Description: 
The course taken was ICS 111 and the final for the course was a final group project where we had to work together to create a game. Our group decided to create a snake game but with a twist. Instead of the traditional Snake that needs to go in one direction and cannot touch any part of its body, we made a spirite named "Poro" that is able to navigate around the map and dodge objects that comes towards it. Poro is actually a very small puff ball that is from the game League of Legends. It was not our intention for it to stray away from the original Snake game. However, it evolved into a game that requires you to dodge enemies and obtain poro snacks in order to win. The enemies themselves gradually increase in number over time and spawn at random points in the map. In order to win the game you will need to collect a certain amount of cookies that are randomly placed around the map. 

## Role:
The group work was divided evenly where we all took turns writing the code together during class time and helped each other if we were to have trouble with any part of it. We each had moments where we were unsure of what to write down and received help from each other collaboratively. I also created the Poro spirite that you see as the image of this program. We are able to see the how the Poro looks like and changes appearance when it moves up, down, left, and right.

## Learned Experience:
This was the first group project I ever had and it was interesting to experience it as it was the only the introduction course to computer science. When I first decided to pursue a degree in computer science, I thought that computer scientists spent all their time alone working on code by themselves. However, I was able to learn that the projects you work on will more often than not be collaborative. It requires a lot of team effort if you would like to maintain and manage an extremely large program or application. It also helps you learn if you do not know an answer but the person sitting next to you has the answer to all your questions. Although puts you out of your comfort zone, you are able to learn from each other and grow as a software engineer. 

## A sample of the main source code:
    //allows the poro to collect porosnax and increases the score by 1 per snack
	public static void collect() {
		if (poro.isInside(Collectibles.snaxX(), Collectibles.snaxY())) {
			Collectibles.translateTo(3000,3000);
			new Collectibles();
			score++;
			text.setMsg("Score: " + score);
			eat.play();
		}
	}
	
	//moves each enemy towards the poro
	public static void moveEnemies() {
		for (int i = 0; i < eList.size(); i++) {
			eList.get(i).move(poro.x, poro.y);
		}
	}
		
	//checks if poro has crashed into the enemy
	public static boolean isPoroCaught() {
		for (int i = 0; i < eList.size(); i++) {
			if (eList.get(i).isInside(Sprite.x, Sprite.y)) {
				return true;
			}
		}
		return false;
	}

&nbsp;
&nbsp;
