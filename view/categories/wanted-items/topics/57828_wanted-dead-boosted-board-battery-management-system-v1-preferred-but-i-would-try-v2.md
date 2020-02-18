# Wanted: Dead boosted board battery management system V1 preferred but I would try V2

### Replies: 47 Views: 2281

## \#1 Posted by: Drm5602 Posted at: 2018-06-04T19:57:14.266Z Reads: 264

```
My boosted board v1 bms system took a dump on me. I already took the battery apart and tested and replaced the dead cells but It still gives me the 1 long 3 fast red flashes. So I'm looking to replace it with another bms if anyone has one they're not using. Or if anyone knows where I can purchase another bms that would be helpful. I'll take dead packs and disassemble them myself or if you have just the bms itself that would be great. I live in San Jose California if that makes any difference. If its worth anything I want to try and connect one of these bms to 12 headweay 38120 8ah cells to see if it works with them. 
Thanks in advance.
```

---
## \#2 Posted by: Tunda Posted at: 2018-06-08T06:14:21.574Z Reads: 224

```
I got one!
```

---
## \#3 Posted by: Tunda Posted at: 2018-06-08T06:19:26.485Z Reads: 220

```
![image|375x500](upload://ebc1ocmzGyk7wd581SYcrhLHCYm.jpeg)![image|375x500](upload://92vmakYwbUKi2X48AQLeN22vBId.jpeg).  
Is this what you looking for!
```

---
## \#4 Posted by: Tunda Posted at: 2018-06-08T06:20:12.050Z Reads: 212

```
It’s a v1🤙🏼
```

---
## \#5 Posted by: Drm5602 Posted at: 2018-06-11T21:25:31.388Z Reads: 205

```
Yes! that is what I'm looking for.
```

---
## \#6 Posted by: walleywalker Posted at: 2018-07-19T01:31:12.433Z Reads: 191

```
Any thoughts on if a supplimentary board could be wired to the CAN bus to fake communication with the BB ESC?   That way letting you run BB batteries on any AM setup..
```

---
## \#7 Posted by: Drm5602 Posted at: 2018-07-21T20:42:55.380Z Reads: 180

```
So i'm trying to figure out the protocol to have an aftermarket BMS connect up to the ESC. I'm talking to best tech about their CAN BMS. I'm currently trying to gather more information about the CAN setup since the factory BMS sends a signal for it to work and another signal the same time to give battery level to the remote. The V1 BMS I received from Tunda(Thanks again! Tunda!) works enough that it allows me to operate the board without the battery level. However it just keeps beeping as if the board is out of battery. It also doesn't have balance discharge of the twelve cells. I don't have the hardware to connect the BMS to my computer yet but i'm trying to get one with two of the CAN BMS that Best tech sells. Have you tested with any this stuff yet? I'm slowly going through this since I'm learning as I go.
```

---
## \#8 Posted by: Elitejarcool Posted at: 2018-08-27T09:56:38.602Z Reads: 157

```
Hey progression on what information is being sent by the bms, l have a v1 with a broken bms aswell and l have same issue and l trying t ok workout what l can do to retain the same main board. Any new information or  discovery of supplyers that would help
```

---
## \#9 Posted by: mikegeezy Posted at: 2018-09-05T07:25:25.846Z Reads: 150

```
Howdy folks, I've also gotten interested in CAN Bus sniffing lately.  My battery got below the threshold where the BMS would charge it, and rather than follow the recommended guidance to push it around until it would charge, I decided it would be better to tear into it with a claw hammer in a drunken rage.  The aftermath was pretty ugly - that battery is NOT user serviceable.  

Anyways I built this 3D printed caddy and replaced half the cells, wired it all back up and it's still not 100%.  As soon as you power it up, it starts beeping BUT power is available and the wheels will move for maybe 10 sec, then it starts flashing orange and the power cuts out.

I bought the hardware to perform CAN bus sniffing.  It's pretty cheap, all you really need is a raspberry pi and a little interface card.  Then can-utils is your friend.  I got to the point where I was pulling data from the bus and will try to post something when I get home around Sep. 23rd.  Eventually I would like to get a Arduino mini that just broadcasts out a "HEY EVERYTHING IS FINE" on the can bus, and an XT90 connector so I can use any battery I want.  I expect the ESCs will operate OK on a pretty wide range of voltage if you don't mind taking a top speed hit.

https://imgur.com/pwuE3oy
https://imgur.com/EMxasIb
```

---
## \#10 Posted by: tarpan Posted at: 2018-09-12T14:13:50.286Z Reads: 130

```
mikegeezy, i have a boosted v1 with similar issue. can you share what that 'everything is fine' can bus looks like and how you got your arduino programmed to send it to ESC? i think paying $500 or $600 to boosted people for repair is unreasonable and i would love to use that board few more seasons. i don't care if i see how much battery is used. i just want ESC to engage and drive. Thanks
```

---
## \#11 Posted by: Drm5602 Posted at: 2018-09-13T01:04:00.480Z Reads: 122

