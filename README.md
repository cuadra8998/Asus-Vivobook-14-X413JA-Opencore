# Asus-Vivobook-14-X413JA-Opencore
This EFI is for the ASUS Vivobook 14 X413JA (i3-1005G1)

<img width="1424" alt="Screen Shot 2023-06-04 at 5 38 43 PM" src="https://github.com/cuadra8998/Asus-Vivobook-14-X413JA-Opencore/assets/83425771/76207a0e-644e-4316-aa43-9f9867524a7e">

Tested OS's:
- Monterey 12.6.3
- Ventura (Not recommended), but working
- Big Sur
- Catalina
---------------------------------------------------------------------------------------
System Configuration
- CPU: Intel Core i3-1005G1 (Ice Lake)
- Memory: 4GB DDR4 2667Mhz Single Channel
- Display: 1920x1080 FHD IPS Panel
- TouchPad: l2C Precision TouchPad
- Graphics: Intel Iris Plus Graphics G1
- Ports: 1 USB-C 3.2, USB A 3.2, USB A 3.1
---------------------------------------------------------------------------------------
BIOS Configuration:
- Disable Secure Boot
- Disable Network Stack
- SATA Configuration: AHCI
- Everything else can be kept as default
---------------------------------------------------------------------------------------
What's Working
- Graphics Acceleration Full QE/CI
- TouchPad
- Wi-Fi: BCM943224PCIEBT2
- Bluetooth: BCM2070A3
- Brightness Control
- Audio ALC 3246 or ALC 256
- Microphone
- iMessage & Facetime (Now App Store too)
- iCloud Services
- Battery Status
- All USB Ports
- Keyboard
- SD Card Reader (Working with RealtekCardReader kext)
----------------------------------------------------------------------------------------
What's Not Working
- Sleep (macOS issue)
- HDMI Port (Not Supported)
- Camera (Camera doesn't work and shows a black screen when initialized)
----------------------------------------------------------------------------------------
Notes:
- Sleep: Sleep is completely broken as of for now. I'm working on a fix but doesn't look promissing. (Will keep you guys updated)
- TouchPad: Make sure to disable the Force Click & Haptic Feedback option in System Preferences so that your touchpad works properly
- NOTE: This model has CFG-Lock enabled in the BIOS. You would have to disable CFG-Lock before proceeding with the Install. Also note since ASUS doesn't provide a full BIOS Image on their website, you will have to make a BIOS Dump instead using Intel FPTw/ Intel Flash Programming Tool. This will give you native CPU-PM. Instead you can enable Kernel -> Quirks -> AppleCpuPmCfgLock and Kernel -> Quirks -> AppleXcpmCfgLock
- Wi-Fi & Bluetooth: If you still have a Intel Wi-Fi Card, Make sure to delete any BCM related kexts and install AirportItlwm or itlwm. Currently Bluetooth on any non Broadcom chipset is wonky so don't expect much.

That's it have fun!
