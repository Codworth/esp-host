# esp-host

Today I show you a simple way to serve payloads using the esp8266
This works with firmware 5.05 , 4.55 and 4.05

![alt tag](https://raw.githubusercontent.com/Codworth/esp-host/master/esphost.jpg)


Benefits of using esp-host

    -extremely low cost hardware , available worldwide
    -ability to run 24/7 via usb, self-hosted payloads, no external apps or programs required.
    -includes stable payloads, almost no memory errors or reloading pages.
    -completely block all updates
    -no need for custom dns server or settings, features automatic redirect.
    -easy to program and update via usb
    -very low power consumption


Requirements:

    -esptool.py https://github.com/espressif/esptool 
    -ESP8266 Module with at least 4M flash
    -Firmware 5.05 4.55 or 4.05 
    -.bin file you want to flash
   
   Payloads included in esphost.bin (4.55 Only)
   
  
    -VORTEX HEN+VR (stable)
    
   Payloads included in esphostmulti.bin (4.55 Only)
   
    - HEN (stable)
    - HEN+VR (stable)
    - FTP (stable)
    - DUMPER (stable)
    - BACKUP (stable)
    
   Payloads included in esphost505.bin
   
    Vortex's HEN (Homebrew Enabler)
    Mira


Instructions:

    Flash esp host using the following command:
    
    sudo esptool.py --port /dev/ttyUSB0 write_flash 0x00000 ./esphostmulti.bin

    -after flashing completes, connect to "PS4-WIFI" using "easy setting" then go to [Settings] > [User Guide]
    
    -NOTE: windows users must use the appropriate com port when flashing with esptool.py
    
    -NOTE2: users can optionally flash using the GUI version of esptool  https://github.com/Rodmg/esptool-gui
    
    
Compatible boards:

These are the most popluar esp8266 boards, but any esp8266 with 4M flash or larger will work.

    ESP8266 NodeMcuV2 4M wifi Module        (amazon) https://tinyurl.com/y9xskhcy
    			                (aliexpress) https://tinyurl.com/y7jq3fnq
                                
   
                                     
    ESP8266 D1 Mini NodeMcu 4M              (amazon) https://tinyurl.com/y9mx83ev
                                            (aliexpress)https://tinyurl.com/y8rqfafz
                               
                               
   To-Do
    
    -add http uploading or ftp server
    -custom ssid & password
    

   Notice and credits
    
    Credit should be given to original authors of payloads - qwertyoruiopz ,Flatz , Anonymous , Vortex, Stooged  and anyone else who I missed.
   
    

