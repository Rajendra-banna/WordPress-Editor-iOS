🚨 Deprecation Notice: 🚨 As of December 2017 this project has been deprecated and will no longer be updated. The code is here for historical purposes only. 

<p align="center">
<img width=200px height=200px src="https://github.com/wordpress-mobile/AztecEditor-iOS/blob/develop/RepoAssets/aztec.png" alt="Aztec's Logo'"/>
</p>

We encourage you to try [Aztec](https://github.com/wordpress-mobile/AztecEditor-iOS), 
our new, open-source fully native HTML editor.

If you find Aztec is missing some functionality you were relying on from this editor, please file an issue [in the Aztec repo](https://github.com/wordpress-mobile/AztecEditor-iOS/issues).

____


[![Build Status](https://travis-ci.org/wordpress-mobile/WordPress-Editor-iOS.svg?branch=develop)](https://travis-ci.org/wordpress-mobile/WordPress-Editor-iOS)

![WordPress Logo](http://s.w.org/about/images/logos/wordpress-logo-hoz-rgb.png)

# WordPress-Editor-iOS

![WordPress-iOS-Editor Screenshot](https://cldup.com/5I1YePnOWU.png)![WordPress-iOS-Editor Screenshot 2](https://cldup.com/CbNB0dFERt.png)![WordPress-iOS-Editor Screenshot 3](https://cldup.com/o4ZpUjkDxi.png)

## Introduction

The WordPress-Editor-iOS is the text editor used in the [WordPress iOS app](https://github.com/wordpress-mobile/WordPress-iOS) to create and edit pages & posts. In short it's a simple, straightforward way to visually edit HTML.

## How to get started
You can install the editor in your app via [CocoaPods](http://cocoapods.org):

```ruby
platform :ios, '10.0'
pod 'WordPress-iOS-Editor'
```

Or, you can just try out the demo by using the CocoaPods try command:

```ruby
pod try WordPress-iOS-Editor
```

## Requirements

WordPress-iOS-Editor requires iOS 10.0 or higher. It depends on the following Apple frameworks:

* Foundation.framework
* UIKit.framework
* CoreGraphics.framework
* CoreText.framework

and the following CocoaPods:

* [CocoaLumberjack](https://github.com/CocoaLumberjack/CocoaLumberjack)
* [WordPressCom-Analytics-iOS](https://github.com/wordpress-mobile/WordPressCom-Analytics-iOS)

See the [podspec](https://github.com/wordpress-mobile/WordPress-iOS-Editor/blob/develop/WordPress-iOS-Editor.podspec) for more details.

## Usage

There are three things that you need to do in order to use the WordPress-iOS-Editor in your app.

1. Create a ViewController that extends ```WPEditorViewController```

        #import <UIKit/UIKit.h>
        #import <WordPress-iOS-Editor/WPEditorViewController.h>

        @interface WPViewController : WPEditorViewController <WPEditorViewControllerDelegate>

        @end

2. Implement any of the optional ```WPEditorViewControllerDelegate``` [methods](https://github.com/wordpress-mobile/WordPress-iOS-Editor/blob/develop/Classes/WPEditorViewController.h) in your view controller.

3. The ```titleText``` and ```bodyText``` properties can be used to set and get the title and body of the text document.

For more details, you can review the [EditorDemo](https://github.com/wordpress-mobile/WordPress-iOS-Editor/tree/develop/Example) project included in this repo.

## Other Resources

#### Developer blog & Handbook

Blog: [http://make.wordpress.org/mobile](http://make.wordpress.org/mobile)

Handbook: [http://make.wordpress.org/mobile/handbook](http://make.wordpress.org/mobile/handbook)

#### Style guide

[https://github.com/wordpress-mobile/WordPress-iOS/wiki/WordPress-for-iOS-Style-Guide](https://github.com/wordpress-mobile/WordPress-iOS/wiki/WordPress-for-iOS-Style-Guide)

#### To report an issue (for the editor only)

[https://github.com/wordpress-mobile/WordPress-iOS-Editor/issues](https://github.com/wordpress-mobile/WordPress-iOS-Editor/issues)

#### Source Code

GitHub: [https://github.com/wordpress-mobile/WordPress-iOS-Editor](https://github.com/wordpress-mobile/WordPress-iOS-Editor)

#### How to Contribute

[http://make.wordpress.org/mobile/handbook/pathways/ios/how-to-contribute](http://make.wordpress.org/mobile/handbook/pathways/ios/how-to-contribute)

## Attribution

The following projects were used in the WordPress-iOS-Editor codebase:

| Component     | Description   | License  |
| ------------- |:-------------:| -----:|
| [ZSSRichTextEditor](https://github.com/nnhubbard/ZSSRichTextEditor)      | ZSSRichTextEditor is a rich text WYSIWYG Editor for iOS and was the basis for this project.| [MIT](Attribution/ZSSRichTextEditorLicense/LICENSE.txt) |
| [CYRTextView](https://github.com/illyabusigin/CYRTextView)      | CYRTextView is a UITextView subclass that implements a variety of features that are relevant to a syntax or code text view. | [MIT](Attribution/CYRTextViewLicense/LICENSE) |
| [HRColorPicker](https://github.com/hayashi311/Color-Picker-for-iOS)      | Simple color picker for iPhone      |   [BSD](Attribution/HRColorPickerLicense/LICENSE.txt) |
| [jQuery](https://jquery.com)      | jQuery is a fast, small, and feature-rich JavaScript library.      |   [MIT](http://jquery.org/license) |
| [JS Beautifier](https://github.com/einars/js-beautify)      | Makes ugly Javascript pretty      |   [MIT](Attribution/jsBeautifierLicense/LICENSE.txt) |

## License

WordPress-iOS-Editor is available under the GPL license. See the [LICENSE](https://raw.githubusercontent.com/wordpress-mobile/WordPress-iOS-Editor/develop/LICENSE) file for more info.
