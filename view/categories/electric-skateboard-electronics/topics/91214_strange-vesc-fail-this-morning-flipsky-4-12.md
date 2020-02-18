# Strange VESC fail this morning (flipsky 4.12)

### Replies: 3 Views: 175

## \#1 Posted by: Bobby-gg Posted at: 2019-04-20T09:43:26.328Z Reads: 66

```
I did use the search function but just got a load of hits about VESC and programming them

Woke up early this morning to sunshine and blue skies so thought I'd go out for a early morning blast

I was going to replace my motor the other day so had the motor wires and the sensor connection disconnected, so plug them all back in again and powered up the board but pulling the trigger did nothing. 

Connected VESC tool via Bluetooth and watched the real time data, the motor amps were going up, the duty cycle was too, but I wasn't getting an error code, nor any motor movement. 

Went to reprogram the VESC as a new install and the tool responded by saying it needed the latest firmware, I only built this board a month ago so it should of been running the latest firmware from then 

Once updated, it ran the motor and handset config no problem, but I had to reverse the motor sense within the app as I'd wired the motor phases up incorrectly, it accepted that setting but would allow me test the motor direction from the app, again saying that it needs the latest firmware to do the function 

So, would disconnecting the motor completely make the VESC loose its programming, which I doubt as it doesn't when powered down, or is it just a thing it'll do every so often often and it was completely coincidental that it occurred whilst the motor was out 

Oh, and I did get out for my ride, just a little later than planned 

Rob
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-20T10:13:55.707Z Reads: 57

```
If you disconnect the phase wires and plug them back in a different order than before you always need to run a new motor detection before it will work again.

If you have the right vesc tool version for your FW than the old FW message shouldn’t pop up.
```

---
## \#3 Posted by: Bobby-gg Posted at: 2019-04-20T10:38:06.295Z Reads: 53

```
Thanks Andy, that would explain having to reprogram it

I'll try and get the firmware error up again to get a screen shot and post it up
```

---
