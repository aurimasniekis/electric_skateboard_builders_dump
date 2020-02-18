# Latching Relay Based Main Switch ( in lieu of electronic anti-spark switch)

### Replies: 28 Views: 1619

## \#1 Posted by: SkaterBoy58 Posted at: 2018-05-01T00:02:27.615Z Reads: 218

```
Due to unreliability of anti-spark switches and having gone through two failing closed in past 12 months – I have built and tried a latching relay based alternative to use in a new build I am commencing.  

I want the main power switch to be 100% reliable 100% of the time.

 The new build will be a 10S system using dual vescs.

Basic design concept is to use
•	a heavy duty latching relay as main +ve power switching from battery +ve to vescs +ve  ( no BMS)
•	two momentary action push-buttons – one for “close” and one for “open” with leds in push buttons to indicate latching relay status
•	no electronics (to fail from the transient voltage spikes!) 
•	use main +42V supply rail to power relay switching circuits
Started off looking around for a heavy duty latching relay. Settled on one from china [link to latching relay](https://www.aliexpress.com/item/Latching-Relay-80A-meter-relays/778321893.html?spm=a2g0s.9042311.0.0.zQvSNs) . This unit is quite cheap (Approx. US$6). Ordered two and shipping was approx. 2 weeks.
 ![picture 1|381x412](upload://iafiQZ2vbVbTgf95123O6RyJlUk.jpg)

This beast ticked most boxes. The contacts are rated at 80A at 240Vac with no dc rating indicated. The contacts are quite beefy and they should be OK for the application for battery through current whilst closed (My board draws about 40A maximum battery current).

The relay dc breaking current will be practically zero (vescs idle current only)- the dc making current will be the vesc capacitor charging inrush current which causes the problems on electronic anti-spark switches. 

As a test -I mocked the latching relay up through the XT90 main power socket on my existing board and completed 10 closes and opening onto dual vescs – took the cover off to look at the contacts and there was no visible signs at all of arcing on power contacts during both closing and opening. 

This is probably due to the very positive mechanical action of contacts when making and the very low current when breaking.
For the pushbuttons – using this one for “close” (it has a led built in)

![picture 2|485x459](upload://w7ibjN5wUEwFMTjAeo3PnLjvodc.jpg)  
And this one for “open”
![picture 3|532x500](upload://q70dGEZKBtyt2T9hZSFJY8FLSmh.jpg)
 
Any momentary illuminated pushbutton with spdt contacts will do the job.

The latching relay has a single 12V coil and you need to reverse current direction in the coil to reverse the latched main power contact operation.  

This means a bit of control circuitry to achieve this. I used two mini 24V relays (each with 2x SPDT contacts) hot-glued to back of latching relay. [link to mini relay](http://www.altronics.com.au/p/s4132b-2a-24vdc-dpdt-pcb-mount-telecom-relay/)   
![picture 4|352x500](upload://sdT6j6f37KCRbp64zNxvJw6wnIJ.jpg)
Reaching back approx. 20 years to my past EE days – designed up a hard-wired relay circuit with a bit of electrical interlocking between the two push-buttons to avoid shorting +42V control supply if both pushbuttons are operated.

![circuit |690x487](upload://1yXg1CiWfjapTf5I9qv2MxOLhkP.jpg)

Used a 2A wire fuse from input +v for control supply.

 After testing – hot glued wires and connections to avoid any future issues from vibration.  Bench tested OK and put aside for new build.

Total cost around $20  - around same size as anti-spark switch and hopefully a lot more reliable.
![latch relay 00 |666x500](upload://g1FVxjaM7E0oC9ZNAGPubiji7bU.JPG)![latch relay 2 |500x666](upload://clM1XaNHrREMiRZdtZtokLJUmqz.JPG)![latch relay 3 |666x500](upload://sxv4JC9HzU3ZIOhd5IoqS48BWH8.JPG)![latch relay 0 |666x500](upload://e8zYMpSuZUtyPAiTvxWcFsz8CPv.JPG)![latch relay 1 |666x500](upload://z4et3y5DgufYAoqFdcos7lpPBTb.JPG)![latch relay 4 |666x500](upload://VGRks8sknrhnIoLGtECLNA78JM.JPG)
```

