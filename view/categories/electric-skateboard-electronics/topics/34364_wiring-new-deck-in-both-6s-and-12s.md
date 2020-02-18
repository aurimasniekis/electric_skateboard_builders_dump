# Wiring new deck in BOTH 6S and 12s

### Replies: 25 Views: 1711

## \#1 Posted by: Malakai Posted at: 2017-09-30T10:31:06.555Z Reads: 158

```
This is my third Eskate, I have a 6s and 12s already and I like them both for different reasons. Now I'm trying to get the best of both and adding a few things I didn't have on my other decks but I'm running in to a few bumps in the design. I have diagrams for both a 6 and 12 cell build but I wanted to somehow connect both of them with some sort of switch. (6s/off/12s) going to add some sort of Display for the voltage and a better mechanism for charging. 
The parts list includes two vesc that I'm using have a 300a peak and 60a contenous. 
http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/
Does anyone know of a switch I can use to do this that can handle the 300a?
I'm also trying to permanently mount these lipos because opening my case every time I have to charge it sucks. 
http://www.ebay.com/itm/like/292181460283?ul_ref=https%253A%252F%252Frover.ebay.com%252Frover%252F2%252F0%252F8%253Fbu%253D44809890090%2526segname%253D16TE1798429_T_GENERIC_CT1%2526crd%253D20170810090000%2526mpre%253Dhttps%25253A%25252F%25252Fwww.ebay.com%25252Fulk%25252Fitm%25252Flike%25252F292181460283%2526ch%253Dosgood%2526url%253Dhttps%25253A%25252F%25252Fwww.%252524%25257Bprefix%25257Debay.%252524%25257Bdomain%25257D%25252Fulk%25252Fitm%25252Flike%25252F%252524%25257BITEM1_NUMBER%25257D%2526osub%253Dc9865e14250eaeb90646221224dc16f0%25257E5473d7cc868f380a6efae9eb6ccaa7ee%2526sojTags%253Demid%25253Dbu%25252Csegname%25253Dsegname%25252Ccrd%25253Dcrd%25252Curl%25253Durl%25252Cch%25253Dch%25252Cosub%25253Dosub%2526srcrot%253D0%2526rvr_id%253D0&ul_noapp=true
I have four of these liposuction ready to install but I'm getting a little lost when it comes to wiring all of these to a single charger. To my knowledge all I'll need is one BMS for each stage a 6s and a 12s depending on what side of the switch I'm on but If I'm being honest I have no idea. The last two decks I wired had to be dismantled every time I charged it. I tried uploading the scamatics i drew up for this one but for some reason the site isn't liking pictures from my iPad but the parts list so far include 4x 6s lipo, 2x VESC, and two motors.
I know I need a voltmeter, a good charger, and at least one 12s BMS
Need to find the best BMS and fastest charger for the project also could use a little help drawing a new scamatic incorperating the new parts or a more efficient design 
   I'm aware this is a bit over my head but I'm sure it's easier then I think and totally doable with some solid advice. any help would be GREATLY  appreciated
```

---
## \#2 Posted by: krloz Posted at: 2017-09-30T13:52:15.338Z Reads: 134

```
There are switches you can use designed to switch between battery banks in rv's boats etc but they are huge expensive and huge.  I think you are better off mounting An xt90s female in each battery bank and a single male towards the escs. That way you can plug one or the other
```

---
## \#3 Posted by: richgang Posted at: 2017-10-02T04:53:06.477Z Reads: 115

```
i have a q for you what is better for high speeds a lower or higher kv motor
```

---
## \#4 Posted by: Idle Posted at: 2017-10-02T05:18:22.761Z Reads: 107

```
Really?

Try a simple search and if you don't find what you are looking for you need to work on your google-fu.


It may be easier to use google or whatever instead of the forums search function *ymmv

Try this:

Electricskateboard.builders What kv? I feel the need for speed
```

---
## \#5 Posted by: Idle Posted at: 2017-10-02T05:26:00.273Z Reads: 103

