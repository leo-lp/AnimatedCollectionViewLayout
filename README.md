# AnimatedCollectionViewLayout

[![CI Status](http://img.shields.io/travis/KelvinJin/AnimatedCollectionViewLayout.svg?style=flat)](https://travis-ci.org/KelvinJin/AnimatedCollectionViewLayout)
[![Version](https://img.shields.io/cocoapods/v/AnimatedCollectionViewLayout.svg?style=flat)](https://cocoapods.org/pods/AnimatedCollectionViewLayout)
[![License](https://img.shields.io/cocoapods/l/AnimatedCollectionViewLayout.svg?style=flat)](https://cocoapods.org/pods/AnimatedCollectionViewLayout)
[![Platform](https://img.shields.io/cocoapods/p/AnimatedCollectionViewLayout.svg?style=flat)](https://cocoapods.org/pods/AnimatedCollectionViewLayout)
[![Carthage compatible](https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat)](https://github.com/Carthage/Carthage)

<table>
<tr>
<th>Parallex</th>
<th>ZoomInOut</th>
<th>RotateInOut</th>
<th>Cards</th>
</tr>
<tr>
<td><img src="http://i.imgur.com/v8JuRYj.gif"/></td>
<td><img src="http://i.imgur.com/lLooXQ7.gif"/></td>
<td><img src="http://i.imgur.com/lCNh5mg.gif"/></td>
<td><img src="http://i.imgur.com/joA1emB.gif"/></td>
</tr>
<tr>
<th>CrossFade</th>
<th>Cube</th>
<th>Page</th>
<th></th>
</tr>
<tr>
<td><img src="http://i.imgur.com/U1hOKYo.gif"/></td>
<td><img src="http://i.imgur.com/897mcdm.gif"/></td>
<td><img src="http://i.imgur.com/HRcvRIV.gif"/></td>
<td></td>
</tr>
</table>

## Example

To run the example project, clone the repo, and start `iOS Example` in Xcode.

## Requirements

- iOS 8.0+

## Installation

### CocoaPods

To integrate AnimatedCollectionViewLayout into your Xcode project using CocoaPods, specify it in your `Podfile`:

```ruby
pod 'AnimatedCollectionViewLayout'
```

## Usage

### Get Started

Import the library where you want to use it. Create a `AnimatedCollectionViewLayout` object, set its `animator` and assign it to your `UICollectionView`.

```swift
import AnimatedCollectionViewLayout

// ...

let layout = AnimatedCollectionViewLayout()
layout.animator = ParallexAttributesAnimator()
collectionView.collectionViewLayout = layout
```

### Customization

Animators implement the protocol `LayoutAttributesAnimator`. Most of them have additionaly parameters that you can tweak the transitions.
You can also write your own animators.

## TODO

- [ ] Support non-paging mode.
- [ ] Support non-full screen items.  
- [ ] Support item selection notifications.

## Author

Jin Wang


## License

AnimatedCollectionViewLayout is available under the MIT license. See the LICENSE file for more info.
