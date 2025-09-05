# ZMK Corne Keyboard Layout
- Corne 6 column
- Controller: nice!nano v2 + nice!view (for both left and right keyboard)
- Dongle: Seed Xiao nRF52840


## Installing Firmware

Whether you built it yourself or downloaded my prebuilt firmware, it should
contain the following files:

For the Dongle (XIAO):

- xiao_dongle.uf2
- xiao_reset_settings.uf2

For Keyboard (Corne):

- nano_corne_left.uf2
- nano_corne_right.uf2
- nano_reset_settings.uf2

> The `*_reset_settings.uf2` file is used to clear persistent settings like
> default layers, BLE pairings, and other saved data that may remain after
> repeatedly flashing new firmware.

### Steps

1. Plug in your XIAO dongle to your computer.
2. Double-press the small button on the XIAO to enter bootloader mode.
3. Copy `xiao_reset_settings.uf2` to the XIAO's root folder. (Optional, but
   recommended to ensure a clean slate.)
4. You’ll see an error after flashing—this is normal. Unplug and replug the
   XIAO.
5. Double-press the button again to re-enter bootloader mode.
6. Copy `xiao_dongle.uf2` to the root folder of the XIAO.
7. Wait for the error, then unplug the XIAO dongle. Done flashing the dongle for
   now.
8. Plug in your left Corne keyboard (it doesn't need to be turned on).
9. Double-press the side button to enter bootloader mode.
10. Copy `nano_reset_settings.uf2` to the keyboard's root folder.
11. After the error appears, unplug and replug the keyboard.
12. Double-press the button again to go back into bootloader mode.
13. Copy `nano_corne_left.uf2` to the device. (Make sure to use the correct left
    firmware!)
14. Unplug after the error, then repeat steps 8–13 for your right Corne using
    `nano_corne_right.uf2.`
15. Plug your XIAO dongle back in to your computer.
16. Turn on both sides of your keyboard. Enjoy!
