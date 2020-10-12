# boot-args

This is a simple EFI boot package which will set `boot-args="-no_compat_check"` and then reboot, hopefully on any Mac. (Tested only on one late 2012 x64 Mac so far though.)

To use it:

 - Download `boot-args.zip` from the latest release
 - Unzip it
 - Copy the whole EFI folder into the root of any FAT32 USB drive
 - Reboot your MAC with the USB drive plugged in, while holding down the ALT-Option key
 - You should see a new boot option called `boot-args` (if you're not sure, you could try unplugging and plugging back in the USB drive, to see it disappear and reappear again)
 - Select this boot option to immediately set `boot-args="-no_compat_check"` and reboot

This release is just a [slightly modified](https://github.com/MikeBeaton/big-sur-micropatcher/commit/1437ef24f91d81ad667bfe278f8ba5f56f8b4adb) version of Barry K. Nathan's [setvars](https://github.com/barrykn/big-sur-micropatcher/tree/main/setvars) program from the excellent [big-sur-micropatcher](https://github.com/barrykn/big-sur-micropatcher).
