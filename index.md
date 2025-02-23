# CS-499 ePortfolio

## Introduction
Hello, my name is Evan Boucher and I am currently a senior at SNHU. This page provides an ePortfolio for my work on the CS-499 capstone project where I took a project I had previously created, and made enchancements to it.

## Professional Self-Assessment
  
  Throughout the Computer Science program I have created many different projects with multiple languages and goals, and I feel that throughout working on the projects I have learned many useful tools and skills that prove my strengths. I have not only learned about the basics of programming, I have also learned the basics of many of the major fields of the CS industry, such as software development, website design, security, database development, game design, and computer graphics. Showcasing that I am capable of even just the basics of these fields proves that I am capable and willing to learn about new topics and areas, meaning that employers will see that I can work in a new field and still be capable of learning the new material and putting it to use.
  
	Collaborating and communicating are important factors in the Computer Science field as development is a group effort between multiple parties. There has to be good communication within the development team and between the stakeholders to show that the developers are creating the product that the stakeholders want and to show that work is getting done in a timely manner. I have proven that I am capable of this by creating projects that are inline with the class’ goals and that I have completed these projects on time. I have also proven my skills in software engineering, algorithms, and databases throughout my courses by developing working products that make use of these principles.

## Purpose 
  The purpose of this page is to show the improvement of my skills by taking a previously made project, and enhancing it in three different ways. The project I chose is an arena shooter game that I created in a game design class. The enhancements I have made to this project are split into three main categories; Software Design and Engineering, Algorithms and Data Structures, and Databases. Before working on the enhancements I reviewed the original code in the project to show where I am starting from, and to outline my goals. The reason I selected a game to enhance is because I feel that working with this artifact will let me be more creative, alongside having all of the changes that I make be very noticeable. This game was created in Unreal Engine, one of the most popular game engines. When I created the original artifact, the class used Unreal Engine's blueprint feature instead of using C++. This means that I will have to make my project using both blueprints and C++ as they can both be used in a project.

## The Code Review 
- [Youtube Link To Code Review](https://youtu.be/oa3iN82uB4Y)

## Enhancement One - Software Design and Engineering 
  In this enhancement I created a new gamemode, a main menu screen, two new maps, and a new pickup. The new gamemode that I created is a survival gamemode, where the player has to face waves of enemies and their goal is to survive as long as possible. In the survival gamemode there is the new pickup item; a syringe. This doubles the player's movement speed for 6 seconds allowing them to outspeed the enemies. When the survival gamemode starts there are two possible maps for the player to get, which is randomly selected.
  
  This enhancement ended up being much more work than I expected and I struggled to get it all complete within the timeframe. Making the enhancements proved to be a much bigger challenge than I had anticipated. When going into this I expected the blueprints to be more compatible with C++ than it turned out to be. Blueprints can access the C++ code, but the C++ cannot access the blueprints. Since all of the original game was made using blueprints I needed to convert some of the blueprints into C++ and link them to make them a sort of hybrid where the blueprint is a child of the C++ class. This allows the bleuprint to call all of the C++ class's functions. I have also run into the issue of there being very little documentation for Unreal Engine’s C++ code and also few guides or videos online for it too. This has caused me to stumble in figuring out how to write the code that I need and caused these enhancements take a lot more time and effort than I expected.

- [Enhancement One Repository](https://github.com/eboucher21/CS-499-Enhancement-One-Evan-Boucher)

## Enhancement Two - Algorithms and Data Structures 
  The second enhancement introduces a new enemy type; the turret. This turret functions very differently from the normal enemies that are currently in the game, it does not move and cannot be killed. The turret is a stationary obstacle that forces the player to limit their active area, or to not stay still when in the turrets sight range. The turret automatically targets and shoots at the player if they walk in its sight range and will stop shooting if they leave the range. To create the turret I had to create an algorithm that dictates the turret's AI behavior. This algorithm searches for any objects that overlap with the turrets sight range, and checks if it is a player object. If it is a player then it faces and shoots at it, otherwise it will ignore it. Once the player leaves the sight range it will stop shooting and becomes inactive again.
  
  Most of my time in this enhancment was in bug-fixing and testing. The main challenge I ran into was not creating the turret's functionality, but instead spawning the turrets at the correct time and place while still having them target the player. I ran into issues where the turrets would spawn on the wrong waves, occasionly spawn on top of each other, and also not being to target the player from on top of the walls and cubes they were stationed on. 

- [Enhancement Two Repository](https://github.com/eboucher21/CS-499-Enhancement-Two-Evan-Boucher)

## Enhancement Three - Databases
  For the third enhancement I added database interaction in the form of a user login screen and a way to store and view all previous survival gamemode scores. This allows the player to create a new account and login with that account to play the game, and each attempt at the survival gamemode will be saved to this database by the user's account. This was done using a MySQL database that is hosted on a free Clever Cloud server. I also made a change to the arena game mode that now displays the players username on the scoreboard instead of the default name that was part of the original artifact. Being able to see past scores give more immsersion to the player and lets them see if they are improving at the game, and will give reason to continue to play the game.
  
  Most of the difficulty when working on this enhancement was in using Unreal Engine's tools to do what I need. Creating and using the databases was very simple, but being able to use that data on screen was difficult. Being able to add each of the past game scores on screen took multiple attempts as the ways to generatively add text on screen is not the most intuitive in Unreal Engine.

- [Enhancement Three Repository](https://github.com/eboucher21/CS-499-Enhancement-Three-Evan-Boucher)

## Game Download
- [Download Game Here](https://drive.google.com/file/d/1dP0vr011IjWT9NcxDnDONSZDmBiezICN/view?usp=sharing)
