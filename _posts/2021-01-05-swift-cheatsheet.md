---
title: Swift Cheatsheet
image:
  path: /images/general-banner-1.jpg
  thumbnail: /images/general-banner-1.jpg
excerpt: "Swift Cheatsheet with short code snippets"
last_modified_at: 2017-03-09T10:27:01-05:00
categories: ios
tags: 
  - swift
  - ios
---

The post covers basics of Swift progrmaming based on multiple resources. The references are listed at the end.

## Naming Convention
Variable and Global Constants: `lowerCamelCase`

## Constant, Variable, and Type
Constant: `let`
Variable: `var`
Type Declaration: `var name : type = val`

In Swift, type declaration is optional.

## Collection
Array
TODO: cover `reduce`, `filter`, `drop`

```swift
var intArray: [Int] = [1, 2, 3]

// Array for Multiple Types
var anyArray: [Any] = [1,2, "three"]

// Type casting
var anyArray = [1,2,"three"] as [Any]
var emptyArray: [Int] = []
var emptyArray2 = [Int]()

// Slicing
intArray[1...2] // [2, 3]
```

Dictionary
```swift
var myDict: [String:String] = ["key1": "val1"]
var emptyDict: [String:String] = [:]
var emptyDict2 = [String:String]()
```

Set
```swift
var mySet: Set<Int> = [1,2,3]
var mySet2 = Set<Int>([2,3,4])
var emptySet = Set<Int>()

// insert
mySet.insert(10)
// union returns Set
let u = mySet.union(mySet2)
// sorted returns Array
let s = u.sorted()
```

## Loop
Note that `1..<=10` is an invalid syntax.
```swift
for i in 1..<10 {
    print(i)
}
for _ in 1..<10 {
    print("Hello World")
}
```

## TODO
1. Optional
2. Function
3. Closure
4. Struct
5. Protocol


## References
1. https://devxoul.gitbooks.io/ios-with-swift-in-40-hours/content/
2. https://velog.io/@wimes/2019-11-01-2111-작성됨-3zk2g3ey9k
