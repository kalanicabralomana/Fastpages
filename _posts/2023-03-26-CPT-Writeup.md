---
toc: true
layout: post
description: CPT Writeup
categories: [markdown]
title: Create Performance Task Tri 2
---

# Writeup - Roulette

## 3.a. Program Purpose and Function

### 3.a.i
This program is a way to test peoples luck and its purpose is to give a user a fun experience and see how they might turn out in a real Casino.

### 3.a.ii
This program prompts a user to insert their username. After they create their our account with their coins they are able to place those coins on squares spanning on a 9x7 board. By placing a coin on a square they have a chance to win that bet once they spin. Once a play spins, a square will be selected and if the selected square is one that is betted their bet will multiply. A user can then load their account later with their amount of coins.

### 3.a.iii
Inputs for the program would be the players username, bets placed, and spinning. The players username can either be loaded or created with respective buttons, while bets are placed on squares and spinning is prompted by a "spin" button. The out puts would display their coin counts after bets and after spins.

## 3.b. Data Abstraction

### 3.b.i
![]({{site.baseurl}}/images/3bi.jpg "https://github.com/fastai/fastpages")

### 3.b.ii
![]({{site.baseurl}}/images/3bii.jpg "https://github.com/fastai/fastpages")

### 3.b.iii.
The variable representing local storage is "user" which populates the collection type through an SQLite Database.

### 3.b.iv.
The data that is being stored in local storage as user represents the number of coins that the user has. This is vital to the functionality of the program as it is able to do mathematical calculations with this data in order to update the user’s coin amount after the user has spun or bet.

### 3.b.v. Managing Complexity
Local storage is an efficient and straightforward way to store and retrieve data in this section of the program, as it allows for easy updates and retrieval. Another approach to achieving the same functionality would involve fetching the user's coin count every time the roulette feature requires an update on the coin amount.

## 3.c. Procedural Abstraction

### 3.c.i
![]({{site.baseurl}}/images/3ci.jpg "https://github.com/fastai/fastpages")

### 3.c.ii
![]({{site.baseurl}}/images/3cii.jpg "https://github.com/fastai/fastpages")

### 3.c.iii.
The procedure here is spinner(). As the name implies, this function is able to return a random integer between there numerical values that are passed into it as parameters. Using that integer it selects the square that matches that integer highlighting it purple if there was no bet. And if the bet was placed it highlights green. Using the bets it will update score according to the bet placed or if there was no bet placed on the square that will be highlighted.

### 3.c.iv Algorithm Implementation
![]({{site.baseurl}}/images/3civ.jpg "https://github.com/fastai/fastpages")
Spinner(), generates an animated sequence of characters that produces a spinner animation on the console. The spinner variable, a list of characters, represents each frame in the animation. Upon calling the function, an infinite while loop is entered, which prints the next character in the spinner list followed by a carriage return character. The carriage return moves the cursor back to the beginning of the line and allows for overwriting of the previously printed character to create the illusion of a rotating spinner. The function prints the last character in the spinner list before resetting the index variable to zero, so the animation restarts from the beginning of the list. The spinner function is a dynamic and interactive example of how Python's built-in functions and constructs can be utilized to create engaging programs that add a creative touch. By calling this function, users can easily add a fun and interactive element to their Python programs.

## 3.d. Testing

### 3.d.i. 
The first call in this function is selecting a random value for the selected squares. When the spinner button is clicked the function generates a random number for a selected square for the user. The second call is to remove the coins from the playing board and change the background color of the selected/betted square or non-betted square.

### 3.d.ii.
The conditions tests by the first call are if the player was selected on the certain square the coins may be added to the total. The conditions tests by the second call are if the player didn't selected the certain square

### 3.d.iii.
The results of the first call are if the player placed a bet on the winning square, an alert is displayed with a winning statement and value of coins won. The results of the second call are if the player did not place a bet ont he winning square, an alert is displayed with a losing statement.

[VID](https://drive.google.com/file/d/11HbBr-nPnaBKmJ_vxR5NgpK8T-6P4Mlu/view?usp=sharing)