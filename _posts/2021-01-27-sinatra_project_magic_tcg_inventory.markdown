---
layout: post
title:      "Sinatra Project: Magic TCG inventory"
date:       2021-01-27 06:06:34 +0000
permalink:  sinatra_project_magic_tcg_inventory
---


The Sinatra portfolio project was to design a website that manages content for the users. In deciding what to base my project on I was hoping to find something with multiple models I could design and some interaction between the models, allowing me to get experience working with these relationships in interesting and complicated ways. I decided on doing an inventory system for Magic the Gathering cards and decks. In this system a user can view all of the cards that are currently legal in Magic standard, add any cards they want from that list to their collection and create decks and use cards to build those decks. One important note is that the cards added to the decks and to the collection do not take from the same list. This is to simulate the idea that someone could have something they are working towards making but dont have all of the copies yet, the deck view shows the number of cards of a certain type go in the deck compared to the number of copies of that card you own. 

# Managing routes in complex situations
While building this project there were a few situations I found that the usual Sinatra routing might not be the ideal choice. For example, when adding a new card to your collection, normally you would go to the show page for that card. However there were a couple reasons I thought this would not be ideal in this case. First of all, adding the card to your collection is often a situation where you own the card, looking at the card show page is not giving you that much information. Also, I did not implement any methods of batch adding cards and a lot of times I imagine people would be either entering their collection for the first time or getting a bunch of new cards and thus it would be tedious to have renavigate to the new card page each time. For this reason I chose to have the cards post action re-route to card/new assuming there is a good chance the user has additional cards to input. The nav bar really helps users who might have a bunch of different patterns for editing their collection easily go where they need. 
