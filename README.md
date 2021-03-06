# Timer Relay

This is a Timer Relay switch based on the Wemos D1 mini.
The Wemos is used to read the time from a DS 3231 RTC module via I2C, and when a configured "Start Time" is reached, a relay is turned ON, via a GPIO pin. When the time reaches a configured "End Time", the relay is turned OFF. 
An additional feature is that the relay can also be controlled manually from a mobile phone or laptop.

There are two such relays which can operate independent of each other.

When the device is turned on, the Wemos starts a WiFi hotspot and gets the IP address 192.168.4.1. It runs a web-server which shows a configuration screen when the address http://192.168.4.1/ is accessed from a mobile phone or laptop computer connected to the Wemos' Wi-Fi hotspot. 

The configuration screen allows the user to set the RTC time, and the two timers for the relays. Aditionally, it shows the times when the timers become ON and OFF the next time. 

The screen also allows the user to turn ON or OFF the two relays manually.

The configuration page looks like the following:

<img src="https://github.com/ajithvasudevan/TimerRelay/raw/master/TimerRelay%20-%20Web%20UI.png" alt="Drawing" width="400px"/>

The circuit can be powered either directly by a 5V DC power source as shown in the schematic diagram below, or a USB (mobile phone) charger connected to the USB port on the Wemos.


## Schematic

![Schematic](https://github.com/ajithvasudevan/TimerRelay/raw/master/TimerRelay.png)


## Prototype
![Prototype](https://github.com/ajithvasudevan/TimerRelay/raw/master/TimerRelay%20-%20Prototype.jpg)
