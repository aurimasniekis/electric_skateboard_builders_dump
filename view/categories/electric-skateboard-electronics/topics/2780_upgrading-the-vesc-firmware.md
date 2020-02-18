# Upgrading the VESC firmware

### Replies: 8 Views: 2277

## \#1 Posted by: theviith Posted at: 2016-05-01T16:59:56.106Z Reads: 196

```
Hey everyone,

So I was wondering, did any of you guys have any success with upgrading the VESC firmware to the latest FW 2.8 FOC?

I'm thinking about upgrading mine from FW1.14 to FW2.8 FOC but I just wanted to check with you guys first to see if there has been any success/or failures and what precautions or advices I should take. 

Thanks
```

---
## \#2 Posted by: treenutter Posted at: 2016-05-02T14:05:57.850Z Reads: 173

```
Assuming you have a bootloader installed, and you probably do, the upgrade itself is easy. If you don't,[ read this.](http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752) When you upgrade the firmware  be sure to follow the instructions and to select the right firmware file based on the hardware version of VESC that you've got. 

The upgrade is definitely worth it, even if you don't use FOC. If you do use FOC, and you have an older hardware version of VESC, you might need to do some work to [get the braking to work properly](http://www.electric-skateboard.builders/t/vesc-foc-braking-trouble/996)
```

---
## \#3 Posted by: theviith Posted at: 2016-05-03T04:50:06.320Z Reads: 153

```
thanks treenutter for the input. just want to clarify what bootloader is...like is it a software program, driver that I need to install on my computer? or is it a physical device that I have to buy? The link that you provided said that the bootloader should come with the VESC so I am assuming it is a physical device that connects the VESC to your computer. But from other sources that I read somewhere, I was told that bootloader is a software program that you have to install. Soo I'm a little confused here haha.
```

---
## \#4 Posted by: trbt555 Posted at: 2016-05-03T05:47:43.665Z Reads: 142

```
The bootloader is a fixed chunk of software that loads and runs the firmware.
You need the bootloader to be there if you want to use bldc tool to upgrade the firmware. All recent vescs should have a bootloader in place.
I don't know if there's a way of telling if you have the bootloader installed other than trying to upgrade the fw from bldc tool, anyone ?
```

---
## \#5 Posted by: Tarzan Posted at: 2016-05-03T15:28:45.772Z Reads: 125

```
I've stumbled over the same issue.
My latest VESC came with the 2.8 firmware but I had difficulties to find the correct BLDC tool.
With difficulties I mean I wasn't able to find a working BLDC tool....
I downgraded the firmware back to 2.16 and it is working fabulous.
Can anybody confirm my issues with firmware 2.8?
```

---
## \#6 Posted by: theviith Posted at: 2016-05-05T03:20:56.537Z Reads: 116

```
wait so if bootloader is a software, is it the same thing as STM? I remember installing something called STM microcontroller, which was required to use the VESC. But if not, where can I download the bootloader software?
Also, I heard that it's not safe to upgrade the firmware with a voltage higher than 20V or else it'll fry the FETs. Can anyone testify to this? Thanks guys
```

---
## \#7 Posted by: trbt555 Posted at: 2016-05-05T07:21:43.637Z Reads: 98

```
The bootloader runs on the vesc.
You probably remember installing the windows driver.

My opinion: if your vesc is working ok and you have a version of bldc tool that allows you to configure it, there's no need to upgrade the firmware unless you're into the nitty gritty details.
```

---
## \#8 Posted by: sl33py Posted at: 2017-07-02T01:14:09.733Z Reads: 53

```
Trying to update some old 4.07 VESC's, and don't have a correct BLDC Tool for the OLD fw1.10 they have now.  Going to setup for my brother - can someone send me the correct firmware for these if they have them?  Link or PM?  I'm using a new Ubuntu install and have the BLTC tool build correctly, but every time i try to update it closes the tool and nothing updates.

I'm much better on Windows... but missing something obviously.

Of course i have the new VESC Tool - but fw for 4.xx hasn't been released still...

While i'm asking - which firmware file is correct?  i see default, w33, 2811ws or similar, etc.

Thanks All!
```

---
