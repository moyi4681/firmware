# RGB板修正版固件

V3固件对源文件的修改

config.h

#define USB_SUSPEND_WAKEUP_DELAY 5000  USB唤醒等待5000ms。

rule.mk

#NO_USB_STARTUP_CHECK = no  启用USB启动初始化识别

#WAIT_FOR_USB = yes    强制等待USB初始化

V1固件对源文件的修改

rule.mk

#NO_USB_STARTUP_CHECK = yes  禁用USB启动初始化识别，这样键盘不会识别开关机重启动作，一直处于工作状态，需要对BIOS设置USB关机断电


