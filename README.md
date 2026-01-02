## Quiet Widget for Raspberry Pi 😴📱🔔

## Demo video

[![Watch the demo]]([https://youtu.be/TU_ENLACE_AQUI](https://youtube.com/shorts/a92lK1VmTD4))

Small IoT project where I control a Raspberry Pi from a widget on my phone’s homescreen.

When I tap the widget, the phone sends a value to an Adafruit IO feed.  
The Raspberry Pi is subscribed to that feed using MQTT. When it receives the signal, it:

- turns on LEDs, and  
- makes a buzzer beep

…so my brother gets a “please be quieter, I’m trying to sleep” alert.

### Tech stack

- Raspberry Pi (Python + `RPi.GPIO`)
- Adafruit IO (MQTT feed + mobile app widget)
- `paho-mqtt` client to receive messages on the Pi
- Optional: IFTTT if you want extra actions (emails, notifications, etc.)
