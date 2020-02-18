# TB ESC connectors

### Replies: 4 Views: 431

## \#1 Posted by: lennarn Posted at: 2018-10-06T10:32:42.460Z Reads: 79

```
I'm trying to figure out what all the connectors on my TorqueBoards VESC are for. Most importantly, I'm trying to figure out where to plug in the motor sensors and the remote control. I made a labeled picture. If someone could just go through the numbers and tell me what each plug is for, that would be great! I really wish the TB store had this information easily available (at least I couldn't find it).![vesc_connections_crop|690x466](upload://2VkEAPsBA7F3A2uMKSVcKPedlaI.jpeg)
```

---
## \#2 Posted by: lennarn Posted at: 2018-10-06T11:02:48.052Z Reads: 70

```
https://www.electric-skateboard.builders/t/new-hobbyking-motor-6374-sensored/54792/327?u=lennarn
I found a post stating the pinout of the sensor plug for my motor (sk8 6374). This coincides with the silkscreen on the pcb of 6-pin plug "1".

6-pin (1) seems to be for Hall sensors
GND
H3
H2
H1
TEMP
5v

(2) is just the usb

4-pin (3) since pins say CAN I guess this is the "can bus"
5v
CANH
CAN1
GND

3-pin header (4) since the RC connector is 3-pin, this must be it
not labeled

6-pin (5) serial communication?
3.3v
CLK
GND
DIO
RST

7-pin (6) - ~~seems to be for remote control~~
ADC2 MISO
RX MOSI SCL
TX NSS SDA
ADC SCX
GND
3.3v
5v
```

---
## \#3 Posted by: L3chef Posted at: 2018-10-06T11:40:39.910Z Reads: 56

```
https://goo.gl/images/YqE1MD
```

---
## \#4 Posted by: mmaner Posted at: 2018-10-07T13:59:34.538Z Reads: 49

```
![vesc-diagram_1538920754832|581x500](upload://kaRzxdANp9VJfHcT0FV4jt5eGtg.png)
```

---
