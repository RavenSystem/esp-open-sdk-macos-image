# esp-open-sdk macOS image file

Compiled esp-open-sdk image to use directly with macOS, without any additional layer.

Source code: https://github.com/pfalcon/esp-open-sdk

[![GitHub download](https://img.shields.io/github/downloads/RavenSystem/esp-open-sdk-macos-image/total.svg)](https://github.com/RavenSystem/esp-open-sdk-macos-image/releases/latest)
[![Donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/ravensystem)

Download from releases, unzip, double click to mount, and add it to PATH:

```shell
export PATH=$PATH:/Volumes/esp-open-sdk/esp-open-sdk/xtensa-lx106-elf/bin
```

Python and ESPTool are needed. To install them, open a Terminal and type:

```shell
python3 -m pip install esptool
```

* To compile, go to directory where source code is, and type:

```shell
make rebuild
```

You can use `-jN` gcc parameter to use `N` CPU threads.
For example, if your CPU has 10 cores with HyperThreading, you can use:

```shell
make -j20 rebuild
```
