# CocoaTop
CocoaTop: Process Viewer for iOS GUI

Current 64-bit version should work on iOS 10-13, with support for safe area on iPhone X screen, dark mode, and split view on iPad!

Versions prior to 2.0.1 are 32 bit and work on iOS 6-10. They are separated into the **32bit** branch. The **master** branch is intended for new iOS versions, thus it will only support 64-bit builds. Non-relevant code should be removed.

# Crash/reboot issues
If CocoaTop crashes and/or reboots your phone, you should try removing the SUID bit from /Applications/CocoaTop.app/CocoaTop. You can do it via Filza: find the executable file, tap (i), then make sure "Set UID" is unchecked.

# Contributing
Source code is available for everyone to improve. The license is GPL-3, except for the include files in *kern*, *net*, *netinet*, *sys*, and *xpc* folders. These are taken from public Mach kernel code and put here to simplify building. You are free to modify the *About* text (a.k.a. *The Story*) any way you want, but I will appreciate if you keep the "Developers" section up-to-date.

# Building
To build CocoaTop you need:
* Theos (https://github.com/theos/theos), make sure $(THEOS) environment variable points to it.
* Appe iOS SDK (currently version 13.0 is used). Download it from Apple and unpack to theos\sdks\. Also look here: https://github.com/theos/sdks/
* make
* make package

or, you can use XCode.
