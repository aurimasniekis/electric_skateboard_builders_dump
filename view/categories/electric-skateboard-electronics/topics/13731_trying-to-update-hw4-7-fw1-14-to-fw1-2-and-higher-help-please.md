# Trying to update HW4.7 FW1.14 to FW1.2 and higher. Help Please

### Replies: 2 Views: 443

## \#1 Posted by: chuttney1 Posted at: 2016-11-27T01:30:11.600Z Reads: 32

```
I've updated firmware from 1.10 on my VESC to FW.1.14 from a repository on Windows. I want to update to FW1.2 and higher by the files for HW4.7 is not in the folder. So I'm doing the firmware updates through ubuntu version 14.04 LTS. I'm running into the "can't assert SRST".  I want make sure each update from FW1.2 is not going to break the DRV8302 chip because programming is specific to hardware version 4.7. 



Old VESC FW repository: http://vesc.net.au/BLDC-TOOL/Firmware/OLD%20Firmware/

<img src="/uploads/db1493/original/3X/b/f/bf59129949a56cdcd66c1350053c8a521b9ab7c4.png" width="690" height="387">
```

---
## \#2 Posted by: chuttney1 Posted at: 2016-11-27T07:01:11.467Z Reads: 14

```
I solve this issue because it has to deal with the communication of USB to VESC through the Terry Guo; PPA- gcc-arm-embedded code. The version used in Ubuntu 14.04 LTS is "deprecated" or not in used such that I had to Vitualbox install Ubuntu 16 LTS to get me a working firmware update because to the updates to the repository to the "gcc-arm-embedded" code were not working for 14.04 LTS. The other thing I kind of forgot is Virutalbox does not connect automatically connect USB devices to the virtual environment. You must right click the USB stick icon and left click the USB device to be use. Let this be information to any unknown user who comes across this...
```

---