```
Hey, I just recently ordered the CANBUS sniffer gear. Sounds like I went the same route Mikegeezy with the hardware I ordered. However, I'm also trying to fix either of the original BB1 BMS to have a fully working BMS to read. Besttech has a selection of Canbus programmable BMS but I just haven't gotten deep into this yet to see how it would work out. http://bestechpower.com/communicationbms/
But who knows if it'll work. Anyone on these forums a CANBUS whisper who could point us in a more educated route? 
Oddly though with one BMS I can run the board for a while having just the new battery leads connected into the BMS (BMS connected as intended except I didn't connect the balance wires, still has the annoying beeping for the 15 minutes I rode it) and on the other hand, the other BMS will give me, absolutely no power to the motor but the remote does show connection.
```

---
## \#12 Posted by: mikegeezy Posted at: 2018-09-13T15:49:39.984Z Reads: 115

```
Good stuff.  I'm glad to see there's some interest in this.  It seems silly to me that all the V1's were essentially designed to be bricked once the battery reaches end-of-life.  Expect we are not the only ones who are going to face this problem.  That's a sweet find on that CANBUS programmable BMS.  I didn't realize such products existed.  That could potentially open up an aftermarket for these batteries.

The more folks we have sniffing the bus and comparing different addresses / values for different situations etc, the better off we'll be for decoding what's what.  Will post more on how to get the data and whatever I can pull when i get home week after next.

Cheers.
```

---
## \#13 Posted by: mikegeezy Posted at: 2018-09-24T16:54:22.703Z Reads: 108

