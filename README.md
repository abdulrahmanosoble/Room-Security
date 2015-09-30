# Room-Security
This a side project developed using arduino. Whenever someone enters my room it will both sound a buzzer and send a tweet logging the time that the room was entered.

Here is a demo of the project: https://youtu.be/t_8g3pXZr54

Below is a schematic that does not include the Adafruit CC3000 breakout board or the battery pack:
![Schematic](https://github.com/abdulrahmanosoble/Room-Security/blob/master/images/schematic.png)

The CC3000 is connected to the following pins:

Arduino | CC3000
--------|--------
GND | GND
5v | Vin
Digital 5 | VBEN
Digital 3 | IRQ
Digital 13 | CLOCK 
Digital 12 | MISO
Digital 11 | MOSI
Digital 10 | CS

Below is a photo the set up. The reed switch is taped under the door and cannot be seen:
![Photo](https://github.com/abdulrahmanosoble/Room-Security/blob/master/images/photo.jpg)

#How it works

The setup uses a magnet and a reed switch to detect when the door is open. The arduino then makes a request to a certain page on my personal website (http://www.abdulrahmanosoble.me). That page, in turn, then sends the tweet logging that someone entered the room.
