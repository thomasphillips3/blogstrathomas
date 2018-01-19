---
day: '104'
title: Espresso with React-Native
date: 2018-01-18T09:46:22-08:00
tags:
  - espresso
  - react-native
  - android
  - java
  - javascript
  - 100daysofcode
categories: code
weight: 0
---
# Day 104

## Today's Progress

Added **`accessibilityLabel`** and **`testID`** props to React-Native UI components for phone views

<!--more-->

## Thoughts

As I was going through hell yesterday trying to describe UI elements  in relation to each other using Matchers, I realized how much easier life would be if I could just target elements directly, using an element name or something. [This SO answer](https://stackoverflow.com/a/41678992/270847) says to add **`accessibilityLabel`** and **`testID`** props to React-Native UI components. **`accessibilityLabel`** shows up as **`content-desc`** in Android Hierarchy Viewer. This will make writing automation much easier, and ultimately benefit the project overall.

## Links

* [Automated UI Testing with React Native on iOS](http://blog.xebia.com/automated-ui-testing-with-react-native-on-ios/)
* [Accessibility (React-Native Docs)](https://facebook.github.io/react-native/docs/accessibility.html)
* [Components, Props and State (React VR Docs)](https://facebook.github.io/react-vr/docs/components-props-and-state.html)
* [No ID for my Android UI Testing (SO post)](https://stackoverflow.com/a/41678992/270847)
