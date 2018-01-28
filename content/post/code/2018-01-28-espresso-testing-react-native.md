---
day: '111'
title: Espresso Testing React-Native
date: 2018-01-28T06:53:43.000Z
tags:
  - 100daysofcode
  - java
  - javascript
  - react-native
  - espresso
  - automation
categories: code
weight: 0
---
# Day 111

## Today's Progress
- Created tablet page objects
- Merged a huge pull request of all my work over the past week back to master. 

## Thoughts
While writing my code today I noticed I was repeating the same few blocks a lot. I was creating classes for each page in the app under test. Each page has **`ViewInteraction`**s for UI components, and methods to validate them.   

[Interfaces](https://docs.oracle.com/javase/tutorial/java/IandI/createinterface.html) would help a lot in this regard. I need to create a `Page` interface, and implement it in all the pages. I wanted to do it today, but the refactor would have taken me off my schedule. 

## Links
- [Interfaces] (https://docs.oracle.com/javase/tutorial/java/IandI/createinterface.html)
