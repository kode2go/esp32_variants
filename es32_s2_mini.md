# Setup

# VS Code 

## Correct Bootloader Sequence for ESP32-S2 Mini:

Hold down BOOT (usually labeled 0)

While holding BOOT, tap or press RESET (RST)`

Release BOOT

platformio device monitor --port COM13

# Platform.ini

```
[env:esp32-s2-saola-1]
platform = espressif32
board = esp32-s2-saola-1
framework = arduino
upload_speed = 115200
monitor_speed = 115200
upload_port = COM13
```

# Code

```
#include <Arduino.h>

#define LED_PIN 15  // Change to the correct GPIO for your board

void setup() {
  pinMode(15, OUTPUT);

}

void loop() {
    digitalWrite(15, HIGH);
    delay(500);
  
    digitalWrite(15, LOW);
    delay(500);
  }

```

# Arduino
<img width="692" height="298" alt="image" src="https://github.com/user-attachments/assets/a21e6eec-8714-4d04-a929-8d5d0f575db7" />
