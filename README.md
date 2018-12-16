# Objective-C-Trick
This repository contain some of great tricks for Objective-C language i've learn in great repository and documents.

## Clang

### Warning message

1) For preventing Clang to show warning messages:

```objective-c
#pragma clang diagnostic push
#pragma clang diagnostic ignored "-Warc-performSelector-leaks"

// Put your code here, For example you want to use reflection to get value of a system library.
// Adjust library for get AdevertisingId use `clang diagnostic` preprocessor code.

#pragma clang diagnostic pop
```

Example of this code in [Adjust install tracker library](https://github.com/adjust/ios_sdk/blob/ace81b8fafeb66285c51dac19562eef03bda94d4/Adjust/ADJAdditions/UIDevice%2BADJAdditions.m#L36-L52)

