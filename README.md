| Supported Targets | ESP32 | ESP32-C2 | ESP32-C3 | ESP32-C6 | ESP32-H2 | ESP32-S2 | ESP32-S3 |
| ----------------- | ----- | -------- | -------- | -------- | -------- | -------- | -------- |

# MQTT with SSD1306


With this code, you can send the values of a DHT11 to a broker. Additionally, you can upload a user and password to the SPIFFS of the ESP32, and you can see DHT11 values on an OLED display.

## How to use the example
 
Upload the firmware into ESP32, you should to press the CONFIGURAR botton to save a password and network.
After that you are able to see DHT11 sensor values into a OLED. 

### Hardware Required

* An ESP development board
* An SSD1306 OLED LCD, with I2C interface
* An USB cable for power supply and programming

### Hardware Connection

The connection between ESP Board and the LCD is as follows:

```
      ESP Board                       OLED LCD (I2C)
+------------------+              +-------------------+
|               GND+--------------+GND                |
|                  |              |                   |
|               3V3+--------------+VCC                |
|                  |              |                   |
|               SDA+--------------+SDA                |
|                  |              |                   |
|               SCL+--------------+SCL                |
+------------------+              +-------------------+
```

The GPIO number used by this example can be changed in [lvgl_example_main.c](main/i2c_oled_example_main.c). Please pay attention to the I2C hardware device address as well, you should refer to your module's spec and schematic to determine that address.


