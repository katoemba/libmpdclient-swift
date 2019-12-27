# libmpdclient-swift

This is a variant of libmpdclient for use inside a swift application. It's functionally the same as [libmpdclient](https://github.com/MusicPlayerDaemon/libmpdclient),
with changes to the directory structure to turn it into a swift package.

## Requirements

* Xcode 11
* Swift 5.0

## Installation

libmpdclient-swift doesn't contain any external dependencies.

Currently only build and usage via swift package manager is supported:

### [Swift Package Manager](https://github.com/apple/swift-package-manager)

The easiest way to add the library is directly from within XCode (11). Alternatively you can create a `Package.swift` file. 

```swift
// swift-tools-version:5.0

import PackageDescription

let package = Package(
  name: "MyProject",
  dependencies: [
  .package(url: "https://github.com/katoemba/libmpdclient-swift.git", from: "0.21.17")
  ],
  targets: [
    .target(name: "MyProject", dependencies: ["libmpdclient"])
  ]
)
```

