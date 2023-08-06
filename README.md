# Narsil Keyboard


It's a (pair of?) ZMK powered wireless ergonomic split keyboard.

## Suggested Materials

Below are some of the more important materials for the build. Misc materials not listed.

- choc switches * 46, 47 or 48
- 1N4148 diodes * 48
- EC11 compatible encoder * 0, 1 or 2
- 3.7v LiPo battery * 2
- Seeeduino Xiao BLE (NRF52840) * 2

This board only uses choc-spaced (18x17mm) 1u keycaps because
1. It's really hard to find keycap sets that come with enough 1.5u or 1.25u keys.
2. Thanks to the rise of popularity of ortholinear keyboards it's relatively easy to find good ortho sets and they usually comes with many extra/novelty caps.
3. Your milage may vary but I personally don't think >1u modifiers are necessary.


## Customizing

You might want to make your own keymap instead of using mine(which I guess only make sense to me). You can fork this repository and edit the .keymap file. ZMK utilize Github actions to compile firmwares so upon commit Github will automatically create firmware files with your keymap. You can find it in the actions tab to your repo -> `https://github.com/$your_username/$your_repo_name/actions`

To flash Xiao boards you need only to double click reset(or quickly bridge GND and RESET twice) and it will show up as a flash drive. You can then drop the `.uf2` files that you grabbed from Github to it and it's done.

Please refer to official ZMK documentations for more info.

https://zmk.dev/docs/user-setup

https://zmk.dev/docs/customization

## Credits
ZMK developers!
To rebase to ZMK 3.2, I forked the clavert repo, and modified from there.

