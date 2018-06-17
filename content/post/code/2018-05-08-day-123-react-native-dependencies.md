---
day: '123'
title: React Native dependencies
date: '2018-05-08T22:52:18-07:00'
categories: code
weight: 0
---
# Day 123
 
## Today's Progress

Fixed React-Native dependencies in my project. There were 3 issues I had to resolve versioning issues with

* [gms](https://www.android.com/gms/)
* react-native-google-analytics-bridge

## Thoughts

### GMS issue

Had to specify versions in my `android/build.gradle` file

```
configurations.all {
    resolutionStrategy.eachDependency { DependencyResolveDetails details ->
        def requested = details.requested
        if (requested.group == 'com.android.support') {
            if (!requested.name.startsWith("multidex")) {
                details.useVersion '26.0.2'
            }
        }
        
        if (requested.group == 'com.google.android.gms') {
            details.useVersion '12.0.1'
        }
    }
}

subprojects {
    project.ext.'googlePlayServicesVersion' = '12.0.1'
}
```

Google Analytics Bridge issue

There was a `+` in the dependency version (i.e.
