<p align="center"><img src="https://raw.githubusercontent.com/nahive/Doppelganger-Swift/master/Screenshot_bad.gif" alt="bad ux" style="max-width:100%;" width="186px"></p>
<p align="center"> <img src="https://raw.githubusercontent.com/nahive/Doppelganger-Swift/master/Screenshot.gif" alt="good ux" style="max-width:100%;" width="186px"></p>


# Doppelganger-Swift

![Build Version](https://img.shields.io/github/release/nahive/doppelganger-swift.svg)
[![Build Status](https://travis-ci.org/nahive/spotify-notify.png?branch=master)](https://travis-ci.org/nahive/doppelganger-swift)
##### *Inspired by [Doppelganger](https://github.com/Wondermall/Doppelganger) written in Swift*

## Features

- [x] Removes confusion from users when data changes
- [x] Animates moving, inserting and deleting rows/items
- [x] Example
- [ ] Working with sections

[Changelog](https://github.com/nahive/spotify-notify/blob/master/CHANGELOG.md)

## Installation

Doppelganger-Swift is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:
```
    pod "Doppelganger-Swift"
```

## Using

```swift
let oldDataSource = dataSource
dataSource = newDataSource
let diffs = NIArrayDiffUtility.diffForCurrentArray(dataSource, previousArray: oldDataSource)
    
tableView.ni_applyBatchChangesForRows(diffs!, inSection: 0, withRowAnimation: .Right)
```

## Contributing

If you found a **bug**, open an issue.

If you have a **feature** request, open an issue.

If you want to **contribute**, submit a pull request.

## License

The source code is dedicated to the public domain. See the `LICENCE.md` file for
more information.