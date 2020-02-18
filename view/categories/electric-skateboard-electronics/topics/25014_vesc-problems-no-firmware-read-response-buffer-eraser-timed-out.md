# VESC Problems, No firmware read response / Buffer eraser timed out

### Replies: 2 Views: 1106

## \#1 Posted by: Bluecro Posted at: 2017-06-10T07:05:03.007Z Reads: 143

```
Hello Im a newbie trying to connect my vesc to the BLDC Tool. 

When i push connect I get "No firmware read response"  
When I try to upload new firmware I get "Buffer eraser timed out"

I have tried connecting the other VESC, I changed the USB cable to the one provided, I have changed USB ports, I get the sound that it recognizes the connection when i turn it on, but a window pops up say not recognized, One of the usb devises attached to this computer is not recognized.

I have VESC v4.12, hardware v2.18. BLDC Tool supports v2.17, v2.18. 

Coms1 and Com3 show in box, Com1 works. 

I checked out "BLDC Tool not recognising my VESC - “No Firmware Read Response”
Esk8 Electronics thread but did not help.

Im at a loss, help would be much appreciated. Thanks
```

---
## \#2 Posted by: Bluecro Posted at: 2017-06-12T00:24:38.409Z Reads: 115

```
turns out I needed this driver, working now. 


http://www.st.com/en/embedded-software/stsw-link009.html
```

---
