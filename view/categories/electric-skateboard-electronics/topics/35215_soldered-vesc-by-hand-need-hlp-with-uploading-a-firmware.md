# Soldered VESC by hand, need hlp with uploading a firmware

### Replies: 8 Views: 449

## \#1 Posted by: SpyChar Posted at: 2017-10-10T00:38:45.320Z Reads: 117

```
Hello there. So, here is the problem. I've soldered together a vesc and flashed it with a bootloader from vedder's github. Now I want to upload a firmware using the bldc tool but my vesc doesn't show up on the list. Are there any additional steps that I need to take to be able to connect it to my PC? Or should it work right now? If so, what could be wrong?
```

---
## \#2 Posted by: monkey32 Posted at: 2017-10-11T05:57:08.726Z Reads: 69

```
Photos or it didn't happen......also just want to see
```

---
## \#3 Posted by: scepterr Posted at: 2017-10-11T06:11:37.437Z Reads: 67

```
Are you powering the vesc with something other than the USB?
Does it light up when you power on?
Does anything show up in Device Manager when you plug it in, if it powers on and lights up?
```

---
## \#4 Posted by: Surfer Posted at: 2017-10-11T06:16:03.084Z Reads: 66

```
If I remember well you should do it with the st link programmer.
```

---
## \#5 Posted by: scepterr Posted at: 2017-10-11T06:23:40.156Z Reads: 65

```
He already flashed the bootloader with stlink, now hes trying to flash the firmware with bldc tool
```

---
## \#6 Posted by: Martinsp Posted at: 2017-10-11T06:30:54.132Z Reads: 65

```
Assuming you are powering it on with a psu or a battery and it boots correctly (confirmed by flashing 3 times red light) and it does not show on the screen you after have a hardware problem so something around the USB port might not be soldered corrcly or your PC does not have the STM device driver. You can download them from their website. If your are using Windows then the way to test is that if the device shows as unrecognizable in Windows then it is the drivers if it does not show at all it is not actually connected.
```

---
## \#7 Posted by: Surfer Posted at: 2017-10-11T06:35:47.738Z Reads: 64

```
The firmware can be also flashed with the programmer.
```

---
## \#8 Posted by: SpyChar Posted at: 2017-10-11T15:39:20.356Z Reads: 53

```
Thanks for all the support guys, u r geat. Turns out, the problem was my lack of knowledge. I assumed that bootloader is enough to connect with bldc tool. I flashed it with 2.18 firmware and went with Ackmaniac's bldc tool right away. 2.54 firmware was uploaded successfuly and it didn't catch on fire which is a good sign. Photos will come, but only when I'm sure that everything works. Otherwise I would be ashamed :P. I forgot to buy banana plugs for motor wires, so testing has to wait for a couple of days.
If I already have this thread going, could U guys suggest any bldc tool settings? I bought an SK3 236kv motor and two 4s lipos which r gonna make a n 8s package.  The gearing i'm thinking about is 12 teeth for a motor and 40 teeth for a wheel.
```

---
