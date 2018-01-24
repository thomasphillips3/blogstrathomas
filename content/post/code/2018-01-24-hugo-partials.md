---
day: '109'
title: Hugo Partials
date: 2018-01-23T10:09:09.839Z
tags:
  - 100daysofcode
  - hugo
  - javascript
  - netlify-cms
categories: code
weight: 0
---
# Day 109

## Today's Progress

Added a partial to display panorama photos to my blog.

## Thoughts

This was giving me trouble for a while. I finally decided to check the console in the browser, and saw I was getting a 404 for a file. It was a typo. 

I had the decision to add the partial as an override, or directly to the theme. I chose to add it to the theme, because I think it would be a cool addition. I took care to make sure it was encapsulated properly, so it could be added cleanly. I'm going to test it on my own setup for a while, and make sure it's good before sending a PR to the theme maker. 

## Links

* [Front Matter (Hugo Docs)](https://gohugo.io/content-management/front-matter/)
* [Introduction to Hugo Templating](https://gohugo.io/templates/introduction/) 
* [Panorama Viewer](https://github.com/peachananr/panorama_viewer) 
* [My 100 days of code](https://blogstrathomas.netlify.com/tags/100daysofcode/)
* Puako - (blog post using panorama partial)
