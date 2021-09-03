---
layout: project
type: project
image: images/poroSpriteSheet.png
title: The League of Legends Snake
permalink: projects/league-snake
date: 2019-12-09
labels:
  - Java
summary: A final group project where we created an alternative way of playing the classic Snake game. 
---

## Description: 
The course taken was ICS 111 and the final for the course was a final group project where we had to work together to create a game. Our group decided to create a snake game but with a twist. Instead of the traditional Snake that needs to go in one direction and cannot touch any part of its body, we made a sprite named "Poro" that is able to navigate around the map and dodge objects that comes towards it. Poro is actually a very small puff ball that is from the game League of Legends. It was not our intention for it to stray away from the original Snake game. The enemies themselves gradually increase in number over time and spawn at random points in the map. In order to win the game you will need to collect a certain amount of cookies that are randomly placed around the map. 

The group work was divided evenly where we all took turns writing the code together during class time and helped each other if we were to have trouble with any part of it. We each had moments where we were unsure of what to write down and received help from each other collaboratively. 

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
