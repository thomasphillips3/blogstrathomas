---
day: '129'
title: Testing React with Jest
date: '2018-08-07T18:38:40-07:00'
tags:
  - 100daysofcode
  - javascript
  - react
  - jest
  - mocha
  - automation
categories: code
weight: 0
---
# Progress
Wrote tests for 
- UI components
- behavior
- cookies

# Thoughts
Good experience with Mocha's `describe` and `it` blocks. 

My test actually found a bug in my code. Due to a typo, I wasn't clearing the state properly when I clicked the Delete All Notes button. 

**The Bug**
```javascript
    deleteAllNotes() {
        delete_cookie(cookie_key);
        this.setState = ({ notes: [] });
    }
```

**The Fix**
```javascript
    deleteAllNotes() {
        delete_cookie(cookie_key);
        this.setState({ notes: [] });
    }
```
# Links
- [notetoself](https://github.com/thomasphillips3/notetoself)
