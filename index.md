## Introduction
Hello, my name is Evan Boucher.

## Purpose 
The purpose of this page is to show the improvement of my skills by taking a previously made project, and enhance it in three different ways. The project I chose is an arena shooter game that I created in a college class. The enchancements I have made to this project are split into three main categories; Software Design and Engineering, Algorithms and Data Structures, and Databases. Before working on the enhancements I reviewed the original code in the project to show where I am starting from, and to outline my goals. 

## The Code Review 
[Youtube Link To Code Review](https://youtu.be/oa3iN82uB4Y)

## Enhancement One - Software Design and Engineering 
  

[Enhancement One Repository](https://youtu.be/oa3iN82uB4Y)

## Enhancement Two - Algorithms and Data Structures 
  The second enhancement introduces a new enemy type; the turret. This turret functions very differently from the normal enemies that are currently in the game, it does not move and cannot be killed. The turret is a stationary obstacle that forces the player to limit their active area, or to not stay still when in the turrets sight range. The turret automatically targets and shoots at the player if they walk in its sight range and will stop shooting if they leave the range. To create the turret I had to create an algorithm that dictates the turret's AI behavior. This algorithm searches for any objects that overlap with the turrets sight range, and checks if it is a player object. If it is a player then it faces and shoots at it, otherwise it will ignore it. Once the player leaves the sight range it will stop shooting and becomes inactive again.
  Most of my time in this enhancment was in bug-fixing and testing. The main challenge I ran into was not creating the turret's functionality, but instead spawning the turrets at the correct time and place while still having them target the player. I ran into issues where the turrets would spawn on the wrong waves, occasionly spawn on top of each other, and also not being to target the player from on top of the walls and cubes they were stationed on. 

[Enhancement Two Repository](https://youtu.be/oa3iN82uB4Y)

## Enhancement Three - Databases
  For the third enhancement I added database interaction in the form of a user login screen and a way to store and view all previous survival gamemode scores. This allows the player to create a new account and login with that account to play the game, and each attempt at the survival gamemode will be saved to this database by the user's account. This was done using a MySQL database that is hosted on a free Clever Cloud server. I also made a change to the arena game mode that now displays the players username on the scoreboard instead of the default name that was part of the original artifact. Being able to see past scores give more immsersion to the player and lets them see if they are improving at the game, and will give reason to continue to play the game.
  Most of the difficulty when working on this enhancement was in using Unreal Engine's tools to do what I need. Creating and using the databases was very simple, but being able to use that data on screen was difficult. Being able to add each of the past game scores on screen took multiple attempts as the ways to generatively add text on screen is not the most intuitive in Unreal Engine.

[Enhancement Three Repository](https://youtu.be/oa3iN82uB4Y)

## Professional Self-Review

