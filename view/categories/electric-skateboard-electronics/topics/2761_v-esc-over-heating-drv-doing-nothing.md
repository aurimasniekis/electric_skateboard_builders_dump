# V-ESC over heating drv doing nothing

### Replies: 6 Views: 698

## \#1 Posted by: boubak Posted at: 2016-04-30T22:04:33.500Z Reads: 78

```
Hi,

I bought two v-esc from enertion boards the 4th of august 2015, and I just started tu program them.

Both are a 4.7HW version and have a 2.16 firmware flashed using a stlink-v2 plugged into the swd ( the bootloader was broken, impossible to update by the bldc-tool).

Both are working now, but only one of them heats up anormaly fast (i.e : Mosfets at 50 degrees rising, idle).

Is this normal, should I be worried about this? (the other one stays at 30 degrees )

Thanks.
```

---
## \#2 Posted by: elkick Posted at: 2016-04-30T22:09:19.891Z Reads: 75

```
About the firmware: Did you open conf_general.h and select which hardware version you are using before the make upload command? Default is 4.10/11/12 now, so it needs to be changed for 4.7 when working with Ubuntu.
```

---
## \#3 Posted by: boubak Posted at: 2016-04-30T22:32:16.888Z Reads: 72

```
I took a pre compiled version configured for HW4.7.Both of them use this firmware, but only one is over-heating.
```

---
## \#4 Posted by: boubak Posted at: 2016-05-01T09:08:34.136Z Reads: 53

```
Hi again,

I checked again and on the over heating one the DRV8302 is especially hot ( I can't let my finger on it more than
2 seconds, I know it's not a really precise mesurement, but I have not any thermometer with me to the place where I am right now :) ).

Thanks
```

---
## \#5 Posted by: boubak Posted at: 2016-05-03T14:06:01.663Z Reads: 32

```
Hi again again,

Has anybody any clue about this?

(Another information about my test I forgot to give, I was supplying maximum 4A of current, with a modified laptop
power supply)

Thanks a lot in advance.
```

---
## \#6 Posted by: boubak Posted at: 2016-05-09T22:28:15.383Z Reads: 28

```
Hi again,

Probleme solved : A friend of mine took a look with a x10 magnifier and found a micro tin bridge between two legs of the DRV, removed it and now it works without overheating.

Bye
```

---
