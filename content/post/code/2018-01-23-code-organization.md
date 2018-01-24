---
day: '108'
title: Code Organization
date: 2018-01-23T06:09:09.839Z
tags:
  - 100daysofcode
  - javascript
  - react-native
  - java
  - espresso
  - qa
  - automation testing
categories: code
weight: 0
---
# Day 108

## Today's Progress

Refactored the structure of my tests. I created 3 packages:

```
pages  --->  Classes that represent pages in the app, and helper methods to validate their elements.
```

```
tests  --->  Classes that implement utils and page actions to implement test scenarios.
```

```
utils  --->  Tools to help navigate and interact with the UI
```

## Thoughts

Focusing on clean, readable code lately. The blog post [How to write a good commit message](https://juffalow.com/other/write-good-git-commit-message) was really helpful. The comments section has interesting (opposing) viewpoints. Lots of information from both points of view - write good commit messages, but use PRs to fully describe the overall picture.

I'm enjoying building the test infrastructure to be built upon as the app grows. Keeping an eye on the future allows me to put into practice all of the good coding habits I've learned and heard along the way, and see what does and doesn't work for me, and why. I'm enjoying learning as I progress, and building a dope foundation for the test codebase. 

## Links

* [How to write a good commit message](https://juffalow.com/other/write-good-git-commit-message)
