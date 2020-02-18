# Need help updating my Maytech VESC&rsquo;s and programming everything with macbook

### Replies: 6 Views: 821

## \#1 Posted by: mxrider9239 Posted at: 2018-04-21T04:18:06.198Z Reads: 72

```
hey guys I'm having trouble figuring this all out. I'm all ready to set up my board and i currently have the BLDC tool on my macbook but my firmware on my vest's are out of date and i have been trying to figure out how to update them but no luck. if i can have this all set up within the next day or so id finally be able to ride my build!
```

---
## \#2 Posted by: goldrabe Posted at: 2018-04-21T04:42:59.713Z Reads: 70

```
If you ordered your vesc directly from Maytech then they have likely no bootloader installed. I had the same issue. In the older days you where out of look at this point, but with the new Vesctool, which you can download directly from Benjamin Vedders Vesc Project page, you are able to install the bootloader just over your usb connection.
Follow,all the steps thoroughly provided by the wizards inside the Vesctool.
Upload the bootloader and after that update your firmware. Make sure that you choose the firmware for 4.12 hardware, update the firmware, then the vesc will automatically disconnect. After disconnection wait a few seconds untill the vesc boots again and you computer recognizes the vesc, connect the vesc again in the Vesctool and check the firmware version.
Thats the way I did it in Win10, but I guess with mac it is quite similar.
```

---
## \#3 Posted by: Scoo_B_SK8 Posted at: 2018-04-21T04:44:43.686Z Reads: 66

```
http://www.electric-skateboard.builders/t/how-to-programm-flash-a-new-born-vesc-4-12-with-st-link-v2-widows-10/52813

http://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103?source_topic_id=52813

reading this might help?
```

---
## \#4 Posted by: mxrider9239 Posted at: 2018-04-21T04:58:41.168Z Reads: 58

```
thanks for the links but it looks like everything is for windows. is there any write-ups where people use a macbook?
```

---
## \#5 Posted by: pat.speed Posted at: 2018-04-21T05:00:01.561Z Reads: 56

```
Try using a windows opener thing, I’m not sure what it’s called but it basically boots your Mac as a windows, I remember doing it a while ago
```

---
## \#6 Posted by: lock Posted at: 2018-04-21T05:15:42.898Z Reads: 53

```
There's really not a lot of difference between how you do it on Windows/Linux/MacOS once you get the VESC Tool running. You do have a few options though.

Easiest would be to download the VESC Tool build by @rpasichnyk for MacOS. It'll run directly on your Macbook.
https://github.com/rpasichnyk/vesc_tool/releases

Alternatively you can install a virtual machine (eg; [VirtualBox](https://www.virtualbox.org/wiki/Downloads)) and run either the Windows or Linux version downloaded from the [official site](http://vesc-project.com/). Would recommend using Linux (Ubuntu) as this way you wont need a Windows license. This is a fair bit more work, and you'll need a large amount of free disk space.

Whichever option you choose you may also need to install [some USB drivers](https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers).
```

---
