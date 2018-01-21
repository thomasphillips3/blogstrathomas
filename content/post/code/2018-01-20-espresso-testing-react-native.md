---
day: '106'
title: Espresso Testing React-Native
date: 2018-01-21T03:01:08.294Z
tags:
  - 100daysofcode
  - espresso
  - android
  - java
  - javascript
  - react-native
categories: code
weight: 0
---
# Day 106

## Today's Progress

More UI tests. 

## Thoughts

Tests are kinda flaky now due to the **`wait`** statements. Read about Espresso Idling Resources and got a good understanding of how that works. Espresso normally waits for all asynchronous tasks to finish before running (**`AsyncTasks`**, **`KeyEvents`**, and **`MotionEvents`**). Some UI elements that I'm testing don't fall into those categories, so using an **`IdlingResource`** catches those. 

> An **`IdlingResource`** is an object created by the test author which contains logical condition that must be additionally met in order for app to achieve idle state. 

## Links

* [Espresso Idling Resources](https://developer.android.com/training/testing/espresso/idling-resource.html)
* [Android Espresso doesn't wait for fragments to load (SO post)](https://stackoverflow.com/a/43148880/270847)
* [Wait for it… IdlingResource and ConditionWatcher](https://medium.com/azimolabs/wait-for-it-idlingresource-and-conditionwatcher-602055f32356)
