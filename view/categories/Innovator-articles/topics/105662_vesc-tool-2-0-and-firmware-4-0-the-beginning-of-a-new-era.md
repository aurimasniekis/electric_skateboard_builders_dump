# VESC-Tool 2.0 and Firmware 4.0 - The beginning of a new era

### Replies: 3 Views: 281

## \#1 Posted by: trampa Posted at: 2020-01-29T23:05:38.745Z Reads: 80

```
**VESC-Tool 2.0 and Firmware 4.0 - The beginning of a new era** 

The year 2020 started with a super intense coding session in Nottingham. Miserable weather, tons of perfect mud in the Colwick Woods, hardly any chance to go for a proper ride... Our special guests Jeffrey Friesen and Benjamin Vedder decided not to get bored while waiting for ridable conditions. The outcome was a new exiting feature called **H**igh **F**requency **I**njection, also known as signal injection.

**HFI**:
HFI sounds very technical and doesn't immediately give you an idea what it does.

Basically it does give you high torque startup without cogging, even if your motor has no sensors.
A lot of motors don't come with sensors and a lot of sensored motors get sensor issues over time.
HFI is a nice fall back strategy for broken sensors and an excellent way forward for sensorless motors. 
At this stage you will hear a bit of a high frequency noise for a second, before the Back EMFs kick in and signal injection is switched off. Sensorless startup will work best on three shunt designs as far as I understood. 

@Deodand will probably tell you more about it all in this thread.  

**What else is new in VESC-Tool 2.x**

**Support for old firmware:**
VESC-Tool is now supporting older firmware. If your system is running fine and you are happy, things can stay as they are. You will get a message like this:

*The connected VESC has old, but mostly compatible firmware. It is recommended to update it for the latest features and best compatibility.*

VESC-Tool will not force you to update the FW, while allowing you to run the latest software tool. The support for really old firmware is not given at this stage, but at least 3.55 onwards will see support. If your firmware has a bug, you will see a WARNING and a brief description of the bug (e.g. FW 3.63 and 3.64). In such a case, please update even if you haven't experienced issues so far!

**Dynamic User Interface**:
New features often come with new user interface entries and options to choose from. If you use old firmware, you will not see options that are only available with later firmware versions. The user interface will adapt to your firmware. This feature was needed to make old firmware work in combination with a newer VESC-Tool software. 

**Back up of your entire configuration (ConfBackup):**
One thing that was a bit annoying in the past was the need to re-run the setup wizards each time you do a firmware update. This is now solved via configuration backups, which are assigned to the UUID of the ESC. You can save the entire configuration prior to a firmware update and then restore it after the FW update finished. Everything stays exactly as it was before the update, for all VESCs in an array. VESC-Tool 2.0 had a little glitch with this feature. This is now resolved with the 2.01 version.


**An outlook for 2020:** 
Jeffrey and Benjamin will try interact a lot more in future. We will probably see support for ESC designs using a shared processors for two ESCs. If you own a Unity for example, support for it is probably happening in a overlookable time frame. This way such devices get a future and do not suffer from lack of software updates, making them obsolete sooner than later. The integration of single processor support also allows new and potentially interesting HW designs. Please note that the amount of work to make this happen is not little. Give it some time! 

There are also plans to make something happen for the Apple users. More to be announced once more thought is put into it. There are several options on the table to go forward on this matter....



**Here are two videos with tons of more information:**

https://www.youtube.com/watch?v=TFKGRyOmhWY

https://www.youtube.com/watch?v=-qV1_xyrgzs



**Please consider a donation to Vedder to keep him motivated and to allow further software development.**

VESC-Tool 2.x can be downloaded here: 

https://vesc-project.com/vesc_tool

https://play.google.com/store/apps/details?id=vedder.vesctool&hl=de
```

---
## \#2 Posted by: JohnA Posted at: 2020-01-30T18:39:25.048Z Reads: 53

```
Thanks for sharing @trampa. Beautiful update, was nice BV was willing to take the time to make a video discussing the theory behind the HFI sensing. Is the HFI also supported on 4.xx hardware versions or just 6.xx and up?
```

---
## \#3 Posted by: trampa Posted at: 2020-01-30T20:11:30.401Z Reads: 47

```
At this stage it should work with 4.xx and 6 HW.
```

---
