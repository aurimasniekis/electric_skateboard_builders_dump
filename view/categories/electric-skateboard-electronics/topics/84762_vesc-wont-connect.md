# VESC wont connect :(

### Replies: 21 Views: 1059

## \#1 Posted by: kobra918 Posted at: 2019-02-20T06:10:18.907Z Reads: 186

```
'Could not read firmware version. Make sure that the selected port really belongs to the VESC. '
This is the error message I get with both the BDLC tool and the VESC tool. It connects for a few seconds and then disconnects. I'm not sure on what to do and no google searches have helped me out. All help appreciated. Thanks in advance!
```

---
## \#2 Posted by: pookybear Posted at: 2019-02-20T06:12:43.273Z Reads: 182

```
Try a different cable.
```

---
## \#3 Posted by: Goonman Posted at: 2019-02-20T10:18:58.700Z Reads: 167

```
Pretty common. Change com ports wiggle cables turn VESC off and on then repeat until successful. Auto connect wizard works better than re-connect. And change cables.
```

---
## \#4 Posted by: CarlCollins Posted at: 2019-02-20T11:43:34.103Z Reads: 161

```
Make sure the following
1: Your USB cable is not charge only cable, it must have to be Data cable 
2: Make sure the COM port driver is registered in the system, In Windows See Device Manager (Under Ports and Coms)
3: If you get an Yellow triangle with ChibiOS in your Device manager 
please use below link to update the driver
https://drive.google.com/file/d/1ei5p-xRrJsaJiyP6jYGHhD0cMyFX8eqF/view?usp=sharing

Let me know if this helps, If you are still facing issues, I would like to help you virtually/remotely
```

---
## \#5 Posted by: briman05 Posted at: 2019-02-20T15:10:40.568Z Reads: 139

```
What @CarlCollins said a common cable that I have found that works is a PS4 remote cable.  That is what I used to configure my vesc.  Would be handy if enertion used one of the data cables as the charge cable for the nano-x remotre. Kill two birds with one stone.
```

---
## \#6 Posted by: CarlCollins Posted at: 2019-02-20T16:20:25.992Z Reads: 129

```
@briman05
As Original FOCBOX is no longer available now and Unity uses USB-C, I think we don't have to use data cable for NANO-X charging :slight_smile:
```

---
## \#7 Posted by: briman05 Posted at: 2019-02-20T16:32:21.595Z Reads: 118

```
True now but it would have definitely have been a help to have them included cause I bought both at the same time and found myself trying to find every micro usb and trying it and that is hard when I use all apple products
```

---
## \#8 Posted by: CarlCollins Posted at: 2019-02-20T16:35:32.753Z Reads: 115

```
I agree, That's really a hassle but if you are an Android user then you might be lucky
```

---
## \#9 Posted by: briman05 Posted at: 2019-02-20T16:39:59.299Z Reads: 116

```
Yeah but I prefer apple as I can air drop pictures and videos that I have edited on my mac right to my phone so it is easy to transfer large files.
```

---
## \#10 Posted by: kobra918 Posted at: 2019-02-20T21:14:07.145Z Reads: 107

```
@CarlCollins I tried all of the following but it still not connecting. It gives me the following messages with auto connect and manually connect PFA the images. Thanks in advance for all your help. 

![VESCfirmwareError|690x429](upload://831GHeTUIa2bHwPpPJfjG5xRlVi.jpeg) ![VESCError|690x371](upload://dlfjHNgajQwLuARjv0Lih078Gev.jpeg)
```

---
## \#11 Posted by: briman05 Posted at: 2019-02-20T21:27:10.872Z Reads: 88

```
What type of vesc are you using
```

---
## \#12 Posted by: kobra918 Posted at: 2019-02-20T21:47:54.611Z Reads: 88

```
It's a vesc 4.2 maytech I think .regardless, I solved the problem. It just needed a firmware update. For a sensorless motor though what mode is better (I'm using sk3): foc or bldc
```

---
## \#13 Posted by: pookybear Posted at: 2019-02-20T21:49:16.699Z Reads: 89

```
Are you trying to configure this while having two Vesc connected to your battery?

I found out that my split connector that connects two focboxs to the battery was faulty causing one focbox to have a solid red LED. What I did was disconnected one of them then plug the the otherit to the battery. I powered it on using my loopkey. Solid RED LED went away and connected right away to my PC.

I, since then, made another split cable (parallel) to power both of my focboxs.
```

---
## \#14 Posted by: kobra918 Posted at: 2019-02-20T22:30:18.390Z Reads: 83

```
nah its a single VESC
```

---
## \#15 Posted by: briman05 Posted at: 2019-02-20T23:19:02.507Z Reads: 83

```
I would do bldc unless you are using very conservative settings so foc doesn’t blow the vesc
```

---
## \#16 Posted by: kobra918 Posted at: 2019-02-20T23:46:20.793Z Reads: 83

```
Conservative in the sense low amp limits?
```

---
## \#17 Posted by: briman05 Posted at: 2019-02-21T00:03:39.237Z Reads: 83

```
Yes foc mode puts more stress on your mosfets compared to bldc.
```

---
## \#18 Posted by: kobra918 Posted at: 2019-02-21T04:57:41.913Z Reads: 82

```
ahh gotchu. Also, for the battery max current limit- what do I put in? I'm using a 12s 5000mah lipo (no bms) with 60-120c, so on paper that's a max discharge of 300-600A (correct me if I'm wrong). The vesc documentation says to ensure that the max battery current shouldn't be more than what the battery but does not mention the constraints on the VESC itself. Mine is rated for 50A max continuous current and a higher burst (I forget the number). So should the max battery current draw be < 50A?
```

---
## \#20 Posted by: epruski Posted at: 2019-08-15T00:38:50.722Z Reads: 52

```
Hello, I am having the same problem. But I’m not sure how to download drivers as when I look at device manager I have no COM ports at all. My vesc isn’t being recognized by the tool and I get the same connection error message that he stated too.
```

---
## \#21 Posted by: CarlCollins Posted at: 2019-08-21T23:21:15.724Z Reads: 45

```
Looks like you might be using Wrong cable or wrong port, please double check
```

---
## \#22 Posted by: Shawnl55 Posted at: 2019-10-27T22:41:58.511Z Reads: 21

```
I have the same problem but im on the unity app. It says it everytime i try to update the firmware. What do i do?
```

---