```
OK Folks, I've got some more details and a CANDUMP log file to post.  I followed the tutorial here:

https://harrisonsand.com/can-on-the-raspberry-pi/

(I think there's a typo on the ifconfig command to check that it's connected, I could only get a response using "ifconfig can0" but don't get hung up on it.  Also using 3.3v instead of 5v - not really sure why.)

The baudrate i'm using is 500,000.  I could not get the cansniffer command to work, or display any real data. 

So I'm just posting a candump below, and a couple of youtube videos

https://youtu.be/StHVfY2R4Fw
https://youtu.be/T1d3EdXCjRI
 
    (1537729469.530625) can0 0B57ED01#9402000020140414
    (1537729469.530863) can0 0B57ED02#0000070009000000
    (1537729469.531150) can0 0B57ED03#000000000F00FF00
    (1537729469.630721) can0 0B57ED01#9402000020140414
    (1537729469.630997) can0 0B57ED02#00006B0009000000
    (1537729469.631285) can0 0B57ED03#00000000271C0000
    (1537729469.730598) can0 0B57ED01#940200001C140B14
    (1537729469.730886) can0 0B57ED02#00003A0008000000
    (1537729469.731174) can0 0B57ED03#00000000271C0000
    (1537729469.830803) can0 0B57ED01#940200002214F513
    (1537729469.831085) can0 0B57ED02#0000090008400000
    (1537729469.831373) can0 0B57ED03#00000000271C0000
    (1537729469.930765) can0 0B57ED01#940200002214F513
    (1537729469.930992) can0 0B57ED02#00006D0008400000
    (1537729469.931273) can0 0B57ED03#00000000271C0000
    (1537729470.030746) can0 0B57ED01#9402000025140514
    (1537729470.031026) can0 0B57ED02#00003C0008400000
    (1537729470.031313) can0 0B57ED03#00000000271C0000
    (1537729470.130602) can0 0B57ED01#9402000020140A14
    (1537729470.130888) can0 0B57ED02#00000B0008400000
    (1537729470.131177) can0 0B57ED03#00000000271C0000
    (1537729470.230700) can0 0B57ED01#9402000020140A14
    (1537729470.230987) can0 0B57ED02#00006F0008400000
    (1537729470.231274) can0 0B57ED03#00000000271C0000
    (1537729470.330646) can0 0B57ED01#9402FEFF20140814
    (1537729470.330918) can0 0B57ED02#00003C0008400000
    (1537729470.331206) can0 0B57ED03#00000000271C0000
    (1537729470.430732) can0 0B57ED01#9402FEFF29140514
    (1537729470.430951) can0 0B57ED02#0000080008400000
    (1537729470.431237) can0 0B57ED03#00000000271C0000
    (1537729470.431519) can0 0B57ED04#46FA00007D043A00
    (1537729470.431804) can0 0B57ED05#C50F130000000000
    (1537729470.530955) can0 0B57ED01#9402FFFF29140514
    (1537729470.531226) can0 0B57ED02#00006C0008400000
    (1537729470.531513) can0 0B57ED03#00000000271C0000
    (1537729470.630664) can0 0B57ED01#7C8F050029140114
    (1537729470.630946) can0 0B57ED02#00003B000C400000
    (1537729470.631223) can0 0B57ED03#DBBC1000271C0057
    (1537729470.731059) can0 0B57ED01#5E9AFFFF25140814
    (1537729470.731328) can0 0B57ED02#573A0A000C400000
    (1537729470.731602) can0 0B57ED03#DBBC1000271C0057
    (1537729470.831162) can0 0B57ED01#5E9A000025140814
    (1537729470.831423) can0 0B57ED02#F3396E000C400000
    (1537729470.831700) can0 0B57ED03#DBBC1000271C0057
    (1537729470.875233) can0 0B57ED81#0100000000000000
    (1537729470.930971) can0 0B57ED01#5E9A000023140D14
    (1537729470.931208) can0 0B57ED02#8F393D000C400000
    (1537729470.931464) can0 0B57ED03#DBBC1000271C0057
    (1537729471.030719) can0 0B57ED01#2E9AFEFF22140814
    (1537729471.030997) can0 0B57ED02#2B390A000C400000
    (1537729471.031272) can0 0B57ED03#DBBC1000271C0057
    (1537729471.125514) can0 0B57ED81#0200000000000000
    (1537729471.130904) can0 0B57ED01#5E9A000022140814
    (1537729471.131181) can0 0B57ED02#C7386E000C400000
    (1537729471.131465) can0 0B57ED03#DBBC1000271C0057
    (1537729471.230835) can0 0B57ED01#5E9A000029140814
    (1537729471.231115) can0 0B57ED02#63383D000C400000
    (1537729471.231390) can0 0B57ED03#DBBC1000271C0057
    (1537729471.330709) can0 0B57ED01#8D9A000031140714
    (1537729471.330985) can0 0B57ED02#FF370C000C400000
    (1537729471.331260) can0 0B57ED03#DBBC1000271C0057
    (1537729471.375762) can0 0B57ED81#0300000000000000
    (1537729471.430683) can0 0B57ED01#2E9A000031140714
    (1537729471.430959) can0 0B57ED02#9B3770000C400000
    (1537729471.431235) can0 0B57ED03#DBBC1000271C0057
    (1537729471.431514) can0 0B57ED04#550057007D043A00
    (1537729471.431797) can0 0B57ED05#C50F130000000000
    (1537729471.530933) can0 0B57ED01#5E9A00001C140514
    (1537729471.531205) can0 0B57ED02#37373D000C400000
    (1537729471.531479) can0 0B57ED03#DBBC1000271C0057
    (1537729471.625942) can0 0B57ED81#0400000000000000
    (1537729471.631009) can0 0B57ED01#5E9AFDFF23140E14
    (1537729471.631283) can0 0B57ED02#D3360B000C400000
    (1537729471.631559) can0 0B57ED03#DBBC1000271C0057
    (1537729471.730979) can0 0B57ED01#2E9AFFFF23140E14
    (1537729471.731254) can0 0B57ED02#6F366F000C400000
    (1537729471.731528) can0 0B57ED03#DBBC1000271C0057
    (1537729471.830679) can0 0B57ED01#5E9A00001F140514
    (1537729471.830957) can0 0B57ED02#0B363C000C400000
    (1537729471.831233) can0 0B57ED03#DBBC1000271C0057
    (1537729471.875778) can0 0B57ED81#0500000000000000
    (1537729471.930776) can0 0B57ED01#5E9AFFFF28140514
    (1537729471.930997) can0 0B57ED02#A7350B000C400000
    (1537729471.931271) can0 0B57ED03#DBBC1000271C0057
    (1537729472.030752) can0 0B57ED01#2E9AFEFF28140514
    (1537729472.030981) can0 0B57ED02#43356F000C400000
    (1537729472.031256) can0 0B57ED03#DBBC1000271C0057
    (1537729472.126245) can0 0B57ED81#0600000000000000
    (1537729472.130841) can0 0B57ED01#5E9AFFFF1F140A14
    (1537729472.131121) can0 0B57ED02#DF343C000C400000
    (1537729472.131396) can0 0B57ED03#DBBC1000271C0057
    (1537729472.230746) can0 0B57ED01#8D9A00001F14FF13
    (1537729472.231017) can0 0B57ED02#7B340B000C400000
    (1537729472.231291) can0 0B57ED03#DBBC1000271C0057
    (1537729472.330961) can0 0B57ED01#5E9A00001F14FF13
    (1537729472.331228) can0 0B57ED02#17346F000C400000
    (1537729472.331503) can0 0B57ED03#DBBC1000271C0057
    (1537729472.376100) can0 0B57ED81#0700000000000000
    (1537729472.430950) can0 0B57ED01#FF99000023140514
    (1537729472.431227) can0 0B57ED02#B3333D000C400000
    (1537729472.431503) can0 0B57ED03#DBBC1000271C0057
    (1537729472.431781) can0 0B57ED04#550057007D043A00
    (1537729472.432065) can0 0B57ED05#C50F130000000000
    (1537729472.530730) can0 0B57ED01#2E9A000022140214
    (1537729472.531003) can0 0B57ED02#4F330A000C400000
    (1537729472.531279) can0 0B57ED03#DBBC1000271C0057
    (1537729472.626669) can0 0B57ED81#0800000000000000
    (1537729472.630877) can0 0B57ED01#5E9A000022140214
    (1537729472.631155) can0 0B57ED02#EB326E000C400000
    (1537729472.631431) can0 0B57ED03#DBBC1000271C0057
    (1537729472.730794) can0 0B57ED01#5E9A00001C140214
    (1537729472.731070) can0 0B57ED02#87323C000C400000
    (1537729472.731346) can0 0B57ED03#DBBC1000271C0057
    (1537729472.831078) can0 0B57ED01#2E9AFEFF25140214
    (1537729472.831353) can0 0B57ED02#23320B000C400000
    (1537729472.831628) can0 0B57ED03#DBBC1000271C0057
    (1537729472.876309) can0 0B57ED81#0900000000000000
    (1537729472.930926) can0 0B57ED01#5E9AFFFF25140214
    (1537729472.931149) can0 0B57ED02#BF316F000C400000
    (1537729472.931424) can0 0B57ED03#DBBC1000271C0057
    (1537729473.030902) can0 0B57ED01#5E9AFFFF22140514
    (1537729473.031177) can0 0B57ED02#5B313D000C400000
    (1537729473.031452) can0 0B57ED03#DBBC1000271C0057
    (1537729473.126763) can0 0B57ED81#0A00000000000000
    (1537729473.131035) can0 0B57ED01#5E9A000020140B14
    (1537729473.131314) can0 0B57ED02#F7300B000C400000
    (1537729473.131589) can0 0B57ED03#DBBC1000271C0057
    (1537729473.231100) can0 0B57ED01#2E9A010020140B14
    (1537729473.231377) can0 0B57ED02#93306F000C400000
    (1537729473.231653) can0 0B57ED03#DBBC1000271C0057
    (1537729473.330410) can0 0B57ED03#DBBC1000271C0057
    (1537729473.331322) can0 0B57ED01#5E9A010025140814
    (1537729473.331604) can0 0B57ED02#2E303D000C400000
    (1537729473.376631) can0 0B57ED81#0B00000000000000
    (1537729473.430748) can0 0B57ED01#8D9AFEFF29140814
    (1537729473.430971) can0 0B57ED02#CB2F0A000C400000
    (1537729473.431247) can0 0B57ED03#DBBC1000271C0057
    (1537729473.431523) can0 0B57ED04#550057007D043A00
    (1537729473.431807) can0 0B57ED05#C50F130000000000
    (1537729473.530825) can0 0B57ED01#5E9A000029140814
    (1537729473.531097) can0 0B57ED02#672F6E000C400000
    (1537729473.531372) can0 0B57ED03#DBBC1000271C0057
    (1537729473.627306) can0 0B57ED81#0C00000000000000
    (1537729473.631033) can0 0B57ED01#5E9A000020140B14
    (1537729473.631312) can0 0B57ED02#032F3D000C400000
    (1537729473.631587) can0 0B57ED03#DBBC1000271C0057
    (1537729473.730905) can0 0B57ED01#5E9A00002B141114
    (1537729473.731178) can0 0B57ED02#9F2E09000C400000
    (1537729473.731453) can0 0B57ED03#DBBC1000271C0057
    (1537729473.831066) can0 0B57ED01#2E9AFEFF2B141114
    (1537729473.831336) can0 0B57ED02#3B2E6D000C400000
    (1537729473.831611) can0 0B57ED03#DBBC1000271C0057
    (1537729473.876961) can0 0B57ED81#0D00000000000000
    (1537729473.930912) can0 0B57ED01#5E9AFFFF22140414
    (1537729473.931135) can0 0B57ED02#D72D3C000C400000
    (1537729473.931408) can0 0B57ED03#DBBC1000271C0057
    (1537729474.030730) can0 0B57ED01#2E9AFEFF25140E14
    (1537729474.030985) can0 0B57ED02#732D0B000C400000
    (1537729474.031260) can0 0B57ED03#DBBC1000271C0057
    (1537729474.127343) can0 0B57ED81#0E00000000000000
    (1537729474.131004) can0 0B57ED01#5E9A000025140E14
    (1537729474.131287) can0 0B57ED02#0F2D6F000C400000
    (1537729474.131564) can0 0B57ED03#DBBC1000271C0057
    (1537729474.230951) can0 0B57ED01#5E9A000023140A14
    (1537729474.231232) can0 0B57ED02#AB2C3E000C400000
    (1537729474.231506) can0 0B57ED03#DBBC1000271C0057
    (1537729474.330759) can0 0B57ED01#5E9AFFFF1C140514
    (1537729474.331023) can0 0B57ED02#472C0B000C400000
    (1537729474.331298) can0 0B57ED03#DBBC1000271C0057
    (1537729474.377301) can0 0B57ED81#0F00000000000000
    (1537729474.430912) can0 0B57ED01#5E9A00001C140514
    (1537729474.431188) can0 0B57ED02#E32B6F000C400000
    (1537729474.431465) can0 0B57ED03#DBBC1000271C0057
    (1537729474.431743) can0 0B57ED04#550057007D043A00
    (1537729474.432027) can0 0B57ED05#C50F130000000000
    (1537729474.530962) can0 0B57ED01#5E9A000020140714
    (1537729474.531233) can0 0B57ED02#7F2B3E000C400000
    (1537729474.531509) can0 0B57ED03#DBBC1000271C0057
    (1537729474.627891) can0 0B57ED81#1000000000000000
    (1537729474.630900) can0 0B57ED01#FF9900001D140514
    (1537729474.631181) can0 0B57ED02#1B2B0C000C400000
    (1537729474.631456) can0 0B57ED03#DBBC1000271C0057
    (1537729474.730901) can0 0B57ED01#2E9AFFFF1D140514
    (1537729474.731175) can0 0B57ED02#B72A70000C400000
    (1537729474.731451) can0 0B57ED03#DBBC1000271C0057
    (1537729474.830946) can0 0B57ED01#5E9AFFFF23140B14
    (1537729474.831218) can0 0B57ED02#532A3E000C400000
    (1537729474.831494) can0 0B57ED03#DBBC1000271C0057
    (1537729474.877549) can0 0B57ED81#1100000000000000
    (1537729474.930802) can0 0B57ED01#5E9AFFFF26140414
    (1537729474.931001) can0 0B57ED02#EF290C000C400000
    (1537729474.931277) can0 0B57ED03#DBBC1000271C0057
    (1537729475.030932) can0 0B57ED01#2E9A000026140414
    (1537729475.031170) can0 0B57ED02#8B2970000C400000
    (1537729475.031428) can0 0B57ED03#DBBC1000271C0057
    (1537729475.128002) can0 0B57ED81#1200000000000000
    (1537729475.130736) can0 0B57ED01#2E9AFEFF1D140214
    (1537729475.131019) can0 0B57ED02#27293E000C400000
    (1537729475.131295) can0 0B57ED03#DBBC1000271C0057
    (1537729475.230833) can0 0B57ED01#5E9A00002F140114
    (1537729475.231110) can0 0B57ED02#C3280C000C400000
    (1537729475.231395) can0 0B57ED03#DBBC1000271C0057
    (1537729475.331097) can0 0B57ED01#2E9AFEFF2F140114
    (1537729475.331376) can0 0B57ED02#5F2870000C400000
    (1537729475.331652) can0 0B57ED03#DBBC1000271C0057
    (1537729475.377889) can0 0B57ED81#1300000000000000
    (1537729475.431001) can0 0B57ED01#2E9A00001C140A14
    (1537729475.431282) can0 0B57ED02#FB273F000C400000
    (1537729475.431557) can0 0B57ED03#DBBC1000271C0057
    (1537729475.431836) can0 0B57ED04#550057007D043A00
    (1537729475.432120) can0 0B57ED05#C50F130000000000
    (1537729475.530921) can0 0B57ED01#5E9AFFFF2F140514
    (1537729475.531195) can0 0B57ED02#97270C000C400000
    (1537729475.531472) can0 0B57ED03#DBBC1000271C0057
    (1537729475.628498) can0 0B57ED81#1400000000000000
    (1537729475.631193) can0 0B57ED01#2E9A00002F140514
    (1537729475.631441) can0 0B57ED02#332770000C400000
    (1537729475.631719) can0 0B57ED03#DBBC1000271C0057
    (1537729475.731176) can0 0B57ED01#5E9A00001C140B14
    (1537729475.731379) can0 0B57ED02#CF263F000C400000
    (1537729475.731654) can0 0B57ED03#DBBC1000271C0057
    (1537729475.830950) can0 0B57ED01#5E9A000023140114
    (1537729475.831224) can0 0B57ED02#6B260E000C400000
    (1537729475.831487) can0 0B57ED03#DBBC1000271C0057
    (1537729475.878250) can0 0B57ED81#1500000000000000
    (1537729475.930847) can0 0B57ED01#2E9AFEFF23140114
    (1537729475.931063) can0 0B57ED02#072672000C400000
    (1537729475.931345) can0 0B57ED03#DBBC1000271C0057
    (1537729476.030828) can0 0B57ED01#5E9A010025140714
    (1537729476.031098) can0 0B57ED02#A32541000C400000
    (1537729476.031373) can0 0B57ED03#DBBC1000271C0057
    (1537729476.128633) can0 0B57ED81#1600000000000000
    (1537729476.131013) can0 0B57ED01#2E9A00001C140A14
    (1537729476.131295) can0 0B57ED02#3F250F000C400000
    (1537729476.131570) can0 0B57ED03#DBBC1000271C0057
    (1537729476.231147) can0 0B57ED01#5E9A00001C140A14
    (1537729476.231418) can0 0B57ED02#DB2473000C400000
    (1537729476.231694) can0 0B57ED03#DBBC1000271C0057
    (1537729476.331144) can0 0B57ED01#5E9A000029140B14
    (1537729476.331420) can0 0B57ED02#772440000C400000
    (1537729476.331696) can0 0B57ED03#DBBC1000271C0057
    (1537729476.378603) can0 0B57ED81#1700000000000000
    (1537729476.430931) can0 0B57ED01#5E9A000025141114
    (1537729476.431169) can0 0B57ED02#13240F000C400000
    (1537729476.431445) can0 0B57ED03#DBBC1000271C0057
    (1537729476.431721) can0 0B57ED04#550057007D043A00
    (1537729476.432007) can0 0B57ED05#C50F130000000000
    (1537729476.531095) can0 0B57ED01#FF99000025141114
    (1537729476.531371) can0 0B57ED02#AF2373000C400000
    (1537729476.531646) can0 0B57ED03#DBBC1000271C0057
    (1537729476.629209) can0 0B57ED81#1800000000000000
    (1537729476.630868) can0 0B57ED01#5E9A010022140D14
    (1537729476.631146) can0 0B57ED02#4B2340000C400000
    (1537729476.631423) can0 0B57ED03#DBBC1000271C0057
    (1537729476.730903) can0 0B57ED01#2E9AFFFF23140414
    (1537729476.731119) can0 0B57ED02#E7220E000C400000
    (1537729476.731392) can0 0B57ED03#DBBC1000271C0057
    (1537729476.830943) can0 0B57ED01#5E9AFFFF23140414
    (1537729476.831210) can0 0B57ED02#832272000C400000
    (1537729476.831483) can0 0B57ED03#DBBC1000271C0057
    (1537729476.878875) can0 0B57ED81#1900000000000000
    (1537729476.931169) can0 0B57ED01#5E9A000023140D14
    (1537729476.931373) can0 0B57ED02#1F2240000C400000
    (1537729476.931657) can0 0B57ED03#DBBC1000271C0057
    (1537729477.031091) can0 0B57ED01#2E9A000023140414
    (1537729477.031355) can0 0B57ED02#BB210F000C400000
    (1537729477.031630) can0 0B57ED03#DBBC1000271C0057
```

