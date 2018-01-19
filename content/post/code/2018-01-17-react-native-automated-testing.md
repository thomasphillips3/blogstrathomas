---
day: '102'
title: React Native Automated testing
date: 2018-01-16T21:55:04.134Z
tags:
  - espresso
  - android
  - java
  - 100daysofcode
  - mockito
categories: code
weight: 0
---
# Day 102

## Today's Progress

Created a few more automated tests. Refactored 

<!--more-->

## Thoughts

There was a brief little aside on Static Imports that made me understand it better. I usually let my IDE decide how to import my dependencies, but this was really helpful:

> By adding the **`org.mockito.Mockito.*;`** static import, you can use methods like **`mock()`** directly in your tests. Static imports allow you to call static members, i.e., methods and fields of a class directly without specifying the class.
>
> Using static imports greatly improves the readability of your test code, you should use it.

I also found that as I'm adding new features, I have the urge (and sometimes necessity) to refactor code to accommodate the changes.

## Relevant Links

* [Unit tests with Mockito - Tutorial](http://www.vogella.com/tutorials/Mockito/article.html)
* [ViewMatchers](https://developer.android.com/reference/android/support/test/espresso/matcher/ViewMatchers.html)
