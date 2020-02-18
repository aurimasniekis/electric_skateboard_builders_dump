# How to factory reset the VESC

### Replies: 8 Views: 1582

## \#1 Posted by: benslmn Posted at: 2017-06-13T20:29:23.441Z Reads: 160

```
My electric skateboard just stopped working the other day and everything is connected and the batteries are charged. How do I factory reset the VESC to its original settings and firmware?

From my experience, something like this is usually software/firmware related if everthing else works.
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-13T20:38:18.603Z Reads: 161

```
You can click 'read default' at the bottom of the BLDC tool and then apply the settings. You can then go back in and select the original firmware.

That would be the only way I can think of to 'factory reset' the vesc
```

---
## \#3 Posted by: Tampaesk8er Posted at: 2017-07-13T11:10:52.054Z Reads: 121

```
Is there any other ways to factory reset a 4.12 VESC?
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-07-14T17:21:32.180Z Reads: 107

```
Reflash firmware?
```

---
## \#5 Posted by: Tampaesk8er Posted at: 2017-07-14T17:50:28.053Z Reads: 100

```
Thank you, I did reflashed the firmware and it worked. Thankfully I had saved the files to flash and update firmware (4.10, 4.11, 4.12) on my pc.
```

---
## \#6 Posted by: t0m_r1dd1e Posted at: 2017-07-14T17:51:17.694Z Reads: 98

```
Nice. Glad it worked for ya
```

---
## \#7 Posted by: flaviuschris4 Posted at: 2018-04-19T18:13:12.366Z Reads: 76

```
how do you reflash the firmware?
```

---
## \#8 Posted by: wafflejock Posted at: 2018-05-14T22:15:50.814Z Reads: 57

```
Using the vesc_tool you can flash new firmware over usb connection from any computer.  Make sure the hardware version you select matches your real hardware and you should see a few options.
```

---
