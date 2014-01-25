iOS-Logging
===========

port of The Brenwill Workshop iOS Logging header file to work with Test Flight SDK.

 I could just add a Macro
 `#define NSLog(__FORMAT__, ...) TFLog((@"%s [Line %d] " __FORMAT__), __PRETTY_FUNCTION__, __LINE__, ##__VA_ARGS__)`
or 
` #define NSLog(__FORMAT__, ...) TFLog(__FORMAT__, ...)`
Which is what I'm doing now but I wanted to do a but better then that and to make this work with whats to come with TestFlight's FlightPath service for logging in production app metrics.

All pull request are welcome I'm not tring to build a large logging framework its just a small header file using Macros for no CPU overhead of disabled logs and for easy use with current build tools by being controlled by `#define` or compiler flag.


