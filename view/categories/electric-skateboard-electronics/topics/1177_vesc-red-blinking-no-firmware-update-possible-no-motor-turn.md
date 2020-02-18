# VESC red blinking no firmware update possible no motor turn

### Replies: 25 Views: 4866

## \#1 Posted by: Flo Posted at: 2016-01-31T01:21:14.376Z Reads: 233

```
I just started to work with my VESC two days ago. I used the windows BLDC tool. At first everything seemed nice. I soldered the wires and the capacitor to the board. Then I connected a 12V battery to start with low voltages. My computer could connect to the VESC (4.7) and I could upload the newest firmware. After uploading the newest firmware the VESC disconnected automatically. I just could reconnect it after shutting the VESC down and after powering it again I could get it connected to the BLDC tool again. But the firmware didn't update at all. I repeated that step sometimes but I couldn't get the VESC FW updated. It worked exactly like that every time. I think the bootloader is perhaps not flashed right. So I ordered a stlinkv2.
Afterwards I connected my motor to the VESC and decided to start working with the BLDC Tool for FW 1.10. I read the configuration and Uploaded the configuration for the turnigy sk3 168kv. Afterwards I shut down the VESC again, then powered it up again. Connected it to the BLDC tool again. Read all values. They were stored and everything looked good. 
I wanted to start turning the motor. So I pressed the left button on the keyboard. The motor started turning and immediately stopped. The red LED immediately started flashing three times in a row. Then around a second pause and flashing three times again. That happens every time I repower my VESC.
When looking at the Real time Data tab and enabling 'activate sampling' it gives back a fault code: DRV8302.
Additionally I wonder why the Mosfet temp is 40°. 
I'm glad for every help :)
```

---
## \#2 Posted by: chaka Posted at: 2016-01-31T02:03:17.513Z Reads: 224

```
It looks like you may have uploaded the firmware for version 4.10/4.11 hardware. Incorrect temp readings are a sure sign of this. Hopefully you did not burn a trace on the PCB. luckily you were only using 12v so the PCB is probably fine but you will need a new DRV8302 chip.
```

---
## \#3 Posted by: Flo Posted at: 2016-01-31T09:04:26.547Z Reads: 215

```
I always used the VESC_default.bin out of the folder hw_46_47. So never any FW for hw 4.1 or 4.11 Of Course I tried to upload the firmware 2.8. But I also tried to update to older versions for hw_46_47. And as I mentioned the BLDC Tool never succeded in updating the firmware. After reconnecting the BLDC Tool just recognizes FW 1.10. So it seems my DRV8302 already seemed to be broken when arriving? Does anybody think it looks like a change of the DRV8302 could solve all my problems?
```

---
## \#4 Posted by: Flo Posted at: 2016-01-31T09:26:59.941Z Reads: 203

```
here some pictures of my vesc:
<img src="/uploads/db1493/original/2X/5/576830f2e9ef2ae79e56638d411979fa4e991dcc.png" width="690" height="387">
<img src="/uploads/db1493/original/2X/f/f453bf374d96012bac4e2377486050eb8e3d8622.png" width="280" height="499">
and here some screenshots of my bldc tool: 
(I just reduced some current limits for my motor)
<img src="/uploads/db1493/original/2X/8/89724b633119695b7dd8752180546298dd2315ab.png" width="690" height="388">
<img src="/uploads/db1493/original/2X/c/c15963e2c76a2c0f2fa91a88eb5c204f727c2f82.png" width="690" height="371">
and here of the firmware tab:
<img src="/uploads/db1493/original/2X/d/d11fbcd3045efc3693583a71dc57f79df5e82448.png" width="690" height="371">
```

---
## \#5 Posted by: EnertionSupport Posted at: 2016-01-31T15:27:07.028Z Reads: 190

```
[quote="Flo, post:1, topic:1177"]
I just could reconnect it after shutting the VESC down and after powering it again I could get it connected to the BLDC tool again. But the firmware didn't update at all. I repeated that step sometimes but I couldn't get the VESC FW updated. It worked exactly like that every time. I think the bootloader is perhaps not flashed right.
[/quote]

The incorrect firmware update is probably what caused your failed DRV8302 chip. Incorrect settings will often lead to this failure.

As @chaka said, you should be able to get back up and running with a new DRV chip; props for using a power supply and not just a lipo!
```

---
## \#6 Posted by: Flo Posted at: 2016-01-31T16:00:40.207Z Reads: 188

