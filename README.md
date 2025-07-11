---
page_type: sample
description: "Demonstrates how to write a HID minidriver using User-Mode Driver Framework (UMDF)."
languages:
- cpp
products:
- windows
- windows-wdk
---

# Description

This driver is intended for Goodix GT9xx I2C touchscreens commonly found in Xiaomi Mi Max 3. It does not contain any firmware upgrading/loading functionality, nor does it support any Xiaomi features.
Based on [my Goodix GT9897T driver](https://github.com/AistopGit/GT9897T-Windows-driver), which is based on https://github.com/Project-Aloha/gtx9886-driver.

# HID Minidriver Sample (UMDF version 2)

The *HID minidriver* sample demonstrates how to write a HID minidriver using User-Mode Driver Framework (UMDF).

The sample demonstrates how to communicate with an HID minidriver from an HID client using a custom-feature item in order to control certain features of the HID minidriver. This is needed since other conventional modes for communicating with a driver, like custom IOCTL or WMI, do not work with the HID minidriver. The sample also is useful in testing the correctness of a HID report descriptor without using a physical device.

## Related topics

[Creating WDF HID Minidrivers](https://docs.microsoft.com/windows-hardware/drivers/wdf/creating-umdf-hid-minidrivers)

[Human Input Devices Design Guide](https://docs.microsoft.com/windows-hardware/drivers/hid/)

[Human Input Devices Reference](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/_hid/)

[UMDF HID Minidriver IOCTLs](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/hidport/)
