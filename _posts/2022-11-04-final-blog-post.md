---
toc: true
layout: post
description: Notes Final Test
categories: [markdown]
title: Final Blog Post Trimester 1
---
## Reflection:

I thought that this final mc wasn't as bad as I thought it would be. This mc was similar to the practice mc quizzes that are college boards and had similar structured questions. 
Questions Missed:8, 11, 28, 30, 45

## Question 8:
![]({{site.baseurl}}/images/q8 csp.png "https://github.com/fastai/fastpages")
- The procedure does not interchange the values of j and k. Rather, it returns a new list with the values at indices j and k interchanged. 

## Question 11
![]({{site.baseurl}}/images/q11 csp.png "https://github.com/fastai/fastpages")
- The inner loop iterates from index j + 1 to the end of the list, so each element is only compared with the elements that follow it.

## Question 28
![]({{site.baseurl}}/images/q28 csp.png "https://github.com/fastai/fastpages")
- This code segment incorrectly charges customers who use more than 25 units of electricity. These customers are charged $7 per unit for all units, when they should be charged this rate only for the number of units above 25. For examples, if a customer used 32 units of electricity, they should be charged $5 for the first 25 and $7 for the additional 7 units (32 – 25 = 7 units), for a total charge of $174. This code segment would incorrectly charge the customer $224 for the 32 units.

## Question 30
![]({{site.baseurl}}/images/q30 csp.png "https://github.com/fastai/fastpages")
- Introducing a list to a program makes it more likely that the program will attempt to access an index beyond the length of the list, not less likely.

## Question 45
![]({{site.baseurl}}/images/q45 csp.png "https://github.com/fastai/fastpages")
- The code segment iterates through each element in the list, incrementing count1 for each positive value and incrementing count2 otherwise. There are two positive values and three nonpositive values in the list.
