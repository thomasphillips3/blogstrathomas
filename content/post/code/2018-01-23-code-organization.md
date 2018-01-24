---
day: '108'
title: Code Organization
date: 2018-01-23T06:09:09.839Z
categories: code
weight: 0
---
# Day 108

## Today's Progress

Refactored the structure of my tests. I created 3 packages

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

## Links

* [How to write a good commit message](https://juffalow.com/other/write-good-git-commit-message)
