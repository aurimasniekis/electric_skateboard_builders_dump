# Orange Wheel SUV &#124; SkateShred Bottlenose &#124; TB218 &#124; FS 6374 &#124; Janux Mounts &#124; TB 12S4P &#124; FSESC Dual 6.6 &#124; Airless

### Replies: 18 Views: 585

## \#1 Posted by: humanisticnick Posted at: 2019-02-05T20:45:28.152Z Reads: 203

```
Hey everyone,

I finally bought and got all my parts.I know I went on the cheaper route but I still thought I was buying OK quality parts. However when I posted on FB everyone was saying is that my anti-spark is crap and would catch on fire.
https://flipsky.net/collections/accessories/products/antispark-switch-pro-280a

My first build question is: Is the anti spark crap? If it is can I just wire my VESC directly to TB battery since the battery has it's own switch?

![IMG_1670|375x500](upload://kFiQqYTEXYgTwzW02FLeK91tmjQ.jpeg) 
![deck|690x344](upload://ok8ksFxd6AbIirus40Uu2ru2XCH.jpeg)
```

---
## \#2 Posted by: J_Dizzle Posted at: 2019-02-05T20:59:41.944Z Reads: 195

```
Yes, the battery has an anti spark switch included in it. I would throw that flipsky switch out, as it is known for blowing very fast. Build is looking good so far!
```

---
## \#3 Posted by: humanisticnick Posted at: 2019-02-05T21:05:52.787Z Reads: 189

```
Thanks for the info. Waste of $40, damn. What makes the antispark die the amps or volts or it's just a piece of crap?
```

---
## \#4 Posted by: anorak234 Posted at: 2019-02-05T21:07:42.669Z Reads: 180

```
Poor quality control leads to early parts failure. Flipsky has always been hit or miss but it just seems that their switches are particularly bad.
```

---
## \#5 Posted by: humanisticnick Posted at: 2019-02-05T21:09:13.457Z Reads: 174

```
Well one less thing to solder I suppose :slight_smile:
```

---
## \#6 Posted by: humanisticnick Posted at: 2019-03-02T14:28:17.032Z Reads: 150

```
Hey guys looking for some more help. I'm having a hard time getting my VESC working. Not sure if it's a VESC issue or a battery issue.

https://youtu.be/PPwIFH8631g
```

---
## \#7 Posted by: Deodand Posted at: 2019-03-02T17:39:02.582Z Reads: 141

```
My best guess is a short in the ESC is causing overcurrent protection on the BMS to trip. But it's pretty hard to tell from this one test. Do you have anything else you could run off the battery to test?
```

---
## \#8 Posted by: humanisticnick Posted at: 2019-03-02T22:16:14.742Z Reads: 118

```
https://youtu.be/_MQjtsMU38Q
```

---
## \#9 Posted by: Deodand Posted at: 2019-03-02T23:04:18.269Z Reads: 108

```
One of two possibilities, 

A) the flipsky is shorted and causing BMS protection to trigger

B) The increased capacitance of the bigger ESC is causing too much inrush current during power on (powering up the capacitors) tripping BMS overcurrent.
```

---
## \#10 Posted by: humanisticnick Posted at: 2019-03-18T19:36:35.106Z Reads: 86

```
Alright time for a question about which one you all this is better for this build.

I had some issues with my TB12s4p battery and just sent it back to them to repair/replace. However it left a bit of a bad taste in my mouth so i was looking around at alternatives.

At $450 dollars this is what I originally got:
https:///products/electric-skateboard-battery-epower-pack-12s4p

But for almost the exact same amount of money I could just go Lipo with 2 of these and an AC/DC charger. ($170x2(batteries)+$100(charger)= $440

https://hobbyking.com/en_us/turnigy-high-capacity-16000mah-6s-12c-multi-rotor-lipo-pack-w-xt90.html

For this build 2X6374 and a 6.6Dual, which one is better? Opinions welcome.
```

---
## \#11 Posted by: J_Dizzle Posted at: 2019-03-18T23:13:51.567Z Reads: 70

```
I would just replace the Torqueboards pack, as that is a high quality pack with 30q cells, which are the preferred cells of builders on this forum. If you do decide to go down the lipo route, do not use those lipos as the are 12c which is way too low discharge for what you want. Look for 35c or above if you can
```

---
## \#12 Posted by: rusins Posted at: 2019-03-18T23:16:02.796Z Reads: 68

```
16Ah * 12C = 192A. Seems enough to me :upside_down_face:
```

---
## \#13 Posted by: ninTHIENdo Posted at: 2019-03-18T23:19:45.844Z Reads: 68

```
Beat me to it
```

---
## \#14 Posted by: J_Dizzle Posted at: 2019-03-18T23:20:28.251Z Reads: 65

```
I would like to respectfully disagree, as those packs are intended for field charging other lipo packs
```

---
## \#15 Posted by: ninTHIENdo Posted at: 2019-03-18T23:22:30.156Z Reads: 69

```
How do you calculate discharge rates for lipos then?

What are 18650s intended purpose? Don’t think Samsung made the 30qs specifically for esk8 purposes.
```

---
## \#16 Posted by: humanisticnick Posted at: 2019-05-14T13:38:25.859Z Reads: 46

```
Ended up going with 2 10s5p running in parallel so a total of a **10s10p** . Still need to tinker with VESC settings and make some physical adjustments but it works and it went for it's first ride around the neighborhood.

![image|666x500](upload://aYT0xHSepJfwn7CJ8sv3UYAs0Rq.jpeg) 

![image|666x500](upload://eL9L2uk81bucqP23OjjV3NnVCXQ.jpeg) 

![image|666x500](upload://lqRFrwTfm4zJjAmEsptCYPqTvPu.jpeg)
```

---
## \#17 Posted by: humanisticnick Posted at: 2019-05-14T14:15:31.935Z Reads: 39

```
Just in case anyone else wants to use the enclosure for the DIYEBOARD.com 10s5p battery. I would print it PETG and spray it with something.

https://www.thingiverse.com/thing:3629813
```

---
## \#18 Posted by: humanisticnick Posted at: 2019-05-14T14:21:59.731Z Reads: 38

```
Just in case anyone wants a Printable Flipsky Dual 6.6 enclosure. 

https://www.thingiverse.com/thing:3629830
```

---