```
@Malakai
 Are you intending on using it @6s so other people can ride it without needing immediate medical attention? 

Just curious, as I'd thought about this very same thing for riding in hilly areas. 

Would be kind of nice to have a Jekyl and Hyde setup. 
Well mannered for casual cruising, and then flip a switch for bsc hill climbing mode
```

---
## \#6 Posted by: scepterr Posted at: 2017-10-02T05:53:15.534Z Reads: 84

```
If talking about straight switching from parallel or series between 2 banks that's possible but the BMS situation I'm not sure about.
```

---
## \#7 Posted by: Malakai Posted at: 2017-10-02T06:00:01.092Z Reads: 87

```
Was thinking I could double the amp hours for the battery when I was in flat areas but toning it down for curious friends would be an added bonus
```

---
## \#8 Posted by: scepterr Posted at: 2017-10-02T06:01:25.862Z Reads: 82

```
Would it really matter? Same watt hours
```

---
## \#9 Posted by: Cobber Posted at: 2017-10-02T06:03:42.226Z Reads: 78

```
I'm confused what the benefit of having a 12s1p & a 6s2p battery is when you could just have a 12s2p? unless slower with less torque is the goal? It certainly won't go further in my experience.
12s with FOC on a FOCBOX is more than I'd try though...
```

---
## \#10 Posted by: Malakai Posted at: 2017-10-02T06:04:47.079Z Reads: 75

```
I already have two boards with pretty similar parts I use my 6s all the time and my 12s sits in my trunk unless I am in an area with lots of hills of have a friend riding with me this build was me trying to combine them so I could potentially get rid of my first set up the 6s. Two hybrid decks would be way better then one of each
```

---
## \#11 Posted by: scepterr Posted at: 2017-10-02T06:20:13.736Z Reads: 71

```
So you want to carry 2 diff battery setups and be able to switch between them?
```

---
## \#12 Posted by: Malakai Posted at: 2017-10-02T06:24:32.363Z Reads: 71

```
I didn't want to mount two sets of  batteries I wanted to be able to switch from parallel to series with a switch. It's the first time permanently mounting a battery so naturally i found myself trying to add way more features then I need to. If it's impossible or will ruin the efficiency of my set up then I can always keep the 6s for other people since it lasts all day, and is probably better for people to learn on anyways.
```

---
## \#13 Posted by: Malakai Posted at: 2017-10-02T06:31:33.888Z Reads: 70

```
It's more to tone it down in flat areas and for beginners
```

---
## \#14 Posted by: scepterr Posted at: 2017-10-02T06:38:50.384Z Reads: 71

```
You can just load a low power profile using the extended firmware and an Android or ios app and just have a 12s battery
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#15 Posted by: Malakai Posted at: 2017-10-09T02:51:25.394Z Reads: 63

```
So I decided to cut the system in half because having all four on one line brought the amperage higher then my parts can handle. After a bit of reading I saw these diagrams
<img src="/uploads/db1493/original/2X/3/3da4c7516f7f5063c7b42614869161bf0d18d8e8.jpg" width="479" height="500"> <img src="/uploads/db1493/original/2X/b/ba1fffe24e70934051549b4dd5fe6f0cf9082498.jpg" width="374" height="500">
Then I drew up a new one with the parts I have hoping the 300a anti spark switch I have will work in place of the loop key 
<img src="/uploads/db1493/original/3X/0/5/05e25b95280d92ba2c2123172c0768da6f967dfe.JPG" width="187" height="500"> 
this will be mirrored if it all works
The battery pack should be 10000mah 12s 300a and all the parts have been rated to at least that. It's the first time I've done a permanent mounted battery so I could use a little help with the wiring.
```

---
## \#16 Posted by: Malakai Posted at: 2017-10-09T02:53:56.699Z Reads: 58

```
Forgot to add a voltameter at the anti spark switch
```

---
## \#17 Posted by: jmasta Posted at: 2017-10-09T04:16:45.574Z Reads: 55

```
Definitely don't hook it up like you have drawn. 

