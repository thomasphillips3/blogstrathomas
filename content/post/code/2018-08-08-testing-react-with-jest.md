---
day: '130'
title: Testing React with Jest
date: '2018-08-07T18:38:40-07:00'
tags:
  - 100daysofcode
  - javascript
  - react
  - jest
  - mocha
  - automation
  - ethereum
  - solidity
categories: code
weight: 0
---
# Progress
Wrote tests for 
- UI components
- behavior
- cookies

Learned about test coverage.  
```
thomas[master]$ npm test -- --coverage

> notetoself@0.1.0 test /Users/thomas/workspace/react_testing/notetoself
> react-scripts test --env=jsdom "--coverage"

 PASS  src/components/Note.test.js
 PASS  src/components/App.test.js

Test Suites: 2 passed, 2 total
Tests:       10 passed, 10 total
Snapshots:   0 total
Time:        7.225s
Ran all test suites.
-------------------|----------|----------|----------|----------|-------------------|
File               |  % Stmts | % Branch |  % Funcs |  % Lines | Uncovered Line #s |
-------------------|----------|----------|----------|----------|-------------------|
All files          |     52.5 |        0 |       55 |    65.63 |                   |
 src               |    15.38 |        0 |        0 |       25 |                   |
  index.js         |        0 |        0 |        0 |        0 |         1,2,3,4,6 |
  setupTests.js    |      100 |      100 |      100 |      100 |                   |
  tempPolyfills.js |       50 |      100 |        0 |       50 |                 2 |
 src/components    |    70.37 |      100 |    61.11 |    79.17 |                   |
  App.js           |    78.95 |      100 |       75 |    88.24 |             35,36 |
  Note.js          |       50 |      100 |    33.33 |    57.14 |          18,22,26 |
-------------------|----------|----------|----------|----------|-------------------|
```

# Thoughts
Good experience with [Mocha](https://mochajs.org/)'s `describe` and `it` blocks. 

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
