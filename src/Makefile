ARCHS = armv7 arm64
TARGET = iphone:clang:13.0:6.0
APPLICATION_NAME = CocoaTop
ADDITIONAL_OBJCFLAGS = -fobjc-arc # -Wno-deprecated-declarations
CocoaTop_FILES = RootViewController.m SockViewController.m Proc.m ProcArray.m NetArray.m Sock.m Column.m GridCell.m Setup.m SetupColumns.m AppIcon.m TextViewController.m THtmlViewController.m PopupMenuView.m BackButtonHandler.m Compat.m AppDelegate.m main.m
CocoaTop_FRAMEWORKS = UIKit IOKit CoreGraphics MessageUI
CocoaTop_CODESIGN_FLAGS = -Stask.xml
#ifeq ($(TARGET),iphone:clang:7.0)
CocoaTop_RESOURCE_DIRS = res
#endif

include $(THEOS)/makefiles/common.mk
include $(THEOS_MAKE_PATH)/application.mk

SUBPROJECTS = postinst
include $(THEOS_MAKE_PATH)/aggregate.mk

#before-package::
#	@cp .theos/obj/five/CocoaTop.app/CocoaTop .theos/_/Applications/CocoaTop.app/CocoaTop5
#	@cp .theos/obj/six/CocoaTop.app/CocoaTop .theos/_/Applications/CocoaTop.app/CocoaTop6
