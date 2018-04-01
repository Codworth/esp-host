# esp-host

Today I show you a simple way to serve payloads using the esp8266

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
    -Firmware 4.55 or 4.05 
    -esphost.bin or esphostmulti.bin or esphostmulti405.bin
   
   Payloads included in esphost.bin
   
  
    -VORTEX HEN (stable)
    
   Payloads included in esphostmulti.bin
   
    - HEN (stable)
    - HEN+VR (stable)
    - FTP (stable)
    - DUMPER (stable)
    - BACKUP (stable)
   
    https://github.com/pearlxcore/ps4-playground-455

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
    
    -add ability to upload files via http
    -custom ssid & password
    

   Notice and credits
    
    Credit should be given to original authors of payloads - qwertyoruiopz ,Flatz , Anonymous , Vortex, Stooged  and anyone else who worked on the payloads. Credit to pearlxcore for his payload index used in esphostmulti            
   
    

