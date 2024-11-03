## info
* **ESP32-S3-DevKitC-1-N16R8.json** - this is board description file for ESP32-S3-WROOM-1-N16R8 16 MB (Quad SPI) 8 MB (Octal SPI) [documentation](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)
* **default_16MB.csv**  this is basic partition file with minimum 3.5Mb spiffs file system

![look](./doc/esp32s3.PNG)

## Other
* You can find other partition files [this](https://github.com/espressif/arduino-esp32/tree/master/tools/partitions)
* And other board description files [this](https://github.com/Jason2866/platform-espressif32/tree/Arduino/IDF5/boards)

# Instrustions
1) move all this files to ***{ProjectPath} / boards***
2) edit **platformio.ini** file:

```cpp
; Flash: 16MB QD, PSRAM: 8MB OT
[env:ESP32-S3-DevKitC-1-N16R8]
platform = espressif32
board = ESP32-S3-DevKitC-1-N16R8 ; 16 MB Flash, 8MB octo PSRAM
framework = arduino


monitor_speed = 115200
```

   