---
## \#2 Posted by: Kug3lis Posted at: 2018-05-01T00:13:52.098Z Reads: 185

```
There is difference in between AC current and DC current... I doubt it even will hold 10A on DC level...
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-05-01T00:15:45.268Z Reads: 187

```
Thats how 50A DC relay looks like...

https://image.made-in-china.com/43f34j00HOLTNdJIyioe/Albright-Duplicate-DC66p-Winch-Solenoid-Continuous-50A-Overload-200A-Motor-Reversing-Relay-48V-24V-12V-DC-Contactor-for-Winch-Hoist.jpg
```

---
## \#4 Posted by: SkaterBoy58 Posted at: 2018-05-01T00:24:45.754Z Reads: 178

```
For making and breaking 50A DC yes it needs to be like that -

but that is not the application here!

BTW no difference in thermal heating across power contact for AC or DC current
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-05-01T00:25:38.122Z Reads: 172

```
Are u for real boy? :joy:
```

---
## \#6 Posted by: b264 Posted at: 2018-05-01T00:33:49.036Z Reads: 171

```
[quote="SkaterBoy58, post:4, topic:53972"]
no difference in thermal heating across power contact for AC or DC current
[/quote]

This isn't true, but

My biggest concern is that heavy vibration will cause a mechanical system like this to fail.  And that's if you can stomach the weight and size and complexity issues.
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2018-05-01T00:33:56.667Z Reads: 167

```
Hmmm... do you guys smell that???


I smell.....




Bullshit
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-05-01T00:37:56.540Z Reads: 170

```
Yeah I love the idea then riding board, you loose brakes and etc for several seconds cause you hit a bump on the road :D or VESC restarts and hits full throttle because some remotes fucks up on start up if you have some throttle :D
```

---
## \#9 Posted by: darkkevind Posted at: 2018-05-01T00:40:29.846Z Reads: 172

```
Holy smokes! That seems convoluted!

This is all you need for a high current on/off switch...

![20180501_013839|500x500](upload://5cYs24N1ZZOb7vnwlyS3sNe9317.jpg)
```

---
## \#10 Posted by: deucesdown Posted at: 2018-05-01T01:28:37.218Z Reads: 154

```
Why the mean tone? Has this been tried/failed in the past already?

[quote="darkkevind, post:9, topic:53972"]
This is all you need for a high current on/off switch
[/quote]

How many miles and what kind of juice have you had through that thing?
```

---
## \#11 Posted by: TowerCrisis Posted at: 2018-05-01T01:56:37.984Z Reads: 148

```
IMO this is a bad idea. I've played with mechanical relays before and it's no fun. You will pull crazy amps instantly on powerup, in order to charge the VESC capacitors. Even worse if you have additional caps. It will make a pretty large spark and wear those contacts out very fast, especially on a dual motor setup with twice the capacitors. (talking less than 100 switches)

You should look into latching solid state relays.
```

---
## \#12 Posted by: darkkevind Posted at: 2018-05-01T02:16:56.916Z Reads: 144

```
[quote="deucesdown, post:10, topic:53972"]
How many miles and what kind of juice have you had through that thing?
[/quote]

I've put hundreds of miles on my board with this switch... The battery is 8s4p LG HG2 so 80A constant.

There is an online voltage regulator bringing the voltage down to operate the coil with a rocker switch, one way ON other way OFF.
```

---
## \#13 Posted by: PatRocks Posted at: 2018-05-01T02:26:19.746Z Reads: 137

```
Off topic: is that a benchwheel receiver?? I LOVE mine!!
```

---
## \#14 Posted by: deucesdown Posted at: 2018-05-01T03:34:07.167Z Reads: 133

```
All I know about relays is from AvE... DC arcing is a concern when switching under load, right? And it's breaking contact that's more of a concern, not making? At least for function, not for wear/corrosion.

The things that skeeved me out is that it's a AC relay not rated for DC function, and it's a chinese relay that probably will perform way below spec. @SkaterBoy58 why not look for parts on digikey/mouser, with specs that have some meaning behind them?
```

