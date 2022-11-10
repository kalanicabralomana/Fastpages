---
toc: true
layout: post
description: Notes Final Test
categories: [markdown, Final]
title: Final Blog Post Trimester 1
---
## Reflection:

I thought that this final mc wasn't as bad as I thought it would be. This mc was similar to the practice mc quizzes that are college boards and had similar structured questions. 
Questions Missed:8, 11, 28, 30, 45

## Question 8:
![]({{site.baseurl}}/images/q8 csp.png "https://github.com/fastai/fastpages")
- The procedure does not interchange the values of j and k. Rather, it returns a new list with the values at indices j and k interchanged. 
-Video Notes: Topic is Program Design and Development How is a program developed? Programs are developed with a specific purpose in mind Developers follow specific steps and stick to their plan Sometimes the development is more exploratory than anything, and the steps are dictated by what happens Investigation is an important step in the process Developers must: Determine the requirements of the program Understand the constraints Understand the user concerns and interests How do developers investigate Surveys User testing Interviews Direct observation Developers design program by Brainstorming Storyboarding the program Planning the user experience Laying out the user interface Organizing into modules

## Question 11
![]({{site.baseurl}}/images/q11 csp.png "https://github.com/fastai/fastpages")
- The inner loop iterates from index j + 1 to the end of the list, so each element is only compared with the elements that follow it.

## Question 28
![]({{site.baseurl}}/images/q28 csp.png "https://github.com/fastai/fastpages")
- This code segment incorrectly charges customers who use more than 25 units of electricity. These customers are charged $7 per unit for all units, when they should be charged this rate only for the number of units above 25. For examples, if a customer used 32 units of electricity, they should be charged $5 for the first 25 and $7 for the additional 7 units (32 – 25 = 7 units), for a total charge of $174. This code segment would incorrectly charge the customer $224 for the 32 units.
-Video Notes Topic: Conditionals Algorithm: a finite set of instructions that accomplish a specific task Selection: Given a parameter the algorithm uses its instructions to determine if it needs to return true or false. EX: If statements Evaluates a conditional and return true or false statement

## Question 30
![]({{site.baseurl}}/images/q30 csp.png "https://github.com/fastai/fastpages")
- Introducing a list to a program makes it more likely that the program will attempt to access an index beyond the length of the list, not less likely.
-Video Notes: Topic is Data Abstraction Strings An ordered sequence of characters May contain letters, numbers and all other special characters Ex: Words, phrases, sentences, ID numbers, etc. Lists An ordered sequence of elements Each element is a variable Ex: Playlists of songs, Names of students in a school, contacts in your phone, etc List Index Each element of a string is referenced by an index The index starts at 1

## Question 45
![]({{site.baseurl}}/images/q45 csp.png "https://github.com/fastai/fastpages")
- The code segment iterates through each element in the list, incrementing count1 for each positive value and incrementing count2 otherwise. There are two positive values and three nonpositive values in the list.
