CFLAGS = -fobjc-arc -O2

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = Vitality
Vitality_FILES = $(wildcard *.m) ../FLAnimatedImage.m ../FLAnimatedImageView.m
Vitality_INSTALL_PATH = /Library/PreferenceBundles
Vitality_FRAMEWORKS = UIKit
Vitality_PRIVATE_FRAMEWORKS = Preferences
Vitality_EXTRA_FRAMEWORKS = CepheiPrefs Cephei

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/Vitality.plist$(ECHO_END)
