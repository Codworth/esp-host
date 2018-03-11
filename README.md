# esp-host

Benefits of using ESP8266

    -completely block all possibility of updates
    -ability to run 24/7 via usb, self-hosted , no apps or programs required.
    -no need to edit dns servers or settings, features automatic redirect.
    -easy updates via usb
    -very low power consumption


Requirements:

    -linux, windows or mac
    -esptool.py or other suitable esp8266 flashing tool (many available)
    -ESP8266 Wifi Module with at least 4M flash 
    -Firmware 4.55




Instructions:
    Using esptool.py the included bin can be flashed using the following command:

    sudo esptool.py --port /dev/ttyUSB0 write_flash 0x00000 0x400000 ./esphost.bin
    
    after flashing completes, connect to "PS4-WIFI" using "easy setting"  then launch as normal.
    
    *windows users must use the appropraite com port when flashing with esptool.py*
    




