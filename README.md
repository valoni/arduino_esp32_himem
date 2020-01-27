# arduino_esp32_himem

The ESP32 version WROOM32 is an ESP32 version that supports external RAM (PSRAM / SPI RAM).
For ArduinoIDE, normally can access only the first 4MB
Although some external RAM can be connected up to 8MB

Access to the top 4MB command (ESP32 HIMEM) for on the Arduino will not yet be accessible.

such as
Esp_himem_get_phys_size () command;
-> command to display the HIMEM PSRAM area in excess of the first 4MB

Esp_himem_get_free_size () command;
-> command to display the area of the PSRAM area, the HIMEM area that can be reserved

Etc.
On Arduino, will not be able to run
As well as the order to reserve the Mem area in the upper section


For more external RAM usage
source code in this repository
Will be a supplement that makes Arduino-ESP32 Can access the top 4MB management command of PSRAM too

__Usage__

1. Copy files in folder  /core   to your Arduino platform folder at
```
C:\Users\<USER NAME>\AppData\Local\Arduino15\packages\esp32\hardware\esp32\1.0.2\cores
```

2. Test Arduino Sketch by /example/ESP32_PSRAM_Himem/ESP32_PSRAM_Himem.ino  

<p align="center">
  <img src="example.png" alt="image"/>
</p>  

TridentTD  
25 June 2018  

Translated by Google Translator Valoni
27 January 2020
