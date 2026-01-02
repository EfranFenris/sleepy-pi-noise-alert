## Quiet Widget for Raspberry Pi 😴📱🔔

Small IoT project where I control a Raspberry Pi from a widget on my phone’s homescreen.

When I tap the widget, the phone sends a value to an Adafruit IO feed.  
The Raspberry Pi is subscribed to that feed using MQTT. When it receives the signal, it:

- turns on LEDs, and  
- makes a buzzer beep

…so my brother gets a “please be quieter, I’m trying to sleep” alert.

## Demo video

[Watch the demo on YouTube](https://youtube.com/shorts/a92Ik1VmTD4)


### Tech stack

- Raspberry Pi (Python + `RPi.GPIO`)
- Adafruit IO (MQTT feed + mobile app widget)
- `paho-mqtt` client to receive messages on the Pi
- Optional: IFTTT if you want extra actions (emails, notifications, etc.)