---
## \#15 Posted by: Kug3lis Posted at: 2018-05-01T11:53:27.028Z Reads: 123

```
VESC inrush current can exceed over 500A to charge caps :) so you can expect freaking big sparks inside that relay switch...
```

---
## \#16 Posted by: darkkevind Posted at: 2018-05-01T12:36:57.336Z Reads: 121

```
Yes. 😉

It's great!
```

---
## \#17 Posted by: SkaterBoy58 Posted at: 2018-05-03T00:04:15.212Z Reads: 122

```
Guys - The gross negativity and fearmongering from a forum seller of large expensive (almost same cost as a vesc) anti-spark switches when a much cheaper  possibility is put forward is commercially understandable – but the personal attacks and vitriol in some of the above posts are not helpful to any-one.

This project is aimed at my new build which is pretty average – a 10S 8P battery, dual focboxes and dual 5065 1200W motors with 35A FLC. 

So let’s have a closer look at the duty of a main switch between the battery and the dual focboxes.

There are three main duties through the latching relay contacts:

**1.	Continuous current whilst closed** (thermal consideration only) On a normal ride I average about 10A battery current with a maximum of 40A battery current for high torque demand situations. Despite someone disagreeing with me above, 1A DC current gives same I^2R power loss as 1A (RMS) of AC current.  So - averaged over a ride we are operating at an average of 10A for an 80A rated contact so the contact should be OK for this duty.

**2.	Breaking Current** – this duty is to disconnect 42V supply power from vescs from an idle state. A pair of  focboxes draw about 75mA idle current.  This is a very easy breaking duty for the relay contact. 

**3.	Making Current – the big one!**  This duty is to charge up vesc capacitors from 0V to 42V. This current is very high but for only a very short time.  To demonstrate this – see below a theoretical graph showing current and voltage for  close to what I have – I used 100m ohm as total system resistance. This includes battery internal resistance, wiring, relay contact resistance and capacitor bank internal resistance.  The theoretical charging calculation is for scenario of 42V supply, 100 m ohm resistance charging a total of 3,000 uF capacitor bank. This combination has an RC time constant of 3 u seconds.  (3/1,000,000 of a second)
2 x focboxes have about 2,800uF total capacitance on the  input DC supply.

![charging graph|690x392](upload://yyLJU4ZkKELE2pDSPq2OA1RG63R.jpg)

As can be seen from the theoretical graph, the current drops from maximum to almost 0 in just 3 ms (3/1000 of a second) and the large current (>15A) is over in just 1ms.   If you do the calculation – the total cumulative energy for this making current duty is approx. 2.6 Joule or equivalent to 2.6 Watt second - so not huge. 

I repeated this making duty test again 20 times using my 42V battery pack and dual focboxes  – and there was no visible arc on making or evidence of relay contact burning. The latching relay has quite a large beefy contact and a very positive mechanical closing action.

In regarding vibration and the relay falling to bits – this will be tested in time as well. My enclosure has rubber strip seals to deck which does provide quite a bit of vibration dampening. Will mount the relay on side of enclosure on a foam pad as well. 

Interesting that @darkkevind  has been operating a similar latching relay with no issues – albeit with a different coil control circuit.

In regard to the negative comment above re relay weight and size – you can see it is about 35mm x 35mm and total weight is approx. 50g.   

I will put this in my new build and will pull it out after 6 months service to see status of relay contacts and report back to this post. If it fails before hand - will also update this post.!

Cheers
```

---
## \#18 Posted by: deucesdown Posted at: 2018-05-03T01:05:06.814Z Reads: 112

```
Great post, thank you!
```

---
## \#19 Posted by: SkaterBoy58 Posted at: 2018-06-13T23:30:31.880Z Reads: 106

```
Just to report back in :
Latching Relay main switch in lieu of anti-spark switch has been in testing and service for a month now - no issues to date !
:smiley:
![push%20buttons|666x500](upload://nqa6jjMrqrBrTmiLsssofP0oYxr.jpg)
![pushbuttons|666x500](upload://kS7qbbvqKvMgqKcSPHZmZ5GCJY3.jpg)
```

