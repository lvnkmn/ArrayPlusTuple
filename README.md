# ArrayPlusTuple

 [![Version](http://img.shields.io/cocoapods/v/ArrayPlusTuple.svg?style=flat)](http://cocoapods.org/pods/Zoomy) [![Platform](http://img.shields.io/cocoapods/p/ArrayPlusTuple.svg?style=flat)](http://cocoapods.org/pods/Zoomy) [![License](http://img.shields.io/cocoapods/l/ArrayPlusTuple.svg?style=flat)](LICENSE)

Simple [extension](https://github.com/lvnkmn/ArrayPlusTuple/blob/develop/ArrayPlusTuple/Classes/Array%2Btuple.swift) that makes creating tuples from arrays a breeze. 

Originally created for [Mock 'N Stub](https://github.com/lvnkmn/Mock-N-stub).

## Setup

Just add:

```Swift
import ArrayPlusTuple
```

to the files where you need tuples from arrays.

## Example

Non optional Any:

```Swift
let tuple = [1, 2, "three"].tuple
```

Typed optional:

```Swift
let tuple = [1, 2, "three"].tuple as? (Int, Int, String)
```

## Larger arrays

ArrayPlusTuple currently supports creating tuples from arrays with up to 24 elements. 

When creating tuples from arrays with more than 24 elements, a warning will be logged and a tuple with the first 24 elements of the array is still returned.

![Screenshot Missing](Art/Warning.png)

### Need support for more elements?

Create a [feature request](https://github.com/lvnkmn/ArrayPlusTuple/issues/new) and it will likely be picked up.

Or [add it yourself](https://github.com/lvnkmn/ArrayPlusTuple/blob/develop/ArrayPlusTuple/Classes/Array%2Btuple.swift) and create a pull request, if the [tests](http://htmlpreview.github.io/?https://github.com/lvnkmn/ArrayPlusTuple/blob/develop/fastlane/test_output/report.html) pass i'll merge it.

## Installation

ArrayPlusTuple is available through [Swift Package Manager](https://swift.org/package-manager/). To install it, simply add it to your project using this repository's URL as explained [here](https://developer.apple.com/documentation/xcode/adding_package_dependencies_to_your_app).

## License

ArrayPlusTuple is available under the MIT license. See the LICENSE file for more info.
