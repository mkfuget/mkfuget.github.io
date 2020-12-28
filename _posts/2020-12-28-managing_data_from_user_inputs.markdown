---
layout: post
title:      "Managing Data From User Inputs"
date:       2020-12-28 23:22:57 +0000
permalink:  managing_data_from_user_inputs
---


When starting the Command Line Interface Gem project I started by looking into options for good sources of data to scrape off of the internet. Originally I was looking at pulling sources for vacation destinations, but I felt that most of the sources I looked at were lacking a good amount of data to use for the project. I thought about some different options and ended up putting together a program that pulls NFL stats. This was ideal because there was a large amount of data to work with and it was available in easily accessible table elements. Part of my goal for this project was to include some methods of manipulating the data throught the command line in addition to pulling descriptions from a list, and I thought using football stats to filter out players who didnt meet certain conditions and sort them based on the given attribute would be an effective way to do this. 

# Imprecise Data Entry and Categories
Almost immediatley when parsing throught the data available I noticed a few problems with the data set that I would have to navigate my way around. First of all, lots of table entries would be missing or have inconsistent entries. The position entry had the most obvious issues, a lot of different entries were either capitalized or not capitalized and some had random / characters. This was easy enought to standardize the out the irregularities but there were other problems that were harder to deal with. An example of a use case I was looking at was to take all of the linebackers in a given year with more than 10 sacks and display them sorted with the highest sacks showing first. The immediate issue I ran into was that linebacker was not a category given to any player in their database. They would show up as one of the following MLB (Middle Linebacker) OLB (Outside Linebacker) or ILB (Inside Linebacker). You could either put all of those in the category of linebacker or have the program respond to a call of linebacker by taking all players from all three categories, but ultimately I felt that it was better to leave them in their own categories. Even though it is common place to think of all three of these as the same position, if you look at it from team to team you will find that players in these categories often have very different roles which would make lumping them all into one category imprecise. 

Ultimately this project taught me that any data analysis tools can only work as well as the data they have is available, and that categorizing different parts of data can require balancing how big your groupings of data are with how different the data is inside wach category. 
