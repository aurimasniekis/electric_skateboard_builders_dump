# Trouble connecting VESC to PC

### Replies: 9 Views: 430

## \#1 Posted by: Esk8Builder Posted at: 2018-04-02T05:59:06.757Z Reads: 68

```
As the title states, I'm having trouble getting my VESC (4.12) to connect to my computer. One hour ago everything was working nicely. I havent ridden it, unplugged/changed anything, or uploaded new firmware or even changed any settings since then but now I only get a blue light when I power it on. I know this led is connected to the 3.3v rail which means my MCU is getting the required power. This leaves only two options in my mind. Either the bootlader is gone for no apparent reason or the MCU is fried. Neither of these make sense as I wasn't messing around with the hardware and was only doing testing with the UART communications on this thing (working on an app that communicated with the VESC over bluetooth).

Does anyone here know anything that might be able to help me out? Thanks.
PS: its 2am and I'm tired. sorry if what i typed doesnt make sense
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-04-02T06:07:36.670Z Reads: 63

```
Fried drv? Maybe bad vesc with bad solder joints and was just a accident waiting to happen?
Do you connect it first then turn it on ? 
This just happened to me ... I ridden mine but it just turns on with blue light no flashing. So its DRV likely not sure buddy.
Pictures would help
```

---
## \#3 Posted by: Esk8Builder Posted at: 2018-04-02T11:46:03.339Z Reads: 50

```
I'll take some pictures tonight when i get home from my classes and labs. Why would the DRV be the culprit? Wouldn't the MCU still operate without problem but just throw the DRV fault whenever throttle is applied?
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-04-02T11:48:31.410Z Reads: 44

```
I had something similar happen... was messing around with my vescs while my battery was **in the other room, disconnected** and my MCU started smoking then popped. still not sure what the hell coukdve happened since the caps couldn’t have been charged and wasn’t connected to anything
```

---
## \#5 Posted by: Esk8Builder Posted at: 2018-04-02T11:56:42.927Z Reads: 42

```
Decided to take some quick pictures, the weird looking circuit attached to the vesc is my MOSFET soft switch.![20180402_075110|281x500](upload://5lhvhWzoPprMQBDlyLioj0lUB56.jpg)![20180402_075118|281x500](upload://zPlMFWT0AWbGEAyh5U4O20Yx762.jpg)![20180402_075150|281x500](upload://zWNILSvsXwHZHuUGmZpEnGAnXO0.jpg)
```

---
## \#6 Posted by: Esk8Builder Posted at: 2018-04-02T16:00:24.712Z Reads: 27

```
Forgot to mention that only the blue led turns on when power is applied. No red led flashes or anything
```

---
## \#7 Posted by: Esk8Builder Posted at: 2018-04-05T13:56:37.716Z Reads: 17

```
Managed to solve the problem. All I had to do was reflash the bootloader. I used a raspberry pi running openocd since I don't want to spend money on an stlink V2. I don't know exactly why the bootloader got corrupted but it could have something to do with receiving an invalid command over UART.
```

---
## \#8 Posted by: BayneSolo Posted at: 2019-10-25T02:23:37.020Z Reads: 6

```
Hey I know this is an old thread, but I'm having the exact same problem. Trying to get my VESC connected using a raspberry pi but running into issues with writing the bootloader.

Did you ever run into the "Info : Device Security Bit Set" and being unable to write due to it being protected? I've tried everything I can think of to disable it.

Cheers in advance :)
```

---
## \#9 Posted by: Esk8Builder Posted at: 2019-10-25T03:31:37.821Z Reads: 5

```
Sorry, I don't remember. My board has been working fine for at least a year now. Good luck with your problem
```

---
