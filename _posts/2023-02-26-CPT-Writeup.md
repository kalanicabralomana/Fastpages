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
PIC

### 3.c.ii
PIC

### 3.c.iii.
TXT

### 3.c.iv Algorithm Implementation
TXT

## 3.d. Testing

### 3.d.i. 
The first call
The second call

### 3.d.ii.
The conditions tests by the first call
The conditions tests by the second call

### 3.d.iii.
The results of the first call
The results of the second call