---
day: '114'
title: Testing with Jest
date: 2018-02-04T21:52:29.893Z
tags:
  - 100daysofcode
  - jest
  - javascript
  - react-native
  - testing
  - automation
categories: code
weight: 0
---
# Day 114

## Today's Progress

Created automated tests with Jest

## Thoughts

I have been working on the Android portion of automated tests for the past couple of weeks. I think Jest is the cross-platform way of validating the app from the jump, instead of depending on Espresso for Android, and UI Automation for iOS. 

Building the test projects from scratch gave me some insight on how to better use **`npm`** and **`nvm`**. I had initially tried to run my js from the Terminal, and kept getting permission denied errors. After changing permissions on the files, I realized...I NEVER run JS from Terminal, always in a browser. So I came across [this question on SO](https://stackoverflow.com/a/28756251/270847), which told me to use Node (duh).

The first test was just verifying a sum. For the next one, I was trying to do UI testing with Snapshots. I added a new test, but realized I hadn't added React-Native to the project. I used npm to install it, but I had an old version of node, so the install failed. I used nvm to install the right version of node.

## Links

* [Is it possible to run JavaScript files from the command line?](https://stackoverflow.com/a/28756251/270847)
* [Integration with Existing Apps (React Native)](https://facebook.github.io/react-native/docs/integration-with-existing-apps.html)
* [Jest Getting Started](https://facebook.github.io/jest/docs/en/getting-started.html)
