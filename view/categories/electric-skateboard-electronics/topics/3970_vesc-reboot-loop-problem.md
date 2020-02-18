# VESC reboot loop problem

### Replies: 3 Views: 914

## \#1 Posted by: boubak Posted at: 2016-05-29T10:02:05.336Z Reads: 110

```
Hi,

**Here the context:**

I bought two v-esc from enertion boards the 4th of august 2015.

Both are a 4.7HW version and have a 2.16 firmware flashed using a stlink-v2 plugged into the swd ( the bootloader was broken, impossible to update by the bldc-tool).

I performed my tests with a computer running linux mint 17.2 rafaela and I power my vescs with a laptop power supply giving max 4.74A at 19V.

I wrote a previous post about one of my VESC that was over-heating, there was an anormal bridge between two pins of the DRV8302. A friend of mine gave me hand to remove it, the overheating problem was gone, and after that my previously faulty VESC was running normaly.

**My problem :(**

And now, when I try to configure/test it with the usb wire plugged-in, It randomly disconnect after a while.
The sequence is :

1. I plug the power and the usb wire
2. I start the bldc_tool and connect it to the vesc
3. If I do something with the bldc_tool or not, after a while (comprised between 10 s and 1 min), the tool loose the connection with the vesc, the blue led of the vesc being off.
4. After a time comprised between 1 s and 1 min, the blue led start bliking poorly, then one blink of the red led, and I can connect the bldc_tool to it again.

This restart cycle can be done many times before the vesc seems to restart again and can't never be joined by the tool, at this point the blue led never goes off, and I need to disconnect the vesc power in order to be able to try to connect the tool again. ( tail -f /var/log/syslog doesn't say something anymore about the vesc connection)

Sometimes after the first crash/disconnection the vesc goes directly to the "never be joinable again" step.

It seems that jiggling the cables or try to run my motor, shorten the time before the vesc crash/disconnect.

If anybody has a clue :).

Boubak

**Edit**: 

The green led is on when the blue led is on and not blinking and at  "never be joinable again" step, the green led never goes on again.

So the sequence is a little bit more complex, there is two cases : 

**Case 1 : the vesc will be joinable again after that :**

* Crash/disconnection -> All Leds off
* Shortly after blue led blink rapidly with the intensity and the frequency decreasing
* Blue led completly off for many seconds
* Blue led start to blink with frequency, time on and intensity increasing at the end the red and the green one blinks very poorly 1 or 2 times
* Blue led on, at this time, the red one blink twice very distincly and goes off
* Green led goes on

**Case 2 : the vesc will not be joinable after that :** 

* Crash/disconnection -> All Leds off
* Shortly after blue led blink rapidly with the intensity and the frequency decreasing
* Blue led completly off for many seconds
* Blue led start to blink with frequency, time on and intensity increasing
* Blue led on

**Edit 2:**

My faulty VESC does this with or without usb wire plugged in, with or without any motor plugged in. And it invariably goes to the unjoinable state/only blue led on after a random number of cycles.
```

---
## \#2 Posted by: boubak Posted at: 2016-06-07T20:05:39.366Z Reads: 54

```
Anybody ?

Boubak
```

---
## \#3 Posted by: FlyingJaffaCake Posted at: 2018-02-14T19:41:41.103Z Reads: 22

```
I have exactly the same issue.  What resolved it?

Thanks
```

---
