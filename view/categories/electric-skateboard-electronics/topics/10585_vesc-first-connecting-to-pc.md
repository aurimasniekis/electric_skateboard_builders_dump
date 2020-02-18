# VESC first connecting to PC

### Replies: 3 Views: 550

## \#1 Posted by: ninja Posted at: 2016-10-03T19:34:28.971Z Reads: 65

```
Hi builders!

 I'm just about to finish my first build, but i really don't know how to program VESC, i just don't want to blow up my VESC. My set up will be 8s lipo 8000mah, sk3 245kv and VESC 4.12. 
 
So should i use 8s lipo for connecting to PC or better do 4s lipo or other power supply? If 4s is fine, then what will happen with numbers i should write in BLDC TOOL, i mean, i  still need write numbers as it for 8s?
Where i should download BLDC TOOL?  http://vesc.net.au/download-now/1 down load botton for windows is not working, but i tried to click on Old Versions, than click on Parent Directory, than click on BLDC_Tool.exe. Is this BLDC_Tool.exe is fine or it's too old? What about those firmware bugs, do they still exist? Thing is, that i want download right BLDC TOOL and firmware, how i can know which has bugs in it?
```

---
## \#2 Posted by: Namasaki Posted at: 2016-10-04T03:06:44.056Z Reads: 39

```
I just tried the windows download and it works.
when you get to the donation page, scroll down to the bottom and click the blue download button on the left.
When the next pop up window appears, put in your email address and click then the download will start.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-10-04T03:11:14.604Z Reads: 39

```
The current ramp bug is in the firmware on the Vesc. Download the newest version of BLDC tool and the firmware files that come with it. Then before programing the vesc, update it to the new firmware using the bldc tool.
Flash it with the VESC_default firmware file.
```

---
