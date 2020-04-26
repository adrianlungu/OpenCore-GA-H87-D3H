![](https://i.imgur.com/8bGkiIp.jpg)

**Caution**: Parts of this is still a WIP. Some things may not work as expected. 

# GA-H87-D3H running on OpenCore 0.5.7 (High Sierra)

Just managed to upgrade my hackintosh to **High Sierra** and switch from **Clover** to **OpenCore 0.5.7**.

*(can't go further than High Sierra right now since I'm running on a GTX1060; rip web drivers)​*

## System Specs

- Motherboard: Gigabyte GA-H87-D3H
- CPU: Intel i7 4770k
- GPU: Gigabyte GTX 1060

## BIOS Settings

- Bios Version: F10

### BIOS Features

- FastBoot - Disabled
- Limit CPUID Maximum - Disabled
- Execute Disable Bit - Enabled
- Intel Virtualization Tech - Enabled
- Intel TXT Support - Disabled
- VT-d - Disabled
- Windows 8 Features - OtherOS ~~Windows 8~~ *(Booting would result in Black Screen if the HDMI port was being used with the Windows 8 option; works with OtherOS; has to do with CSM)*
- ~~CSM Support - Never~~
- Network Stack - Disabled

### Peripherals

- Initial Display Output - PCIe 1
- PCH Lan Controller - Enabled
- XHCI Mode - Auto
- Audio Controller - Auto
- Intel Processor Graphics - Disabled
- Intel Rapid Start - Disabled
- Legacy USB - Disabled
- XHCI Hand-off - Enabled
- EHCI Hand-off - Enabled

## What's Working

So far I've only tested the installation process, booting, Nvidia Web Drivers and a few other things and they're all working properly. I'll update the list after further testing.

- [x] Installation
- [x] Booting
- [x] GPU / Nvidia Web Drivers
- [x] Bootcamp
- [x] Sleep
- [ ] Audio - Not sure - I use an USB Audio Card

## How can I use this ?

You can just use the EFI folder in the repository as is to boot either a High Sierra installation disk or boot into your existing Mac installation. 

Do test using an USB stick before overwriting any existing Clover/OpenCore installation as issues could occur. 

If you find a better configuration for these specs, feel free to make a pull request or open an issue!

## Special Thanks To

- Apple for MacOS
- The OpenCore team
- InsanelyMac for a ton of helpful resources
- The InsanelyHack Discord community for help and support
- [The OpenCore Vanilla Desktop Guide](https://khronokernel-2.gitbook.io/opencore-vanilla-desktop-guide/)
