#README.md

These are the "slowclock" Meshtastic variant files for the [Waveshare rp2040-lora](https://www.waveshare.com/rp2040-lora.htm) device. The variant  reduces the CPU speed to 18Mhz to save power. Main drawback is that USB communication does not work at this rate . As such, it is best to install the "normal" rp2040-lora firmware, configure the board and then install the "slowclock" firmware.

**Build instructions**

Clone this repo to your computer and copy the rp2040-lora-slowclock folder to the "variants" folder in your local Meshtastic firmware repo. If you're following the standard Meshtastic build process (VS Code/PlatformIO), set "env:rp2040-lora-slowclock" and run the build.

**Configuring the device**

Meshtastic 2.5.0 just came out, introducing PKI but also deprecating the admin channel in the process. I don't have an Apple device so I have no way of testing remote administration for now. As mentioned in the introduction, best way is to make all the configuration changes while running the "normal" firmware and installing the "slowclock" once done.

**Firmware Binaries**

I will occasionally build binaries - whenever I update my own nodes - and will upload them here.

**Other**

This is my first GitHub project - and I am not a developer - so any feedback and PRs are most welcome.

