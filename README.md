# Asus-Vivobook-14-X413JA-Opencore
This EFI is for the ASUS Vivobook 14 X413JA (i3-1005G1)
![Screen Shot 2021-11-05 at 10 58 03 PM](https://user-images.githubusercontent.com/83425771/140599700-4fa64d7a-13b1-468c-9df5-f462b1171bbc.png)
System Configuration
- CPU: Intel Core i3-1005G1 (Ice Lake)
- Memory: 4GB DDR4 2667Mhz Single Channel
- Display: 1920x1080 FHD IPS Panel
- TouchPad: l2C Precision TouchPad
- Graphics: Intel Iris Plus Graphics G1
- Power: Lithium Battery
- Ports: 1 USB C, USB A 3.1, USB A 2.0
---------------------------------------------------------------------------------------
What's Working
- Graphics Acceleration Full QE/CI
- TouchPad
- Brightness Control
- Audio ALC 3246
- Microphone
- iMessage & Facetime
- iCloud Services
- Battery Status
- All USB Ports
- Keyboard
----------------------------------------------------------------------------------------
What's Not Working
- SD Card Slot
- Sleep (Due to TPM not being able to be disabled in BIOS (blame ASUS)
- HDMI Port (Not Supported Yet)
- Camera (Camera doesn't seem to work even though everything was configured properly
----------------------------------------------------------------------------------------
Notes:
- Sleep: You can install a program called NoSleep to fix macOS automatically rebooting during sleep
- TouchPad: Make sure to disable the Force Click & Haptic Feedback option so that your touchpad works properly

That's it have fun!
