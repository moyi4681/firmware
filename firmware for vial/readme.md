# VIAL固件，兼容VIA，但不是最新版本QMK生成

先使用V3，V3不能修复用V1，刷机前请清EEP，可以用QMKTOOL_BOX清，也可以先拔下键盘，按住ESC插入使其进入刷机模式，这个操作也同时进行了EEP复位。

# V3固件对源文件的修改

config.h文件：

define USB_SUSPEND_WAKEUP_DELAY 5000

rule.mk文件：

NO_USB_STARTUP_CHECK = no

WAIT_FOR_USB = yes

# V1固件对源文件的修改

rule.mk文件：

NO_USB_STARTUP_CHECK = yes  



