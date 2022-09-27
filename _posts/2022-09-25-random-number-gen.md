---
layout: post
description: Personal Usage of JAva
categories: [code]
title: Random Number Generator
permalink: /randomnum
---

<button type="button" class="btn btn-light" onclick="randomNumber()">Click to Generate Number</button>
  <br>
  <h3 id="Number Generator" href="#">The Number Will Appear Here</h3>
  <script>
    const numberList = [ 
    "1",
    "2",
    "3",
    "4",
    "5",
    "6",
    "7",
    "8",
    "9",
    "10",
    "11",
    "12",
    "13",
    "14",
    "15",
    "16",
    "17",
    "18",
    "19",
    "20"
  ];
    function randomNumber() { 
    var index=Math.floor(Math.random() *numberList.length) 
    document.getElementById("Number Generator").innerHTML = numberList
    [index]
  }
  </script>