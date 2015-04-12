# TouchVisualizer

[![Version](https://img.shields.io/cocoapods/v/TouchVisualizer.svg?style=flat)](http://cocoadocs.org/docsets/TouchVisualizer)
[![License](https://img.shields.io/cocoapods/l/TouchVisualizer.svg?style=flat)](http://cocoadocs.org/docsets/TouchVisualizer)
[![Platform](https://img.shields.io/cocoapods/p/TouchVisualizer.svg?style=flat)](http://cocoadocs.org/docsets/TouchVisualizer)

## Let's give a presentation with finger points easily

![Gif](https://github.com/morizotter/TouchVisualizer/blob/master/presentation.gif)

When you give a presentation, your finger points are visible on screen.
- Multiple fingers supported.
- Multiple UIWindows supported.
- You can change colors and images of finger points.

## Installation

> Embedded frameworks require a minimum deployment target of iOS 8.1
> To use TouchVisualizer with a project targeting iOS 8.0 or lower, you must include the TouchVisualizer.swift source file directly in your project.

[CocoaPods](http://cocoapods.org) 0.36 adds supports for Swift and embedded frameworks. You can install it with the following command:

```
$ gem install cocoapods
$ pods --version
```

To install it, simply add the following lines to your Podfile:

```
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.1'

use_frameworks!

pod "TouchVisualizer", '~>1.0.3'
```

## Usage

`import TouchVisualizer` and just write the following line in the `application(application:didFinishLaunchingWithOptions:)` in `AppDelegate`.

```
TouchVisualizer.start()
```

You can change colors and images like this. You can set only color or image.

```
var config = TouchVisualizerConfig()
config.color = UIColor.redColor()
config.image = UIImage(named: "YOUR-IMAGE")
config.showsTimer = true
TouchVisualizer.start(config)
```

You can stop presentation from the app like this.

```
TouchVisualizer.stop()
```

## Requirements

- iOS8.1 or later
- Xcode 6.3

## Author

Naoki Morita, namorit@gmail.com, [page](http://moritanaoki.org)

## License

TouchVisualizer is available under the MIT license. See the LICENSE file for more info.

