OSXNavigationController
=======================

Based on the idea of iOS Navigation Controller

###How to use:

####1) Your controller should be a CODBaseViewController Class

```objective-c 
@interface YOURCUSTOM_SUBCLASS : CODBaseViewController
```

####2) Set up your App Delegate

```objective-c
self.navigationController = [[CODNavigationController alloc]initWithRootViewController:YOURCONTROLLER_INSTANCE];
self.window.contentViewController = self.navigationController;
```
####3) How to pop/push

```objective-c
  //Push
    [self.navigationController pushViewController:YOUR_NEW_VC animated:ANIMATE];
  //Pop
    [self.navigationController popViewControllerAnimated:ANIMATE];
```
    
####TODO list:
 Push/Pop: Resize window to the previous/next view controller (now is fixed)