---
## \#14 Posted by: Acido Posted at: 2018-09-24T17:25:23.181Z Reads: 94

```
does it have to be a boosted one?

idk if your board has other electronics connected to the bms but usually you can just switch out the bms for another one

also i got the same multimeter as you :D
```

---
## \#15 Posted by: mikegeezy Posted at: 2018-09-24T18:34:02.418Z Reads: 91

```
Yeah I would love to be able to swap the battery pack out for anything other than boosted.  The problem is that the BMS communicates with the ESC's over that CANBUS link.  So if the BMS isn't powered on and sending a "MOM I'M FINE" signal - the ESC's won't budge.

yeah Fluke makes nice stuff huh?  I really want their network cable tester, but kinda breaking the bank at like $400.
```

---
## \#16 Posted by: Acido Posted at: 2018-09-24T18:36:48.157Z Reads: 88

```
nice but pricey!
```

---
## \#17 Posted by: Vin Posted at: 2019-03-05T00:00:06.322Z Reads: 75

```
Hi,

I was wondering did any of you guys manage to get to the bottom of this and figure out how this BMS works and is it possible to replace the battery pack with an identical one?

I recently bought a BB-V1 and the battery pack still works for now but does not hold charge for as long as it should. I have managed to find a company that is capable of building and replacing the existing pack with an identical one but not sure if I should I proceed with it as I don't want to run the risk of bricking it.

Also the CANDUMP log file is it worth giving it to someone on Fiverr to figure it out?

Any advice or help would be greatly appreciated.

Thanks
```

