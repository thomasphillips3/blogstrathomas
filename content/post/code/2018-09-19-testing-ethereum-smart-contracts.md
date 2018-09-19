---
day: '137'
title: Testing Ethereum Smart Contracts
date: '2018-09-19T14:43:07-07:00'
tags:
  - 100daysofcode
  - ethereum
  - solidity
  - smart contracts
  - javascript
  - mocha
  - testing
  - automation
categories: code
weight: 0
---
# Progress
Wrote some unit tests for the Campaign smart contract. 

# Thoughts
I couldn't figure out why I was getting an error when I tried to access a mapping on a struct in my contract. I realized, after 3 days of investigating, what had happened. When writing the test, I realized that the address mapping wasn't public. I made it public, but didn't recompile the contract locally. So the test was looking at the older version of the contract that didn't have the method. I recompiled, and all is well!

# Links
- [Kickstart repo](https://github.com/thomasphillips3/kickstart)
