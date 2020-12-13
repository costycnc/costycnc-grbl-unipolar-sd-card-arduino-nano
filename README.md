# costycnc-grbl-unipolar-sd-card-arduino-nano
    insert costycnc folder in documents arduino ... see photo
    Project for include sd card to grbl 1.1h
    copied from:
https://github.com/ryanj1234/SD_TUTORIAL_PART4

    beautiful tutorial about sdcard:
http://www.edproject.co.uk/18Series15.html

    cosduino bootloader from sdcard
https://sites.google.com/site/atmega8pro/cosduino_bootloader   

     1001000 
     400000 boot

     8192*512=4194304
     0x2000*0x200=400000

     1401000

      0x1000000 root directory (penso che e offset da 0x400000... deve adaugare 0x400000 >> 0x1400000

     0x1001000 prima file     >> 1401000/200=sector A008 
     0x1002000 seconda file   >> 1402000/200=sector A010