---
## \#18 Posted by: mikegeezy Posted at: 2019-03-05T13:13:35.625Z Reads: 72

```
I haven't made much progress yet.  I think that I physically damaged my BMS PCB when I disassembled the battery housing, because if I leave all of the cells hooked up eventually it will drain one or two cells down all the way killing them.  So I don't hold a lot of hope that I can sniff healthy CAN signals from that BMS anymore.

I noticed that the V2 boards which have the removable battery have two wires for battery voltage and it looks like two wires for CAN signals.  I'd like to reach out to Boosted tech support and see if the CAN protocol is the same from V1 to V2, in which case maybe those batteries could be made to work with the right connector.

I wouldn't mind chipping in to crowd fund someone who has some expertise with CAN bus hacking.  But expect they are going to need some actual hardware and not just log files.

Another alternative would be to ask Boosted to release at least a portion of the protocol but I'm doubtful they would agree to that.

I think Boosted will replace the battery for you if that's the route you want to go.  What did the third-party you found quote?
```

---
## \#19 Posted by: Drm5602 Posted at: 2019-03-06T05:25:06.087Z Reads: 70

```
So I have changed the batteries before with a damaged BMS. The BMS from Tunda was unfortunately damaged and I haven't been able to get a fully functioning BMS off of a V1. The BMS from Tunda is damaged for the 11th balancing connection, the controller works and you can get the board to move but without that balancing wire it wont read the battery level so it'll continue beeping as if the battery is very low. I have tried it with the 38120 8 amp headway batteries as well as the V2 boosted board battery. So the V2 A123 battery pack has the same dimensions and balance lead locations as the V1 battery pack. If you can take the case apart without damaging the BMS on the V1 you can de-solder and re-solder the both BMS and move the V1 BMS onto the V2 A123 pack. The main leads are different from the V1 to the V2 but the V2 battery leads are smaller and can be soldered on to the V1 BMS. 

I'll double check tonight but I believe the V2 battery pack actually has 3 smaller wires in their connector, I think the can-bus is different version. 

I was looking in to the different can-bus protocols available on the available BMS through tech but I just haven't had time to do more since the BMS doesn't work properly(nothing to base off of). And this is interesting but Bestech BMS actually uses the same programming wire but I haven't gotten that yet either since I'm low on cash at the moment due to going back to school for a career change. We need to find someone who is well versed in can-bus. If not I assume that we're pioneering into something very complicated and could be a waste of money, which I have done quite a bit just to find out that headway 38120 and v2 cells work with the v1 bms. However considering I now have 12 headway lifepo4 and v2 battery cells that need BMS I'll probably contact bestech about 2 different can-bus BMS setups and connecting wire as test subjects and just to be able to use the cells when I have money again.
```

