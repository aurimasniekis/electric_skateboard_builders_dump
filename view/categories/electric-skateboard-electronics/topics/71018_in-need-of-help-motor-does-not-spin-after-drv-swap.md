# In need of help - motor does not spin - after drv swap

### Replies: 14 Views: 167

## \#1 Posted by: OrthodoxName Posted at: 2018-10-12T20:35:19.138Z Reads: 47

```
I have ran into an issue with my vesc and after going through 2 of them, i replaced my drv on my tourqueboard 4.12 vesc  and it seems to be working except for when I go to power the motor using vesc tool. The readout shows an accurate readout of the duty cycle but the current output does not change much (max at .5A or so). I have tried a new motor as well an no luck. The vesc does not work with motor detection either. Duty cycle does read out when spinning the motor by hand however.

* I have been using this board for ~5 months now and have recently ran into drv issues and such, commonly happening when hitting a small bub in the road* 

Here is a real time data readout when messing with arrow key driving back and forth. 

![image|690x394](upload://c9dmM0ZlM84mpxwQbUn1UhGzvWL.png) 

Any ideas and/or help is greatly appreciated. If you have any other questions i am open to answering as well. Sadly I havent found anyone with the same issues or with solutions that work when searching.
```

---
## \#2 Posted by: Bart_Dood Posted at: 2018-10-13T15:46:27.269Z Reads: 31

```
Double check your ground pad is well soldered, if not the vesc will behave oddly. A quick test can be pressing down on the drv chip as you run through your tests, if it all works ok then you've confirmed a bad ground
```

---
## \#3 Posted by: Bart_Dood Posted at: 2018-10-13T15:48:36.501Z Reads: 31

```
Oh and check all your solder joints under a microscope and scrub the PCB with some acetone and an old toothbrush, it will get rid of any tiny solder particles that could be causing weirdness
```

---
## \#4 Posted by: OrthodoxName Posted at: 2018-10-13T18:20:36.655Z Reads: 27

```
holding it down sadly did not help. Here is a picture of the chip if you happen to see anything that might be causing issues..., I don't have access to my soldering supplies at the moment but can check later. 
![image|375x500](upload://2PVo3nnWuOc8u89sf9UCD2DHQbG.jpeg)

I believe my soldering job is decent enough and made sure that the pads are connected but I'm not sure if another chip may have been blown or there is another issue that I'm not sure about. I set my battery cutoff to 10 and changed a few setting that could be an issue (as mentioned in other articles)
```

---
## \#5 Posted by: Bart_Dood Posted at: 2018-10-13T18:50:21.143Z Reads: 25

```
Hard to see from a photo, you need to check under a magnifying glass or microscope, check all the stuff around the chip, next time make an aluminum foil heat shield around it to prevent everything melting and pre heat the PCB from underneath to around 80c
```

---
## \#6 Posted by: OrthodoxName Posted at: 2018-10-13T19:09:12.525Z Reads: 23

```
I was planning to touch the pads again with an iron and/or maybe reflow with a heat gun and then clean it up? Do you know of any other issues that could be causing current to pass through the vesc?
```

---
## \#7 Posted by: b264 Posted at: 2018-10-13T19:15:02.278Z Reads: 24

```
Did you solder the pad underneath the chip?
```

---
## \#8 Posted by: OrthodoxName Posted at: 2018-10-13T19:23:36.528Z Reads: 23

```
I used a heat gun to solder it, yes. As I mentioned above, I made sure that wasn't the issue as well by applying pressure to the chip to confirm connection, sadly no dice
```

---
## \#9 Posted by: Bart_Dood Posted at: 2018-10-13T20:50:37.323Z Reads: 19

```
Did u use low temp solder? Even with 138c solder one of mine required a second rework to get the ground pad right
```

---
## \#10 Posted by: OrthodoxName Posted at: 2018-10-13T21:17:28.276Z Reads: 19

```
I used standard lead free solder because it was what I had. The heat that I used was enough to remove the chip. I added a little extra solder to it and then when I heated it, i made sure it lowered down to see that the past was heated and I believe that it should be good? I can heat it again when I dgo to the shop however to be safe. 

Could there be any other issues with chips on the board that aren't working? Everything seems to save on to it.
```

---
## \#11 Posted by: Bart_Dood Posted at: 2018-10-13T22:46:58.810Z Reads: 17

```
Getting that pad hot enough with regular solder for a rework will be hard. If u plan on fixing more buy some chipquik low temp solder
```

---
## \#12 Posted by: b264 Posted at: 2018-10-13T22:59:24.877Z Reads: 17

```
[quote="OrthodoxName, post:10, topic:71018"]
standard lead free solder
[/quote]

I recommend to never use lead-free solder.  Wash your hands after soldering.
```

---
## \#13 Posted by: OrthodoxName Posted at: 2018-10-13T23:00:58.074Z Reads: 16

```
I'm a fan of leaded stuff as well but sadly don't have any right now, I need to get some.
```

---
## \#14 Posted by: OrthodoxName Posted at: 2018-10-13T23:03:00.490Z Reads: 15

```
I used a soldering heat gun to heat it up so I think it should be good but hopefully I don't have to fix anymore after this.
```

---
