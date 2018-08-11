---
day: '129'
title: Solidity Changes
date: '2018-08-11T11:48:47-07:00'
tags:
  - 100daysofcode
  - solidity
  - ethereum
  - smart contracts
  - javascript
categories: code
weight: 0
---
# Progress

Fixed a couple of warnings while typing in my code into Remix. The instructor warned that things in the Ethereum world are still evolving, and change a lot. 

<hr>

## **`keccak256()`** method
> ```
> Warning: This function only accepts a single ”bytes“ argument. Please use ”abi.encodePacked(…)"
> ```

When creating a **`keccac256`** hash, the function parameters must be wrapped in **`abi.encode()`** now. [This SO answer](https://ethereum.stackexchange.com/a/51008/44392) helped.

<hr>

## Cast **`this`** to `**address**`

> ```
> Warning: Using contract member “balance” inherited from the address type is deprecated
> ```

I had to cast **`this`** to an **`address`** type to get the **`balance`** off it. [SO answer](https://ethereum.stackexchange.com/a/42332/44392)

<hr>

# Thoughts
I'm glad that I was able to fix the warnings on my own. The code in the lectures had the previous ways, but I researched and found solutions on Stack Overflow.

# Links
- [Warning: This function only accepts a single ”bytes“ argument. Please use ”abi.encodePacked(…)](https://ethereum.stackexchange.com/a/51008/44392)
- [Warning: Using contract member “balance” inherited from the address type is deprecated](https://ethereum.stackexchange.com/a/42332/44392)
