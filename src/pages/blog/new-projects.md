---
layout: "../../layouts/BlogPost.astro"
title: "The Knight's Tour"
description: "A knight's tour"
pubDate: "March 8, 2024"
---

I started a new project with my friend David, one that I have been wanting to do for a while. 
It's a website for us to try and work on the <a href="https://en.wikipedia.org/wiki/Knight%27s_tour">Knight's Tour</a> puzzle.
David is a self taught programmer, and want to learn Rails, so we are doing this project without any JS,
because I wanted to see if I could figure out how to make it interactable but by only using restful routes, 
the convention with Ruby on Rails. I know RoR has great interactivity with stimulus, because I use it a lot
at my job at <a href = "https://backerkit.com" target= "_blank">Backerkit!</a>, but I thought it would be cool
to reinforce my own knowledge of Rails by building this project in this way. 

So far, we've come up with the idea of having each square just be it's own page, and so we've created the Square model, 
which so far just has an id, and x and y coordinates. The square index will just show all of the Squares
that we have in the db, which we will just write a script to create.
After thinking about the problem a little bit, I think we'll want to migrate the data to make it 
such that Square has a couple more fields: 
 - has_knight, to determine whether or not to show the knight on that square
 - has_been_visited, to determine if this square was already clicked on previously
 - color not sure if this one is necessary, we can probably just programatically color the squares on the front end. not sure.

It's fun to have a side project!