If you're trying to put them in parallel, the polarity of the top battery is reversed. If you're going for series, it's even more wrong (For series, it should be: lower battery NEG to anti-spark NEG / lower battery POS to upper battery NEG / upper battery POS to anti-spark POS)

 And you can't hook them up in parallel while connected to a dual balance charger
```

---
## \#18 Posted by: Malakai Posted at: 2017-10-09T05:17:15.814Z Reads: 54

```
The balance leads will be on the outside of my case and the balance charger would have only been attached when I had the other electronics off. Or so I thought? I saw the page about using a loop key for this and assumed I could use the switch the same way? If I'm wrong, is there a better way to do it?
```

---
## \#19 Posted by: Malakai Posted at: 2017-10-10T06:28:01.172Z Reads: 48

```
Is this any better?
<img src="/uploads/db1493/original/3X/c/1/c1c61659cc4abf67a6c25db9c20037ee7ba24ae6.JPG" width="170" height="500">
```

---
## \#20 Posted by: pat.speed Posted at: 2017-10-10T11:12:27.760Z Reads: 45

```
The first diagram is fine as far as I can see. I take it that little adapter will be used to connect the batteries together and to the Vesc? So it will be 12s1p?
```

---
## \#21 Posted by: gbutcher Posted at: 2017-10-10T12:05:47.368Z Reads: 29

```
Will you have to change vesc settings when you switch from 6S to 12S?
```

---
## \#22 Posted by: Malakai Posted at: 2017-10-10T13:30:01.050Z Reads: 31

```
Yeah but there's going to be another system parallel with this one with both receivers on the same channel
```

---
## \#23 Posted by: Malakai Posted at: 2017-10-10T14:22:09.555Z Reads: 33

```
I ran in too many problems with having 6 and 12s on a switch but if you put the y harness on the outside you could easily switch between the series and parallel harnesses. I'm not sure if I'm going to do that yet. I baught an electric switch because the loop key design looks messy.
```

---
## \#24 Posted by: Malakai Posted at: 2017-10-12T16:38:38.195Z Reads: 32

```
This is the best voltmeter I could find with the required volt and amperage rating.
http://www.ebay.com/itm/DC-0-01-400V-0-1-300A-Wireless-Digital-Ammeter-Voltmeter-Watt-Power-Meter-K6I3-/192033533337
I'd need the larger one to keep up with my battery but it's huge compared to others I've seen. Anyone have any better ideas? this seems like it's a little overkill
```

---
## \#25 Posted by: florr Posted at: 2017-10-15T19:54:44.356Z Reads: 28

```
If you just need a Voltmeter and no Powermeter there is no need for a certain ampere rating since you are going to connect it in parallel.
You'll need something like [that](https://www.banggood.com/3Pcs-Red-LED-0_28-Inch-2_5V-30V-Mini-Digital-Voltmeter-Voltage-Tester-Meter-p-980044.html?rmmds=search) with a higher voltage rating. For example [Link](https://de.aliexpress.com/item/0-28-inch-small-digital-voltmeter-three-wires-DC0-100V-30V-50V-100V-LED-Digital-voltmeter/32806043671.html?spm=a2g0x.search0104.3.16.7kvXua&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10065_10151_10068_10344_10345_10342_10343_10340_10341_10193_10194_10304_10307_10060_10302_10155_10154_10056_10055_10054_5370015_10537_10059_10536_10534_10533_10532_100031_10099_10338_10103_10102_10052_10053_10107_10050_10142_10051_10320_10321_10322_10084_10083_10080_10082_10081_10177_10110_5590015_10111_10112_10113_10114_5610015_10180_10312_10313_10314_10184_10078_10319_10079_10073_10186-10080,searchweb201603_25,ppcSwitch_3&btsid=9fe6addd-d8ab-4254-a7ac-e374a72ae866&algo_expid=a3d027d2-97ad-4fb9-977d-78b45656bfaf-2&algo_pvid=a3d027d2-97ad-4fb9-977d-78b45656bfafa)
```

---
