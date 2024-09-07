#README.md

These are the "slowclock" Meshtastic variant files for the [Waveshare rp2040-lora](https://www.waveshare.com/rp2040-lora.htm) device. The variant  reduces the CPU speed to 18Mhz to save power. Main drawback is that USB communication does not work at this rate. As such, it is best to install the "normal" rp2040-lora firmware, configure the board and then install the "slowclock" firmware.


**Build instructions**

Clone this repo to your computer and copy the rp2040-lora-slowclock folder to the "variants" folder in your local Meshtastic firmware repo. If you're following the standard Meshtastic build process (VS Code/PlatformIO), set "env:rp2040-lora-slowclock" and run the build.


**Initial Configuration**

As mentioned in the introduction, best way to set up is to make all the configuration changes while running the "normal" firmware  and installing the "slowclock" once the device is set up to your liking. If you are going to run a pre-2.5 "slowclock" firmware, then set up an "admin" channel during your initial configuration to let you manage the device once you install the "slowclock" variant. 

**Remote Configuration**

Tech Previews for Meshtastic 2.5.0 have been coming out, introducing PKI but also deprecating the "admin" channel in the process. I don't have an Apple device so I can't test remote administration for now on the Tech Previews. If you're running a pre-2.5 version then set up an "admin" channel that will allow you to manage the "slowclock" device from another Meshtastic node that shares the "admin" channel.


**Firmware Binaries**

I will occasionally build binaries - whenever I update my own nodes - and will upload them here. For now I have provided the 2.4.2 (Beta), 2.4.3 (Alpha Hotfix) and the 2.5.0 Tech Preview binaries. I can build an older version on request.


**Other**

This is my first GitHub project - and I am not a developer - so any feedback and PRs are most welcome.

