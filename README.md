iOS-ExceptionHandler
====================

This class can be used to catch exception when the app dosen't debug with xcode and use UIAlertview displayed info

This class was made by others, here I just make a note.

Usage:

//  AppDelegate.m
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
#ifndef WS_DEBUG
    InstallUncaughtExceptionHandler();
#endif
    //......
}
