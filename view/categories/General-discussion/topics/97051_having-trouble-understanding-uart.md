# Having trouble understanding UART

### Replies: 3 Views: 155

## \#1 Posted by: hahne Posted at: 2019-06-21T15:49:42.766Z Reads: 59

```
So all this time, I have been connecting to my boards with arduino/bluetooth modules via the ppm receiver section of the VESC. The connection looks like this     
 TX: Arduino nano -->Bluetooth module -----> RX: Bluetooth module --> Arduino nano --> ppm slot

I know that a good number of people are using the UART port on the VESC, but I am really confused as to how to use it. Do I still need an arduino on the RX side? or can the connection simply be         
 RX: Bluetooth module --> UART port? would I still need an arduino on the PPM port?

Also, are there any specific benefits of using the UART port instead of the PPM port?

Basically I suck at electronics, so any help would be appreciated.

Thanks.
```

---
## \#2 Posted by: StefanMe Posted at: 2019-06-21T18:22:19.444Z Reads: 43

```
I don't get u. 

To communicate with the VESC over UART u need TX AND RX connected to the Nano/Bluetooth module. For one UART port just one device. 

On the unity for example u have two UART ports. One hidden under the enclosure and one on the PINOUT. The focbox (single) hast just one UART port. Means just the Bluetooth module or the Nano. U can use  a second focbox over can and use the second UART port on the second focbox as well. 

My receiver from the FeatherRemote is connected to the Pinout on the Unity. 5V. GND. TX. RX. . For the BT module I use the new Metr. Module that is mounted inside the enclosure.
```

---
## \#3 Posted by: hahne Posted at: 2019-06-22T22:37:14.398Z Reads: 23

```
Okay so connecting to the unity, I will only need an Arduino, but no other bluetooth module other than the one on board? 

And the regular vescs I will need an arduino AND a Bluetooth module connected to their own individual UART ports? 

That helps a lot. Thanks
```

---