---
## \#20 Posted by: Sebious Posted at: 2019-03-06T07:00:56.665Z Reads: 63

```
I already tried to put the v2 battery into the V1 ESC with no sucess because there is three wires instead of two.
```

---
## \#21 Posted by: Drm5602 Posted at: 2019-03-18T02:23:38.873Z Reads: 57

```
Assuming your V1 BMS is still good. You can use the cells in the V2 battery pack, but yea the V2 BMS does not work with the V1 ESC. V2 is a completely different CAN system. They chips uses different parts too. I couldn't transfer any of the SMD chips from the V2 BMS to repair the V1 BMS either.
```

---
## \#22 Posted by: Vin Posted at: 2019-04-02T17:18:45.243Z Reads: 51

```
Ah that sucks but I would be down for the idea of crowd funding someone who has the expertise to hack it. 

Yeah I agree I really doubt Boosted will release any kind of information with regards to system being used but who knows you could give it a try and test your luck.

I tried emailing them about a replacement motor recently as the bearings were going in my motors on the board but they said to me that they no longer hold parts anymore and I should either throw the whole board away or just kick push it haha. 

**Also if anyone does have a spare motor they have lying around please do let me know as I would interested to purchase it.**

The battery company quoted £275 to build and replace the pack but if I'm honest not sure if they have dealt with a system like this before.
```

