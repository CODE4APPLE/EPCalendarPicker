# EPCalendarPicker
Colourful calendar component for iOS written in Swift


[![Platform](https://img.shields.io/cocoapods/p/EPCalendarPicker.svg?style=flat)](http://cocoapods.org/pods/EPContactsPicker)
[![Cocoapods Compatible](https://img.shields.io/cocoapods/v/EPCalendarPicker.svg?style=flat)](http://cocoadocs.org/docsets/EPContactsPicker)
[![Swift 2.0](https://img.shields.io/badge/Swift-2.0-orange.svg?style=flat)](https://developer.apple.com/swift/)


Preview
-------
![Single Selection](https://raw.githubusercontent.com/ipraba/EPCalendarPicker/master/Screenshots/Image2.png)    ![Multi Selection](https://raw.githubusercontent.com/ipraba/EPCalendarPicker/master/Screenshots/Image3.png)


Installation
------------

####CocoaPods
EPCalendarPicker is available on CocoaPods. Just add the following to your project Podfile:
```
pod 'EPCalendarPicker'
use_frameworks!
```
####Manual Installation

Just drag and drop the `EPCalendarPicker` folder into your project

Features
--------

EPcalendarPicker provides lot of features which lets you customize the picker

1. Single selection and multiselection option
2. Customize the colors of teh dates in the picker
3. Today Indication and Scrolling to today
4. Delegates that return the selected dates
5. Ability to set the starting and ending year of the calendar

Initialization
--------------
You can init the picker as follows

        let calendarPicker = EPCalendarPicker(startYear: 2015, endYear: 2017, multiSelection: true)
        calendarPicker.calendarDelegate = self
        let navigationController = UINavigationController(rootViewController: calendarPicker)
        self.presentViewController(navigationController, animated: true, completion: nil)   

Properties
----------

Name | Description
---- | ---------
**`tintColor`**|`Tintcolor of the navigationBar bar buttons`
**`weekdayTintColor`**|`Weekday title and date color`
**`weekendTintColor`**|`Weekend title and date color`
**`todayTintColor`**|`Today bar button the today's date color`
**`dateSelectionColor`**|`Selected date color`
**`monthTitleColor`**|`Month title color`
**`multiSelectEnabled`**|`Boolan value indicating whether multiselection enabled or not`
**`calendarDelegate`**|`Delegate`
**`startYear`**|`Starting year of the calendar`
**`endYear`**|`Ending year of the calendar`



Delegates
---------
EPCalendarPicker provides you three delegates for getting the callbacks on the picker

    optional    func epCalendarPicker(_: EPCalendarPicker, didCancel error : NSError)
    optional    func epCalendarPicker(_: EPCalendarPicker, didSelectDate date : NSDate)
    optional    func epCalendarPicker(_: EPCalendarPicker, didSelectMultipleDate dates : [NSDate])

License
-------
EPContactsPicker is available under the MIT license. See the [LICENSE](https://github.com/ipraba/EPContactsPicker/blob/master/LICENSE) file for more info.

Contributors
------------
[@ipraba](https://github.com/ipraba)


