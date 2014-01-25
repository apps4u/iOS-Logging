iOS-Logging
===========

port of The Brenwill Workshop iOS Logging header file to work with Test Flight SDK.

 I could just add a Macro
 #define NSLog(__FORMAT__, ...) TFLog((@"%s [Line %d] " __FORMAT__), __PRETTY_FUNCTION__, __LINE__, ##__VA_ARGS__) 
or 
 #define NSLog(__FORMAT__, ...) TFLog(__FORMAT__, ...)
