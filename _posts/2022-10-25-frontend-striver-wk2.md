---
toc: true
layout: post
description: Striver post for Week 2
categories: [markdown]
title: Implement Quote and Like fetching
author: Kalani Cabral-Omana
show_tags: true
comments: true
---

## Quote

<button onclick="getQuote()">Get new quote</button> # generates random quote from dictionary

<p id="quote"></p> # displays the new quote here

<button type="button" onclick="incrementLikes()">Like</button> # when button pressed adds 1 to like total

<p id="likeCount">N/A</p> # displays like total

<button type="button" onclick="incrementDislikes()">Dislike</button> # when button pressed adds 1 to dislike total

<p id="dislikeCount">N/A</p> # displays dislike total

<script>
    const remote = "https://striver.nighthawkcodescrums.gq";  # identifys the api from the http link
    const quote = document.getElementById("quote");   # defines variable (quote) by the quote that is gernerated by the api
    const likes = document.getElementById("likeCount"); #defines likes by the likecount stored in the api (probably wrong)
    const dislikes = document.getElementById("dislikeCount"); # defines dislikes by the dislikecount stored int eh api (probably worng)
    let currentQuoteID = -1; # ???

    const incrementLikes = async () => {
        if (currentQuoteID === -1) return;
        const { likes: count } = await fetch(remote + "/like", {
            method: "POST",
            headers: { "Content-Type": "application/json" },
            body: JSON.stringify({ id: currentQuoteID }),
        }).then((r) => r.json());
        likes.innerHTML = `${count} likes`;
    };

    const incrementDislikes = async () => {
        if (currentQuoteID === -1) return;
        const { dislikes: count } = await fetch(remote + "/dislike", {
            method: "POST",
            headers: { "Content-Type": "application/json" },
            body: JSON.stringify({ id: currentQuoteID }),
        }).then((r) => r.json());
        dislikes.innerHTML = `${count} dislikes`;
    };

    const getQuote = async () => {
        const res = await fetch(remote + "/quote").then((r) => r.json());
        currentQuoteID = Number.parseInt(Object.keys(res)[0]);
        const currentQuote = res[currentQuoteID];

        likes.innerHTML = `${currentQuote["likes"]} likes`;
        dislikes.innerHTML = `${currentQuote["dislikes"]} likes`;
        quote.innerHTML = currentQuote["quote"];
    };
</script>