---
## \#23 Posted by: huntercasillas Posted at: 2019-04-02T17:42:54.995Z Reads: 49

```
I’ve got the full set of motors attached to the mounts and ESC. Here are some pictures: https://m.imgur.com/a/VJdaStZ?utm_source=share&utm_medium=ios_app

I also have the enclosures which are in perfect condition, a BMS and battery that isn’t working and a V2 BMS that is working.
```

---
## \#24 Posted by: Vin Posted at: 2019-04-02T18:40:28.168Z Reads: 47

```
Hey, thanks for reaching out. How much would you want for the V1 motors and the enclosures?
```

---
## \#25 Posted by: huntercasillas Posted at: 2019-04-02T18:53:23.647Z Reads: 49

```
You just want me to snip the wires off at the base of the ESC and send the motors and mounts? Or are you asking for the enclosures (Battery and ESC)? Because I’m not sure if I’ll be able to remove the motors from the mounts unless I find a 1/2 Allen wrench somewhere or buy one. I’d also have to figure out how to get the pulley teeth/gear off the motors in order to remove them from the mounts, but I can try :slight_smile: and I’m not sure about price, make me an offer?
```

---
## \#26 Posted by: pjotr47 Posted at: 2019-04-11T21:58:28.134Z Reads: 44

```
Is here anybody with a working v1 BMS? I really want to check out the can bus signals. I have bought a month ago a broken boosted v1. I am thinking of swapping all the electronics with a new battery pack and BMS + vesc’s. But I like the remote and esc
```

---
## \#27 Posted by: huntercasillas Posted at: 2019-04-12T02:12:55.668Z Reads: 43

```
I’ve got a V1 BMS with the red blinking light because one of the cells was bad. I’ve also go V1 enclosures in great condition and a working V2 BMS.
```

---
## \#28 Posted by: J11ese Posted at: 2019-04-21T10:24:09.610Z Reads: 40

```
Hi
   I’m in desperate need of a v1 bms if anyone has one for sale, dead or alive.
```

---
## \#29 Posted by: Mikolaj Posted at: 2019-04-21T13:05:30.859Z Reads: 42

```
Hi I have a dead extended range battery
```

---
## \#30 Posted by: huntercasillas Posted at: 2019-04-21T13:53:21.108Z Reads: 42

```
I have a v1 BMS with red flashing lights.
```

---
## \#31 Posted by: huntercasillas Posted at: 2019-04-21T13:53:39.558Z Reads: 40

```
V1 doesn’t have an extended range option.
```

---
## \#32 Posted by: J11ese Posted at: 2019-04-21T18:29:42.063Z Reads: 37

```
Great can I buy it from you?
```

---
## \#33 Posted by: huntercasillas Posted at: 2019-04-21T18:30:22.329Z Reads: 39

```
Yes. DM me with your location! :)
```

---
## \#34 Posted by: J11ese Posted at: 2019-04-21T19:44:46.768Z Reads: 38

```
I don’t know if I can, it may be restricted as I’m a new member
```

---
## \#35 Posted by: grinder Posted at: 2019-08-24T18:30:19.874Z Reads: 31

