# lDoes a wireless passive on/off ignition switch that holds its state exist? Need help for my custom electric scooter!

### Replies: 2 Views: 79

## \#1 Posted by: 010203040506070809 Posted at: 2019-09-30T21:50:49.907Z Reads: 28

```
Hi,

I'm new to electrical engineering and am currently in the process of modding a custom electric scooter I've built. But I need your help.

**Goal:**  Be able to turn on/off my electric scooter wirelessly (technology doesn't matter, wireless, blutooth, RFID, something mechanical like a magnet?). Ideally -- it's a passive switch (no power draw from battery when it is off), and more importantly, it HOLDS it's state. So I don't need to hold a magnet to the switch constantly to have it turned on but just need to tap the magnet once to turn the switch on, and tap it again to turn it off. Something like that. I don't want a physical toggle switch because of security issues (don't want some random person to turn on my scooter while I'm away).

The other important parameter is that because this electric scooter will go over unpaved roads and high-vibration environments, it must not just click on/off easily if you hit a big bump.

Finally, the switch will be connected to a 42v lithium ion battery (10 cells) which is then connected to a Flipsky microcontroller. So the switch should be able to handle 42v / high current because presumably the direct drive motor might take in a lot of current?

Basically, is there some form of wireless passive on/off ignition switch that holds its state and meets the parameters above?

I used to use an antispark switch but after having 3 fail on me in a row, i'm going to find a different solution. Also don't want to carry around a loop key so prefer to make my solution wireless.

Would this work:

https://imgur.com/a/BXBSkHW

Parts list:

https://www.amazon.com/gp/product/B07KWT29WR/ref=ox_sc_act_title_2?smid=AFLYC5O31PGVX&psc=1

https://www.amazon.com/gp/product/B01MYPTVJD/ref=ox_sc_act_title_3?smid=A1EQP448COWZL4&psc=1

Do i have the wiring correct? My only concern is that the relay is rated for 12v... and the battery provides 36v. Do i need to use a buck stepdown converter? If so, the other problem is that wouldn't I be underpowering the motor that connects to the VESC if I'm no longer providing the full 36v of power but instead 12v only?
```

---
## \#2 Posted by: KevinH Posted at: 2019-10-01T03:06:51.229Z Reads: 16

```
I don't think enertion sells anything like that, maybe try on the other fo&ZeroWidthSpace;rum at fo&ZeroWidthSpace;rum&period;es&ZeroWidthSpace;k8&period;ne&ZeroWidthSpace;ws
```

---