```
As far as I read through the forum until now the failed firmware update is due to an improperly flashed bootloader. But the boards of others worked fine in the BLDC tool for FW 1.10. Even after failed FW updates. My board already had a hot MOSFET and immediately stopped turning the motor. I'm concerned that there is more wrong... (Compare to the thread I posted at first: Enertion vesc flashing pink light - failed motor detection DRV8302 error) 
Did that VESC already arrive at you and you figured out the failure? I would guess perhaps my board has the same issues…
After these people flashed the Bootloader again they could update the FW and everything worked fine. At least I read it several times. 
Ok I'll see to get a new DRV8302 and find someone to solder it to the board for me. Afterwards I have to flash the bootloader and install the FW again? I don't have ubuntu. Is there any possibility to flash the bootloader with windows and then install the firmware again?
Sorry what do you mean by:  props for using a power supply and not just a lipo!
I didn't use a power supply. I used a 12V car battery.
Do I need the DRV8302DCA or DRV8302DCAR chip?
I'll try my best to get it working again. The new chip needs around 10 days to deliver. I hope if none of these steps is successful I can get a replacement VESC. I’ll keep you up to date on my repairing process.
```

---
## \#7 Posted by: hexakopter Posted at: 2016-01-31T16:12:24.946Z Reads: 178

```
[quote="Flo, post:6, topic:1177"]
Do I need the DRV8302DCA or DRV8302DCAR chip?
[/quote]


The R stands just for reel and means the package they come with. So the IC is identical, so go with the cheaper one.
```

---
## \#8 Posted by: Flo Posted at: 2016-02-06T19:32:09.043Z Reads: 163

```
So. Until now I didn't replace my DRV8302. Still waiting for a new chip. I bought a stm32 discovery board and installed ubuntu on my computer. So I was able to successfully update the bootloader and the firmware. Afterwards the VESC also stopped blinking red. I have a turnigy aerodrive 149kv with the VESC. So I read in the mc_config Data for turnigy aerodrive 168kv. The difference between these Motors is not too huge. 
The Failt code also disappeared and my Mosfet is quite cool now :) 
My problem now is that the Motor doesn't turn at all when being connected to the BLDC Tool and hitting any up/down/left/right key... 
I tried the automatic Motor detection to get it turning. That also didn't succeed in letting the Motor turn... It just says detection failed...
Please Help. 
<img src="/uploads/db1493/original/2X/8/862fd07e5d5816361d0201e0a3440ea1caa32297.png" width="690" height="428">
```

---
## \#9 Posted by: elkick Posted at: 2016-02-06T20:01:26.613Z Reads: 136

```
Since it's a red PCB: did you purchase this VESC in May/June last year? If so, it would be from the flier batch...
```

---
## \#10 Posted by: Flo Posted at: 2016-02-06T20:09:04.282Z Reads: 142

```
I ordered it the 13th July 2015. It arrived middle of September in Germany. I was studying abroad so I just returned and started working on it... 
The flier batch was mainly good or bad?
Another strange thing is that the BLDC Tool shows a motor current of 0.7 Amps with a battery current of 0 Amp and the motor is not being turned... 
<img src="/uploads/db1493/original/2X/e/e985856c826eeed9947472704feaa62634008190.png" width="690" height="353">
```

---
## \#11 Posted by: elkick Posted at: 2016-02-06T20:31:42.772Z Reads: 146

```
The flier batch was faulty, that's why Jason stopped working with them for esc's. 

Yours is definitely from the second batch (not flier) and this one is ok. I'm still driving that one myself and it works well. The bootloader was missing, so I uploaded it myself (like you did). 

Did you check your capacitor if it is soldered well and working? Another try would be to adjust the detection parameters for the motor detection before hitting detect. 

To be honest, I don't think it makes much sense to use others motor values (the xml files), it's always recommended to detect the correct values of a motor on your specific one.
```

---
## \#12 Posted by: Flo Posted at: 2016-02-06T20:44:07.230Z Reads: 140

```
[quote="elkick, post:11, topic:1177"]
Yours is definitely from the second batch (not flier) and this one is ok. I'm still driving that one myself and it works well. The bootloader was missing, so I uploaded it myself (like you did).
[/quote]

I changed the motor values several times bevore hitting auto detection but it just gave back detection failed. I tried to increase the current until 10A and decrease the min ERPM until 150 but the motor wasn't intereseted in anything and refused turning. When looking in the Realtime Data while the Auto detection worked the Battery current stayed at 0 and the motor current was mostly around 6 A and sometimes a little higher... I also increased low duty until 0.15
```

