---
layout: post
title:      "Benefits to Data Management and Algorithms"
date:       2021-06-22 17:39:55 +0000
permalink:  benefits_to_data_management_and_algorithms
---


For my later portfolio projects I tried to use a consistent philosophy of building applications that are interactive and that demonstrate an algorithm visually to a user. This strategy had a lot of benefits that I saw as use for demonstrating skills in a portfolio, however it also saw some surprising benefits to the application as well. For my final project I built an interactive application for Sudoku that allowed users to attempt to solve the puzzle themselves and gave some feedback based on the rules of the puzzle if the move they were attempting was allowed. In addition I designed an algorithm that would sovle the puzzle based on selecting the square with the lowest number of possibilities that would be known by a user and then built a system to animate that on the screen. While this originally was just to demonstrate use of an algorithm, in the end it had of additional benefits that I had not originally thought of.

One of the potential branches I had thought of with this project was to generate a Sudoku puzzle at random. This had a lot of considerations to make including judging the difficulty of the puzzle. The solving algorithm ended up being very useful here as measuring the breadth of search that the solving algorithm goes through. If it solves it in one pass through we can assume the puzzle is easier than if it took several different branches to solve. This concept was very helpful in developing a random puzzle generator and also useful in giving feedback to users making their own puzzles. A robust analsys of the data involved in the system you are designing can have widespread benefits.
