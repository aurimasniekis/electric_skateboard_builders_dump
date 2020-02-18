# How to connect sensored motor to vesc? 6 pin to 5 pin

### Replies: 13 Views: 1187

## \#1 Posted by: jesser722 Posted at: 2017-05-26T22:03:10.625Z Reads: 180

```
My vesc is 5 pins, and my motor is 6 pins? What is the easiest way to convert it to a 5 pin? Also I think my remote is broken, when I ride now it goes slow then full throttle all of a sudden then I let go and 5 seconds after I let go of the throttle it stops. Its the winning remote, I have had it for a while and dropped it many times. Any one have ideas?
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-26T22:51:59.750Z Reads: 178

```
VESC is 6 pins

5v
TEMP
hall1
hall2
hall3
GND

In that order. Replace your remote, the winning remote is notoriously unreliable.
```

---
## \#3 Posted by: jesser722 Posted at: 2017-05-26T23:28:35.786Z Reads: 169

```
Which Remote would you recommend getting?
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-26T23:31:00.047Z Reads: 158

```
[mine](https://www.aliexpress.com/item/Electric-skateboard-refitting-parts-DIY-800MAH-remote-receiver-2-4G-bench-technology-benchwheel/32791243047.html?spm=2114.01010208.3.1.OLFotx&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10130_10068_5010017_10136_10137_10157_10060_10138_10155_10062_10156_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10096_10147_10052_10053_10107_10050_10142_10051_5170018_5020018_10084_10083_10080_10082_10081_10178_10110_519_10111_10112_10113_10114_10182_10185_10032_10078_10079_10077_10073_10123_142,searchweb201603_9,ppcSwitch_5&btsid=679f1b97-f2d2-4697-89df-81e2d2dbf621&algo_expid=ee4b1384-b12c-45bf-9360-e32e08438124-0&algo_pvid=ee4b1384-b12c-45bf-9360-e32e08438124) if you like thumb throttle

and if you like [trigger style](https://www.aliexpress.com/item/2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32735708994.html?spm=2114.01010208.3.74.swKMoD&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10130_10068_5010017_10136_10137_10157_10060_10138_10155_10062_10156_437_10154_10056_10055_10054_10059_303_100031_10099_10103_10102_10096_10147_10052_10053_10107_10050_10142_10051_5170018_5020018_10084_10083_10080_10082_10081_10178_10110_519_10111_10112_10113_10114_10182_10185_10032_10078_10079_10077_10073_10123_142,searchweb201603_9,ppcSwitch_5&btsid=71c8566a-3dd9-4cb0-99e9-16bba3b3f2d9&algo_expid=c0d1bd46-7730-4bf6-a16d-645c756ee07a-10&algo_pvid=c0d1bd46-7730-4bf6-a16d-645c756ee07a)
```

---
## \#5 Posted by: jesser722 Posted at: 2017-05-26T23:42:35.069Z Reads: 154

```
What does the sensored plug do?
```

---
## \#6 Posted by: jesser722 Posted at: 2017-05-26T23:42:53.489Z Reads: 154

```
Thanks for your help with the remotes
```

---
## \#7 Posted by: saul Posted at: 2017-05-27T01:02:44.667Z Reads: 150

```
mini remote on ebay is like half the price
```

---
## \#8 Posted by: jesser722 Posted at: 2017-06-23T02:32:22.422Z Reads: 131

```
I got the remote and it wont charge over the one out of three lights. Have you had any charging issues?
```

---
## \#9 Posted by: Jinra Posted at: 2017-06-23T07:20:07.274Z Reads: 126

```
what do you mean, it never charges? have you tried a different cable and brick?
```

---
## \#10 Posted by: jesser722 Posted at: 2017-06-23T07:41:29.167Z Reads: 121

```
Its stays at 1 bar. It keeps breaking up with my board. Are your u from santa monica?
```

---
## \#11 Posted by: yaca Posted at: 2017-06-23T20:26:48.998Z Reads: 114

```
Not sure if I understand your words. Just one light is shining while charging or after charging? At the end of charging all five lights have to shine and it ends with only the upper LED is shining.  While using the remote only the lowest LED  will shine, that's normal. And also one of the upper two lights will shine for the mode you choosed. 
What do you mean with "it keeps breaking up my board"?
```

---
## \#12 Posted by: jesser722 Posted at: 2017-06-23T23:08:51.673Z Reads: 110

```
I have charged it with several different chargers and it stays like this: <img src="/uploads/db1493/original/3X/8/7/871991facec2ad9f5a73b4a9ddff888ea5c8693f.jpg" width="375" height="500">

It keeps disconnecting from the board and sometimes it will go full throttle and go by itself. Thankfully it stops after a second. Really frustrating.
```

---
## \#13 Posted by: yaca Posted at: 2017-06-24T08:35:09.223Z Reads: 99

```
If you made the picture after charging without cable and turned on then it is alright. I was also confused with this after I charged my remote the first time. While charging all five lights have to shine or blink.

About the other problem. Be sure your pulsewith in BLDC Tool is set correctly. Click on "Display" and have a look on the green bar (maybe blue if you use mac). Full Throttle must be 100% green bar, full brake is 0% no green bar. Now turn off the remote and the green bar has to be at 50%. If not you have to adjust max and min pulsewith. Btw. with @ackmaniacs firmware 2.54 you also can adjust centre pulsewith, so it's a bit easier.
I would try to rebind the remote with the receiver and for a test try to place the receiver on the outside of the enclosure to be sure there is no problem with shielding. If nothing helps contact your supplier.
```

---
