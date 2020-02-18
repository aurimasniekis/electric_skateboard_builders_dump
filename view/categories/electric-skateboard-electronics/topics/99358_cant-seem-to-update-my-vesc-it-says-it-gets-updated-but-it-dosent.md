# Cant seem to update my VESC. It says it gets updated but it dosen&rsquo;t

### Replies: 12 Views: 306

## \#1 Posted by: mackattack Posted at: 2019-07-29T19:39:57.127Z Reads: 59

```
So i bought my VESC from DIYectricskatebaords and when i connect it to my PC i get this error "The connect VESC has to old frimware. Since the connect VESC has firmware with bootloader support, it can be updatef from the frimware page. Until then limited communication mode will beused where only the firmware can be changed. I then go into the firmware page and update it which takes around 10 seconds. When the update is done i get the mussage that the update has been successful. This is the message " Firmware upload finished! Give teh VESC around 10 seconds to apply the firmware and reboot, then reconnect" I can't really see that the VESC restarts but when i try to reconnect it i get the same message that teh VESSCs firmware is to old. Is there anything wrong with my VESC or am i doing something wrong?

I've prob tried updating it 15 times now.

This is the VESC im using:
https:///products/torque-esc-bldc-electronic-speed-controller
```

---
## \#2 Posted by: Flasher Posted at: 2019-07-29T19:49:45.413Z Reads: 56

```
It's a corruption. I had to use an stlink along with the help of @Gamer43  to fix it
```

---
## \#3 Posted by: Santino Posted at: 2019-07-29T19:56:14.742Z Reads: 54

```
I think is the bootloder. I would download de bootloader from the Vesc tool page, and then update the firmware. You could ask the seller; but I think it is just that.
```

---
## \#4 Posted by: mackattack Posted at: 2019-07-29T20:23:24.665Z Reads: 50

```
With Vesc tool page do you mean their webpage or a tool page in the program?
```

---
## \#5 Posted by: mackattack Posted at: 2019-07-29T20:54:20.704Z Reads: 49

```
Could the problem be my USB cable? I heard that some cable can't transfer data. I'm not sure if that true or not though.
```

---
## \#6 Posted by: Santino Posted at: 2019-07-29T21:03:06.762Z Reads: 46

```
When I was trying to upload the new Vesc firmware to a Vesc 6 I had the same issue. So I've got in to the Vesc project was page and search through the forum....I found some people with the same situation, and read about missing the boot loader, and that the message about destroying your vesc it was an automated answer...So I went to the vesc tool page, and if you get into software downloads, there is a possibility to download the boot loader...So I did that, then git the download the new firmware and got it working...As I mention before, the symptoms were the same as yours...But if you are afraid, ask the vendors....or Frank from Trampa, or just search through the vesc project forum...
```

---
## \#7 Posted by: Santino Posted at: 2019-07-29T21:04:02.553Z Reads: 46

```
Your usb is workin, otherwise you won't be able to download or connect to anything...
```

---
## \#8 Posted by: Santino Posted at: 2019-07-29T21:08:30.919Z Reads: 44

```
I did everything with the vesc-tool...
```

---
## \#9 Posted by: mackattack Posted at: 2019-07-30T11:37:39.224Z Reads: 37

```
Hm yeah it seems like it's missing a bootloader but i can't even download the bootloader in the VESC tool. I get the same message that it seems to be succesful but i can't still download a software update.
```

---
## \#10 Posted by: torqueboards Posted at: 2019-07-30T13:53:26.081Z Reads: 32

```
@mackattack Sounds like the firmware is messed up. If you're local in the USA, you can email us and we an re-flash your VESC or you can also do it yourself as well.
```

---
## \#11 Posted by: mackattack Posted at: 2019-07-30T14:15:42.153Z Reads: 29

```
Im based in Sweden unfortaly. How do i reflash it? If i understand correctly i need to buy an STlink for that.
```

---
## \#12 Posted by: Flasher Posted at: 2019-07-31T03:17:00.800Z Reads: 22

```
@mackattack 

https://www.electric-skateboard.builders/t/i-might-have-bricked-my-esc-help/95393
This is the thread I had created when I had gotten a fw problem. It could help you in understanding and there's a link to get the piece of hardware you'll need if you do it yourself
This is the hardware in question:![15645431142466027948382482074326|375x500](upload://y9c6AS2BEhV1kOcSrMwzgAbyvzY.jpeg)
```

---
