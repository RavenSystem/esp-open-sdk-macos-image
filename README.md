# esp-open-sdk macOS image file

Compiled esp-open-sdk image to use directly with macOS, without any additional layer.

Source code: https://github.com/pfalcon/esp-open-sdk

[![Donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/ravensystem)

Download from releases, unzip, double click to mount, and add it to PATH:

`PATH=$PATH:/Volumes/esp-open-sdk/esp-open-sdk/xtensa-lx106-elf/bin`

Python and PySerial are needed. To install it, open a Terminal and type:

`sudo easy_install pip`

`pip install pyserial`

* To compile, go to directory where source code is, and type:

`make rebuild`

You can use `-jN` gcc parameter to use `N` CPU threads.
For example, if your CPU has 10 cores with HyperThreading, you can use:

`make -j20 rebuild`
