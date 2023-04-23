# coffee-scale
## Overview
Total proportions are ~10x12x1.5cm (conditioned on fitting everything in) in a rectangle shape. Can design a fun model once internals are worked out. There will be a weight area and an OLED area at the bottom of the scale. Neat idea is to use the weighing platform as an opaque cover that sits over the scale that the OLED can shine through. Power and time buttons will be located on the right and left side of the unit respectively. Hold power to turn on/off, press to tare 

```
xxxxxxxxxxx
x WEIGHT  x - Weight area 10cmx10cm
x  AREA   x   
x---------x
x DISPLAY x - Display 2cmx10cm.
xxxxxxxxxxx
```

Basic hadware components:
 - Microprocessor 
 - Weight measurement
 - Weight reading
 - OLED screen
 - Power source
 - Interactivity (touch buttons ideally)

Software components:
  - Timer
  - Bluetooth and WiFi connectivity
     - Streaming data
     - Connect to scale and confirm from scale
  - Weight read
  - OLED display 
  - Menu navigation using two buttons (or perhaps menu selectors at back of scale?)


Project stages:
1. Basic scale functionality:
   1. Turn on and off.
   2. Measure weight 
   3. Tare
2. Timing functionality. 
   1. Start, stop, and reset timer.
3. Bluetooth functionality.
   1. Stream data externally.
   2. Receive data externally and display on OLED (thinking a progress bar for shot duration if the machine has this calibrated, either via time, volumetrics or weight).
4. Case design!
   1. Build a fun case to sit in which supports touch sensitive buttons.

## Parts
Board: [ESP32-S2-DevKitM-1](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s2/hw-reference/esp32s2/user-guide-devkitm-1-v1.html)
Load Cell: [TAL221](https://www.robotgear.com.au/Product.aspx/Details/6023-Mini-Load-Cell-500g-Straight-Bar-TAL221)
Cell reader: [HX711](https://www.sparkfun.com/products/13879)
Display: [Some OLED](https://www.buydisplay.com/green-2-2-inch-oled-128x32-spi-display-module-serial-i2c-ssd1305)
