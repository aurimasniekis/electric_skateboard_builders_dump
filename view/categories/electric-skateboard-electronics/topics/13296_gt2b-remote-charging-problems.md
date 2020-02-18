# GT2B Remote Charging Problems

### Replies: 2 Views: 694

## \#1 Posted by: JdogAwesome Posted at: 2016-11-19T01:02:20.617Z Reads: 57

```
Im working on constructing my Bad Wolf remote and im almost done except im having problems charging it. Right now it turns on fine and it works but when I try to charge it via the micro USB port (swapped from mini usb) it changes the polarity to the battery and triggers the battery's BMS circuit. Ive checked the polarity of the connections on the micro USB port and on all other connections and there all correct its just reversing the polarity for some reason. If anybody has any idea son why its doing this that would be great.

Also if anyone wanted to know the GT2B draws around 60mA consistently. And if the battery it comes with is really 800mAh you should get a run time of around 13 hours, which is pretty impressive for this little thing.

<img src="/uploads/db1493/original/3X/4/c/4cc765cad2ba26fba726bb09f25fd9ed70656cc8.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/8/c/8caa618745d4a041b9b8252097892b784078032f.jpg" width="690" height="388">
```

---
## \#2 Posted by: JdogAwesome Posted at: 2016-11-19T05:17:02.684Z Reads: 40

```
So I wasn't able to figure out was causing the reverse polarity, so I decided to bypass the remotes charging circuit and add my own. I used a simple single cell USB LiPo charger like [this](http://www.ebay.com/itm/TP4056-5V-1A-Mini-USB-3-7V-Lithium-Battery-Charging-Board-Lipo-Charger-Module-1S-/122218139555?var=&hash=item1c74c4cfa3:m:mMb8xb-CXRHVOxwW4Z38ONg) one to do so. Its pretty simple just setup my micro usb input to go to the charger instead of the remote and spliced the battery wires. Also [this](http://www.gearbest.com/other-accessories/pp_336948.html) is the micro USB breakout board I used.

<img src="/uploads/db1493/original/3X/5/0/50d6e18587f243c1c420887d70f4e03c1c4e5b7e.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/0/4/04c8b3115e4d84e6c6003c72e429efb26f7c5607.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/3/2394c78179c6e21aced7d96a422b4f2e3d2760e3.jpg" width="690" height="388">
```

---
