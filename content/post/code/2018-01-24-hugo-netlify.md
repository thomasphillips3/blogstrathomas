---
day: '110'
title: Hugo/ Netlify
date: 2018-01-24T09:48:05.082Z
tags:
  - 100daysofcode
  - netlify-cms
  - git
  - hugo
  - javascript
  - github
categories: code
weight: 0
---
# Day 110

## Today's Progress

## Thoughts

I'm having a Git issue with the submodule mapping of my Hugo theme. Here's the [deploy failure](https://app.netlify.com/sites/blogstrathomas/deploys/5a684fa0a1147721e6ed6de3). I have tried the instructions [here](https://stackoverflow.com/a/2161389/270847) and read the [Git submodule docs](https://git-scm.com/docs/gitmodules), but still getting the deploy failure. Could someone please help when you get a min?

```
1:19:33 AM: Preparing Git Reference refs/heads/master
1:19:35 AM: Error checking out submodules: fatal: reference is not a tree: 22dc3630e73918c2cd9981c7bec432df6a781854
Unable to checkout '22dc3630e73918c2cd9981c7bec432df6a781854' in submodule path 'themes/hugo-tracks-theme'
1:19:35 AM: Failing build: Failed to prepare repo
1:19:35 AM: failed during stage 'preparing repo': Error checking out submodules: fatal: reference is not a tree: 22dc3630e73918c2cd9981c7bec432df6a781854
Unable to checkout '22dc3630e73918c2cd9981c7bec432df6a781854' in submodule path 'themes/hugo-tracks-theme'
```

## Links
- [Git submodule docs](https://git-scm.com/docs/gitmodules)
- [Git submodule head 'reference is not a tree' error
](https://stackoverflow.com/a/2161389/270847)
