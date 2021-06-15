# VIA 固件，不兼容VIAL

# 请注意不要将JSON文件当成固件使用（DO NOT use json file as firmware）

kbd67mkiirgb_v3，dz65rgb_v3, bellargb，bellargb_iso和boop65rgb需要在via里导入json后使用，具体操作方法是打开VIA软件后，点击左上角的File---选择Import Keymap---选择对应的JSON文件。

因网络或电脑设置导致VIA无法加载键盘的情况也可以通过手工导入JSON文件来解决。

重启唤醒不识别的问题先使用V3，V3不能修复用V1，V1相对于V3在confg.h文件设置了 #define NO_USB_STARTUP_CHECK  刷机前请清EEP，可以用QMKTOOL_BOX清，也可以先拔下键盘，按住ESC插入使其进入刷机模式，这个操作也同时进行了EEP复位。

# VIA firmware, not compatible with VIAL

# Please do not use JSON file as firmware

kbd67mkiirgb_ v3，dz65rgb_ v3, bellargb，bellargb_ ISO and booP65rgb need to be used after importing JSON into via. The specific operation method is to open via software, click "file" -- select "import keymap" -- select the corresponding JSON file in the upper left corner.

If via can't auto load the keyboard, which can also be solved by manually importing the JSON file.

V1 add ##define NO_USB_STARTUP_CHECK in config.h file to fix Unresponsive after boot, if V3 can't fix it. Pls clear eeprom before reflash a new firmware.