```
Hi. I am an newbie, and I am in the boat of bricked V1 boosted board users.  I have a dead boosted V1 (yes, the flashing red LED problem) and given that the company will not provide any repair support I decided to open it up and see if I can replace the batteries with new ones myself.  I have some electronics experience.  I was really careful, but it was not easy to disassemble.  At this point I have it apart, I think without damaging the PCB.   Several of the cells read zero volts.  Does anyone have a good "how to" on rebuilding if I purchase a new set of  A123 Systems ANR26650 cells?
I am wondering if anyone has done this successfully and can comment.
Thanks.
```

---
## \#36 Posted by: Drm5602 Posted at: 2019-08-24T18:49:30.180Z Reads: 30

```
I still don't have a functioning v1 bms lol but I've opened the v2 standard range battery and the cells in it are structured similarly. Same soldering points for the balancing leads.
```

---
## \#37 Posted by: grinder Posted at: 2019-08-24T20:28:23.232Z Reads: 29

```
Seems there must be several thousand V1 users who will eventually start googling around when they find out their ~$2K investment is worthless for want of $120 worth of batteries. There must be someone out there who has the skills and can make money by rebuilding batteries for a price.  I would pay cost of batteries + good hourly rate to anyone who could offer this service.
Looking now more closely at the battery management PCB, I see that one of the diodes D7 is damaged, so I suspect my PCB is really hosed.
If I were to try to disassemble a second time, I would:
1). use a dremmel tool to cut thru and remove the plastic housing over the battery management PCB. 
2). with the plastic removed, I would cut the wires to the PCB, and remove it to protect it from accidental electrical overload or mechanical damage.
3). with the PCB removed and protected, I would get medieval on the battery pack and remove it.
4). purchase 12 x new batteries and assemble in the standard way.
5). solder the assembled battery to the PCB. Probably solder the main terminals last.
6). test on the bench and with the charger
7). reassemble the battery package on the board with silicon sealant over the plastic part removed

If anyone has a V1 BMS PCB I would be interested to purchase it so I can try the steps above.
Thanks.
```

---
## \#38 Posted by: grinder Posted at: 2019-08-24T20:35:23.598Z Reads: 30

```
If others have tried and think my approach is flawed, I would be interested to hear your comment.  I see people have tried to debug the CAN bus messages .. etc.  I would think if you have a working board and you replace the batteries carefully and correctly, the system should work as before, but with greatly increased range etc.   If I can purchase a working V1 battery management PCB, I will try this and document my success or failure for this forum.
```

---
## \#39 Posted by: grinder Posted at: 2019-08-26T19:07:43.644Z Reads: 30

```
you still got that V1 BMS?
If yes, what price?
```

---
## \#40 Posted by: Tunda Posted at: 2019-08-30T14:55:48.231Z Reads: 31

```
sold already
```

---
## \#41 Posted by: Dog Posted at: 2019-09-01T04:50:56.273Z Reads: 30

```
Still have it?
```

---
## \#42 Posted by: Mikolaj Posted at: 2019-09-01T07:28:18.446Z Reads: 30

```
Yes still have it
```

---
## \#43 Posted by: GrahamZhu Posted at: 2019-09-17T04:04:22.615Z Reads: 24

```
Anyone still have a working V1 BMS?
```

---
## \#44 Posted by: Lincon Posted at: 2019-10-02T14:47:20.844Z Reads: 22

```
Hello everyone,,
I was wondering did any of you guys manage to get to the bottom of this and figure out how this BMS works and is it possible to replace the battery pack with an identical one?
[reverse image search](https://reverseimagesearch.onl) [email checker](https://emailchecker.vip/) 
I recently bought a BB-V1 and the battery pack still works for now but does not hold charge for as long as it should. I have managed to find a company that is capable of building and replacing the existing pack with an identical one but not sure if I should I proceed with it as I don’t want to run the risk of bricking it.

Also the CANDUMP log file is it worth giving it to someone on Fiverr to figure it out?

Any advice or help would be greatly appreciated.

Thanks
```

---
## \#45 Posted by: Vin Posted at: 2019-10-08T11:46:08.842Z Reads: 19

```
I didn't have much luck in finding out anything with regards to the CANBUS sniffing however I have proceeded open the battery pack and saw there was a damaged resistor on the BMS (RT4). Not sure if it was damaged when opening it or burnt out inside. My BMS and battery pack has now been left with a friend who is an electrician that deals with micro electronics and will try to replace the broken resistor and attempt to reconnect the BMS to the battery pack. If it works I will ask him what he done and how he went about fixing it in detail and will post the findings provided its fixed and functioning safely.

I don't hold much hope for this as anyone who has said they have managed to repair the battery has been vague in the process this is based on posts on Reddit about battery packs being replaced by end users. But fingers crossed hope it works so it can help anyone else on here!
```

---
## \#46 Posted by: kevingraehl Posted at: 2019-11-12T04:08:53.378Z Reads: 14

```
Any updates?    If someone could make a spoofer that allowed v2 batteries that would be amazing
```

---
## \#47 Posted by: Vin Posted at: 2020-01-24T02:51:50.335Z Reads: 10

```
Not yet I’ve left it with him over Christmas period and not sure he had time to look over it as soon as I get some info I’ll be sure to post something.

Yeah if the V2 battery could work that would be great and would stop a lot of people wasting perfectly good parts
```

---
