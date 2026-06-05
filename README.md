# Raspberry Pi Pico W Alarm Clock

A WiFi-synced alarm clock built with the Raspberry Pi Pico W and MicroPython.
Automatically syncs time via NTP on boot and re-syncs every 6 hours. All
components available from [PiShop Africa](https://www.pishop.co.za).

---

## Features

- Automatic time sync over WiFi using NTP
- SAST (UTC+2) timezone support
- Time and alarm status displayed on a 1602 I2C LCD
- Repeating beep pattern on alarm trigger
- Set alarm hour and minute via push buttons
- Toggle alarm on/off without changing the set time
- Dismiss alarm with a single button press

---

## Components

- Raspberry Pi Pico W - [View on PiShop](https://www.pishop.co.za/store/raspberry-pi-pico_0/raspberry-pi-pico-h)
- IIC I2C 1602 LCD Display - [View on PiShop](https://www.pishop.co.za/store/displays/iic--i2c-1602-blue-backlight-lcd-display-module-for-arduino)
- Passive Buzzer with Jumper Housing - [View on PiShop](https://www.pishop.co.za/store/buzzers/buzzerpassive-with-jumper-housing)
- Tactile Momentary Push Buttons - [View on PiShop](https://www.pishop.co.za/store/switchesbuttons/25pcs-tactile-momentary-push-buttons-12x12x73mm-with-caps-5-colours)
- Breadboard and jumper wires

---

## Wiring

**LCD**
- VCC → VBUS 5V (Pin 40)
- GND → GND (Pin 38)
- SDA → GP2 (Pin 4)
- SCL → GP3 (Pin 5)

**Buttons**
- Mode → GP10 (Pin 14) + GND
- Up → GP7 (Pin 10) + GND
- Down → GP8 (Pin 11) + GND
- OK → GP9 (Pin 12) + GND

**Buzzer**
- \+ → GP16 (Pin 21)
- \− → GND

All buttons use the Pico W's internal pull-up resistors — no external resistors needed.

Check out our Blog here for installation instructions and circuit setup process:
