# esp-host

Today I show you a simple way to serve payloads using the esp8266

![alt tag](https://raw.githubusercontent.com/Codworth/esp-host/master/esphost.jpg)


Benefits of using the ESP8266

    
    -extremely low cost hardware , available worldwide
    -ability to run 24/7 via usb, self-hosted payloads, no external apps or programs required.
    -completely block all updates
    -no need for custom dns server or settings, features automatic redirect.
    -easy to program and update via usb
    -very low power consumption


Requirements:

    -esptool.py https://github.com/espressif/esptool 
    -ESP8266 Wifi Module with at least 4M flash
    -Firmware 4.55 or 4.05 (untested on 4.05)
    -esphost.bin or esphostmulti.bin or esphostmulti405.bin
   
   Payloads included in esphost.bin
   
  
    -VORTEX HEN 1.4
    
   Payloads included in esphostmulti.bin
   
    -VORTEX HEN 1.4
    -VORTEX HEN 1.4+VR
    -VORTEX DUMPER 1.7
    -VORTEX FTP 1.2
    -BACKUP BY STOOGED
    -APPTOUSB V3 BY STOOGED

Instructions:

    Flash esp host using the following command:
    
    sudo esptool.py --port /dev/ttyUSB0 write_flash 0x00000 0x400000 ./esphost.bin
    
    -after flashing completes, connect to "PS4-WIFI" using "easy setting" then go to [Settings] > [User Guide]
    
    -NOTE: windows users must use the appropriate com port when flashing with esptool.py
    -NOTE2: users can optionally flash using the GUI version of esptool  https://github.com/Rodmg/esptool-gui
    -NOTE3 when using multi sometimes the page will hang, to fix refresh the page to make sucessful.
Compatible boards:

These are the most popluar esp8266 boards, but any esp8266 with 4M flash or larger will work.

    ESP8266 NodeMcuV2 4M wifi Module        (amazon) https://tinyurl.com/y9xskhcy
    			                (aliexpress) https://tinyurl.com/y7jq3fnq
                                
   
                                     
    ESP8266 D1 Mini NodeMcu 4M              (amazon) https://tinyurl.com/y9mx83ev
                                            (aliexpress)https://tinyurl.com/y8rqfafz
                               
                               
   To-Do
    
    -add ability to upload files/payloads                  
   

   Notice and credits
   
    I did not develop the payloads contained in esphost.
    
    Credit should be given to the original authors
    

