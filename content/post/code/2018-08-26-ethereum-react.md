---
day: '134'
title: Ethereum + React
date: '2018-08-25T20:44:49-07:00'
tags:
  - 100daysofcode
  - ethereum
  - solidity
  - javascript
  - react
categories: code
weight: 0
---
# Progress
- Created a web app to interact with, and display data from, my Lottery Contract. 
- Fixed a build error due to changing dependencies

# Thoughts
I experienced firsthand the nature of open source projects, and how the community reacts to solve issues. I coded and built my project according to the lecture, but kept getting a build error.

> `./node_modules/react-bootstrap/es/DropdownMenu.js Module not found: Can't resolve '@babel/runtime/core-js/array/from'`

[The problem](https://github.com/react-bootstrap/react-bootstrap/issues/3231) was that Babel has removed `core-js` from the runtime package. This showed me the fragility of beta software. 

> <hr>  

> **[Stack Overflow Comment](https://github.com/react-bootstrap/react-bootstrap/issues/3231#issuecomment-414068536)**

> If you're going to use a beta version of babel, pin the version and don't use ^ as there are breaking changes between beta versions.
> <hr>
# Links
- [react-bootstrap Broken with Babel v7.0.0-beta.56](https://github.com/react-bootstrap/react-bootstrap/issues/3231)

```
```