---
## \#13 Posted by: elkick Posted at: 2016-02-06T21:15:33.130Z Reads: 132

```
I only had the effects you are describing once, it turned out that it was related to a bad power connection. Can you try a detection again with another motor?
```

---
## \#14 Posted by: Flo Posted at: 2016-02-06T21:30:46.596Z Reads: 129

```
I'll get another motor from a friend for testing in some days. But I'm not very optimistic...
```

---
## \#15 Posted by: Flo Posted at: 2016-02-07T01:04:04.446Z Reads: 129

```
this is the screenshot of 5A in the motor and no battery current ... perhaps that helps somebody solving my issue? 
<img src="/uploads/db1493/original/2X/9/906453e150d6451ad43102ce17e38c5d830f201c.png" width="690" height="427">
```

---
## \#16 Posted by: Flo Posted at: 2016-02-07T11:17:14.320Z Reads: 124

```
rewired my power connection, checked that nothing is shorted, checked my capacitor and moved it really near the board but did't solve the problem...
Pressing full brake button in BLDC tool also shows no effect... Thats strange because I thought full brake is just shortening all three phases... when physicly connecting the three phases motor is really hard to turn. When pressing full break in BLDC tool there is no difference in motor behavior...
```

---
## \#17 Posted by: Flo Posted at: 2016-02-08T04:12:40.700Z Reads: 127

```
Yesterday I recognized that some Pins of my DRV8302 are shortened. But never 2 Pins that are directly in use. 
Do some VESCs have some pins of the DRV8302 connected and they are still running? 
Is it sufficient to remove the connection between the pins?
As the newest firmware doesn't detect any DRV8302 failure code is it still necessary to change the DRV8302? 
As I haven't been at that place with my soldering iron the VESC already arrived with shortened pins of the DRV8302...:S 
<img src="/uploads/db1493/original/2X/d/d8fccff96bda7a90a3cffbce2fce5ae89d1566d1.JPG" width="690" height="460"><img src="/uploads/db1493/original/2X/b/b8fe4e65ac6976cbf61b82cd9bb2b8e527d6a32c.jpg" width="690" height="460">
```

---
## \#18 Posted by: Blasto Posted at: 2016-02-08T04:45:22.420Z Reads: 114

```
Not sure if you have a short on the left, but if you do it's not supposed to be there.

The 2 shorts on the right is perfectly normal. That should be documented somewhere in a faq
```

---
## \#19 Posted by: Flo Posted at: 2016-02-08T14:51:57.178Z Reads: 118

```
Yes I have and you're right there shouldn't be a short.... 
<img src="/uploads/db1493/original/2X/2/261ff142461387826042bc7637d1ad920233ee35.JPG" width="690" height="460">
So. Just returned from the university laboratory. I got help to disconnect the two shorted pins and measure all the chips on the board. Afterwards the motor controller still didn’t work. And it is very clear why. The connection connected the en_gate pin which can handle only up to 7 V with the cp2 charge pump pin. So the charge pump killed the en_gate pin and so the whole drv8302 and it also killed the pin of the CPU. The CPU can’t any longer set the en_gate high and perhaps even more broke.
Clearly a production failure which caused the complete VESC to fail…!
@EnertionSupport :  Do you still want the messed up board back or will you just send a new one?
```

---
## \#20 Posted by: Flo Posted at: 2016-02-10T20:40:43.111Z Reads: 110

```
I would be super happy to get an answer from Enertion Boards to my warranty request... :blush: 
Sorry for my impatience. Can't wait to finally ride my ebike...
```

---
## \#21 Posted by: onloop Posted at: 2016-02-10T23:01:17.443Z Reads: 107

```
sorry man, at the moment i don't have time to read every thread on here. if you are emailing my support account ill have a word with my support guy to see why he isn't responding.

did you submit and RA?
```

---
## \#22 Posted by: Flo Posted at: 2016-02-10T23:04:19.446Z Reads: 106

```
Thank you so much :)
RA=return request? I already did a return request online in my enertion board account.
```

---
## \#23 Posted by: Flo Posted at: 2016-02-11T18:16:36.498Z Reads: 103

```
@EnertionSupport are you still alive??
```

---
## \#24 Posted by: OGP Posted at: 2016-02-14T20:49:32.871Z Reads: 99

```
Besides asking a vendor, how do you know which version of the VESC you have?  Are there any obvious markings?
```

---
## \#25 Posted by: elkick Posted at: 2016-02-14T20:51:07.029Z Reads: 99

```
Yes, on the PCB itself.
```

---
