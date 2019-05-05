---
day: '138'
title: Build an Android Instsragram Clone
date: '2019-05-05T12:23:50-07:00'
categories: code
weight: 0
---
![null](/img/screen-shot-2019-05-05-at-12.29.55-pm.png)

# Overview

Build an Android photo-sharing app from scratch. Adapted from [The Complete Android P + Java Developer Course](https://www.udemy.com/java-android-complete-guide) on Udemy.

# Steps

## Setup Android Project

* Create a new Android Studio Project with the default settings, except:
  * **Language:** `Java`
  * **Minimum API Level:** `API 16: Android 4.4 (Kit Kat)`
  * `Use androidx.* artifacts`
* Refactor MainActivity to SignUpActivity

![null](/img/screen-shot-2019-05-05-at-12.52.40-pm.png)

## Set up Parse Server

* Go to www.back4app.com
* Create a new app 

## Add Parse Server to Android project

* Add a new `App` class to the  application package with superclass `android.app.Application`
![null](/img/screen-shot-2019-05-05-at-2.49.03-pm.png)
* In the `AndroidManifest.xml` file, add `android:name=".App"` attribute to the `application` tag. 
* Add the dependency's repo to the project. In the `repositories{}` block in the `build.gradle (Module:app)` file, add 

  ```maven { url "https://jitbpack.io" }```
* Add the library to the project. In the `dependencies{}` block in the project `build.gradle` file, add 

  ```implementation "com.github.parse-community.Parse-SDK-Android:parse:latest.version.here"``` 
  
  Make sure to replace with the [latest version](https://jitpack.io/#parse-community/Parse-SDK-Android). 
* Run `gradle sync` and verify there are no issues.

## Connect Android app to Parse Server
