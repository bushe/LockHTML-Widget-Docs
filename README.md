# LockHTML-Widget-Docs

Simple documenation on building a native code(Objective C) widget for LockHTML4. NIC template is included for use with [theos](http://github.com/theos/theos)

Contributions welcome!

## Requirements

* Main class must a subclass of UIViewController
* Main class conforms to LockHTMLWidgetViewDelegate
* Widget.bundle is located /Library/Widgets/

### Optional

Below are the optional methods that are available

```objective-c
@protocol LockHTMLWidgetViewDelegate
@optional
-(void)prepareWidgetForNotificationsWithContent:(BOOL)hasContent; //Called when notifications status changed
-(void)handleMenuButtonTap; //Called when menu/home button is pressed
-(void)updateWidgetForScreenStatus:(BOOL)status; //Called when screen is enabled/disabled
@end
```