---
## \#20 Posted by: Hummie Posted at: 2018-06-13T23:43:47.174Z Reads: 103

```
awesome looking but then i see what looks like an xt90 plug and there's no way i'd get beyond just doing a loopkey there!  like no other ive seen.
```

---
## \#21 Posted by: SkaterBoy58 Posted at: 2018-06-13T23:47:00.589Z Reads: 102

```
nah - that's an XT-60  with a main 40A fuse and I also use it to totally isolate battery pack when required.  
There is a black cover to go over this to make it look nice!
```

---
## \#22 Posted by: SkaterBoy58 Posted at: 2018-08-27T04:33:36.838Z Reads: 83

```
Just an update - latching relay main switch has been in service now for about 4 months with about 350 operations without any issues. Been on some pretty rough tracks in that time. Operation has been flawless from the beginning.

I think the current success of this trial is due to:

* Having a mechanically latched system with momentary push-buttons for control - both open and close

* Having a beefy large contact area contact for the making duty.

Cheers
```

---
## \#23 Posted by: deucesdown Posted at: 2018-08-27T14:14:49.034Z Reads: 76

```
I recently reviewed this thread and @darkkevind's thread. I'm gonna give this a crack. But I'm looking at the 10s-13s range for voltage, and lotta amps. I know this particular build was just for 40a max, so I'll see what I can find for relays.

Thanks again for posting this stuff.
```

---
## \#24 Posted by: SkaterBoy58 Posted at: 2018-08-27T23:20:44.416Z Reads: 71

```
@deucesdown - thanks for your post. AliExpress do a 100A latching relay which should do for most eboard applications . (I think @darkkevind  runs with this relay) 
My latching relay was 80A rated for AC ( but on most rides I peak at 40/50A battery current with an average around 15A)  
Are you running  dual vescs?     
Cheers  

 https://www.aliexpress.com/item/12V-Magnetic-Latching-Relay-100A-with-Copper-Braided/924140636.html?spm=2114.search0104.3.44.1d767833iK59iA&ws_ab_test=searchweb0_0,searchweb201602_1_5724111_10065_10068_10130_10547_5724211_10548_5890011_5724311_10696_5724011_10084_10083_10618_5970011_10307_10131_10132_10133_5910011_10059_100031_10103_5725011_5990011_5724911_5980011,searchweb201603_55,ppcSwitch_5&algo_expid=4df173ad-b182-40a3-96e1-abedc2c349b0-6&algo_pvid=4df173ad-b182-40a3-96e1-abedc2c349b0&priceBeautifyAB=0
```

---
## \#25 Posted by: sismeiro Posted at: 2018-10-18T12:54:50.305Z Reads: 63

```
Hi, I really like your start setup but I think you are missing something like this:
![jpg_640x640|500x500](upload://H9rolKaG3QFzXXoHevb1guzT2V.jpeg) 

:slight_smile:
```

---
## \#26 Posted by: SkaterBoy58 Posted at: 2018-10-18T13:13:52.402Z Reads: 60

```
your right -good idea -will use in next build  

BTW latching relay is still performing faultlessly

Two fellow local DIYers had anti-spark switches fail closed in last week( after about 6 months in service)
```

---
## \#27 Posted by: sismeiro Posted at: 2018-10-21T14:51:40.912Z Reads: 51

```
Hi, going to a little extreme, I found another fine switch to use in a electric longboard. A car battery switch that can be pulled off. I really like this one:

![1d8d5e82-ff3d-4309-9dbb-2c77626b8b9d|500x500](upload://lMtnjj7UjMcALJWlHESeSYRI8A8.jpeg) 

It can be bought here: https://www.ebay.com/itm/CAR-BATTERY-POWER-SWITCH-MAX-50V-DC-50A-CONT-75A-INT/183030387127?hash=item2a9d7611b7:g:ykMAAOSw8-FaZSHm:rk:6:pf:0
```

---
## \#28 Posted by: SkaterBoy58 Posted at: 2018-10-21T23:09:34.323Z Reads: 44

```
@sismeiro  The ASS fanboy Naysayers will say this will not work - but if it has hefty contact area and a positive closing action ( turning to on position) I think it should be fine .
```

---
