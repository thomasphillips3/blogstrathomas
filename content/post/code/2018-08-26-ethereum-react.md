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
- Fixed a Solidity warning message in my contract

# Thoughts
I experienced firsthand the nature of open source projects, and how the community reacts to solve issues. I coded and built my project according to the lecture, but kept getting a build error.

> `./node_modules/react-bootstrap/es/DropdownMenu.js Module not found: Can't resolve '@babel/runtime/core-js/array/from'`

[The problem](https://github.com/react-bootstrap/react-bootstrap/issues/3231) was that Babel has removed `core-js` from the runtime package. This showed me the fragility of beta software. 

> <hr>  

> **[Stack Overflow Comment](https://github.com/react-bootstrap/react-bootstrap/issues/3231#issuecomment-414068536)**

> If you're going to use a beta version of babel, pin the version and don't use ^ as there are breaking changes between beta versions.
> <hr>

<hr>

I had a warning in my contract - `provide an error message for require()`. I've been trying to fix warnings as they come up; I usually learn something new about the language when I do. In this instance, I learned how to specify an error message when a `require()`'d method's conditions aren't met. It's as simple as adding the message as a second parameter now. 

**Previous code**
```
require(msg.value > .01 ether);
```

**After `Solidity 0.4.22` update**
```
require(msg.value > .01 ether, "Not enough ether");

```

# Links
- [react-bootstrap Broken with Babel v7.0.0-beta.56](https://github.com/react-bootstrap/react-bootstrap/issues/3231)
- [Solidity: How can we write a error message in “require”?](https://ethereum.stackexchange.com/questions/24969/solidity-how-can-we-write-a-error-message-in-require)
- [Error handling: Assert, Require, Revert and Exceptions](https://solidity.readthedocs.io/en/v0.4.21/control-structures.html?#error-handling-assert-require-revert-and-exceptions)
```
```
