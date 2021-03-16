---
layout: post
title:      "Path Finding Animations and JS"
date:       2021-03-16 09:33:33 +0000
permalink:  path_finding_animations_and_js
---


When deciding on what kind of project I want to do I wanted to combine algorithm usage, visual effects and user interaction while still feeling unique. I decided on a maze game that will implement pathfinding algorithms and have different squares with special rules. In setting up the classes I decided to have one class that represents a single instance of the maze, containing many cell classes and a single cursor class to track the movement throught the maze and keep important information about the path taken so far. The cells class utilized many child classes for different type of cells, and included all of the logic for what would happen when travelling to that cell. This is important because it allows future new cell designs to be implemented just through the addition of new classes.

When building the visuals of my application I decided to include a layer of abstraction between my data and what was being represented on the screen. This ended up being useful in a lot of cases including designing the path finding algorithms, I was able to utilize methods I had made for the cursor class without those methods being tied to what would happen on screen. 

For animations after some work I decided it would be useful to utilize and existing animations library which after some research I decided on anime.js. This gave a few great benefits to my application, first of all being more visually satisfying animations. While trying a few features on my own using timeout functions, I found that the results I was getting did not look very good. This is because I was drawing animations with a linear progression and that is often not a natural effect for movement, causing the animations to look a little jarring. Anime.js has easy to use tools to work around this and implement a variety of different animation curves. 
