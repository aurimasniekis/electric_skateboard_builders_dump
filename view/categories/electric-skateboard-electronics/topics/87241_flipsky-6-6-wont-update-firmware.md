# Flipsky 6.6 wont update firmware

### Replies: 6 Views: 452

## \#1 Posted by: JensSjogren Posted at: 2019-03-15T16:58:56.666Z Reads: 99

```
Hola, So i got 2 new and unused Flipsky 6.6 ESC's, yesterday i soldered the bullet connectors on to them and hooked them up to my computer for programming. As usual i get the update message that always pops when connecting a ESC for the first time. So i updated the ESC with hardware version **60** and firmware **VESC_default.bin** selected. As normal i got the serial port error and then waited about 30 secs untill i rebooted the ESC, when i reconnect the ESC i still get the update message, so it doesn't seem like the ESC wants to write the update. I get the same results on both of my Flipsky 6.6. 

anyone experienced this issue before? pretty darn annoying.. 

Thankfull for any advice or sulotions!
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-15T17:05:12.683Z Reads: 90

```
Wasn’t there something like they don’t have a bootloader pre installed or something?
Not sure but have a search for it. I think you need first load the bootloader, than you can change the fw version.
```

---
## \#3 Posted by: JensSjogren Posted at: 2019-03-15T17:08:08.306Z Reads: 88

```
hmm okay, in the messages on VESC tool it says that it has a boot loader atleast. i'll search for that, seems a bit odd that a 190$ ESC doesnt have a boot loader
```

---
## \#4 Posted by: Andy87 Posted at: 2019-03-15T17:48:12.503Z Reads: 78

```
Thats what i found on the go.
https://www.electric-skateboard.builders/t/flipsky-6-6-group-buy-its-on-120-w-2-day-shipping-and-tracking-usa/63725/200?u=andy87

But I don’t know what was the issue and how he solved to flash the fw.
```

---
## \#5 Posted by: JensSjogren Posted at: 2019-03-15T21:13:59.375Z Reads: 69

```
Silly me, didn't know that i could flash the bootloader firmware via vesc tool, got them both to work now. Thanks @Andy87 :)
```

---
## \#6 Posted by: DougM Posted at: 2019-03-16T00:12:10.052Z Reads: 65

```
I gave up on the Flipsky's.  I couldn't get mine to flash either (just like you they came with two different versions of the firmware) and then one of them died and took the remote receiver with it, so now the board is in pieces waiting for a Unity to arrive.
```

---
