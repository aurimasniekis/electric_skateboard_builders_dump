# BMS - LiPo and Li-ion

### Replies: 19 Views: 440

## \#1 Posted by: MrDGOrman Posted at: 2018-08-10T23:38:36.762Z Reads: 111

```
Hi everyone,

I'm looking for some advice along with some wiring diagrams.

I've currently got 3 (looking to get 4) Zippy Flightmax 5000mah (3s1p) batteries connected together in parallel. I disconnect each battery to charge them using a balance charger. I'm getting board of this and want a cleaner finish to my board.

I'm wondering if there's a way for me to use a BMS to allow me to plug one lead in and then they all charge up? Like all the other boards out there that have the 18650 Li-ion system or similar. I'm guessing it's possible because the only difference is cell type. My only concern is the fact that LiPos are more dodgy compared to Li-ions.

If this is possible does anyone have a clear wiring diagram I could follow? Can anyone recommend a BMS that'll work? Is there a BMS that will support a 12s4p setup which I plan to have as my final build? I'd quite like to get something that will work with both so I can switch over relatively easily.

If you've got this setup already then I'd love to know!

Cheers,
Daniel
```

---
## \#2 Posted by: b264 Posted at: 2018-08-10T23:48:44.151Z Reads: 104

```
This is similar, but for 10S instead.  It's totally possible and better to use a BMS for lipo

![00%20PM|690x433](upload://eq73nMpXepnCk8uqKsjOSTLlXxZ.png)

It also depends what BMS you use because some are wired differently than others
```

---
## \#3 Posted by: MrDGOrman Posted at: 2018-08-10T23:55:48.536Z Reads: 96

```
I just read a post about a fire that someone had and you mentioned that's why you should have a BMS. He plugged an XT-90 antispark key into his charging port. Lucky for me I've got HXT charging leads to make it an impossibility for that to happen.

Back to BMS - any particular one you would recommend? Looking to add a 4th battery so something that's compatible with that would be great.

Also, if I got one suitable for more batteries would I still be able to use it with less? For example, if I got one suitable for 4 batteries would it still work with 3?

Thanks,
Daniel
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-08-11T00:25:54.996Z Reads: 81

```
Wait you said you have your three batteries in parallel right now? So you're overall using a 3S3P pack at a total 15000mah?

If that's the case then you wouldn't need a BMS if you are already just using a balance charger.

If the packs ARE in parallel then all you have to do is keep them in parallel, and put all the balance leads in parallel. Your current balance charger will be able to charge all three of the packs at once assuming that you have all the balance leads go into one central plug, and the main power all be in parallel.
```

---
## \#5 Posted by: b264 Posted at: 2018-08-11T03:26:10.527Z Reads: 72

```
I think for sure they meant in series and not parallel

Yes, if you shorted the charge port through the BMS you should have one level of safety which would prevent (hopefully) a fire

[quote="MrDGOrman, post:3, topic:64500"]
BMS - any particular one you would recommend?
[/quote]

D190 by bestech
```

---
## \#6 Posted by: MrDGOrman Posted at: 2018-08-11T07:47:44.819Z Reads: 66

```
@TowerCrisis Sorry for the confusion. I meant series. They're all plugged into eachother to make one large (positive of battery 1 into negative of battery 2, positive of battery 2 into negative of battery 3).

@b264 perfect. I'll deck out the D190. Thank you so much for the help!
```

---
## \#7 Posted by: MrDGOrman Posted at: 2018-08-13T09:47:40.324Z Reads: 53

```
@b264 You recommended that I check out the D190. That appears to be for a 6 cell setup? Correct me if I'm wrong but I will have 4 batteries which all contain 3 cells each. Wouldn't that mean I need a 12 cell unit instead?

Thanks,
Daniel
```

---
## \#8 Posted by: b264 Posted at: 2018-08-13T09:50:12.137Z Reads: 50

```
Apparently the D190 is [not available for 12S](http://www.bestechpower.com/pcmbmspcbforli-ionli-polymerbatterypacks/).  I only use 10S and recommend 10S if you're using VESC 4 hardware.

There should be one in there for 12S with similar specs.  @thisguyhere might have some tips for 12S.
```

---
## \#9 Posted by: MrDGOrman Posted at: 2018-08-13T10:02:52.890Z Reads: 50

```
I have the FOCBOX if that makes a difference? Fairly sure that's VESC 4.0 though.

Any particular reason why you would recommend 10s over 12s when using VESC 4.0?
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-08-13T15:35:53.335Z Reads: 48

```
focbox is rated at 60v max, and even though a 12s pack is well below that, it's just better to keep operating voltage / amperage well below the limits.

generally speaking 10s is more reliable and safer, but just as many people run their setups at 12s.  with higher voltages you have to keep your erpm limits in mind as well, in that it has to be well below 60k or you chance blowing something up (namely the drv chip).

one thing for sure that sucks at 12s is blowing through all variations of anti spark switches, i have not been able to get a single one to work out for me for more than a month.

i'm going to order some more 12s charge only d140 modules tonight so i'll list them here in about 10 days or so:

http://www.esk8life.com/bestech-d140-12s
```

---
## \#11 Posted by: MrDGOrman Posted at: 2018-08-14T11:49:11.386Z Reads: 43

```
Hi,

So what's your opinion on my setup then? Don't get another battery to prevent part failure and get a BMS suitable for 9 cells?

I was told that you can't have a BMS for LiPo batteries and then transfer it to Li-ion batteries. Is that true? If so then I'll just wait until I get my main battery pack (10s4p?)

Cheers,
Daniel
```

---
## \#12 Posted by: Andy87 Posted at: 2018-08-14T12:47:43.613Z Reads: 40

```
You can use the lipo bms als for LiIon.
Just it will cut off your battery at 3.5v probably.
So with LiIon you would have less range, as you could discharge them till 2.8-3v usually (that’s where a LiIon bms cut off your battery)
```

---
## \#13 Posted by: MrDGOrman Posted at: 2018-08-14T12:50:18.859Z Reads: 38

```
My friend and I thought that would be the case. Is there such a thing as a "smart BMS" that allows you to set the cut off voltage?

I know real world application would be pointless but I'm just interested.
```

---
## \#14 Posted by: Andy87 Posted at: 2018-08-14T13:02:31.576Z Reads: 37

```
Yes there are. Search here in the forum or on AliExpress. There are some which you can set up and control even via Bluetooth
```

---
## \#15 Posted by: MrDGOrman Posted at: 2018-08-14T13:11:35.419Z Reads: 34

```
Nice! I'll get looking into it then!

AliExpress seems to be a go to place for these random sort of parts!
```

---
## \#16 Posted by: Andy87 Posted at: 2018-08-14T13:26:51.158Z Reads: 36

```
Not for all of them...keep away from buying batteries there.

What else you could make if you plan later to run LiIon and just now have a lipo.
Get a LiIon bms and set your vesc battery cut off to 3.5V. That should save your lipos from overdischarging. You could also add an lipo alarm to your lipos (4$or so on hobbyking) they will let you know when your batteries reached low voltage
```

---
## \#17 Posted by: MrDGOrman Posted at: 2018-08-14T13:38:20.738Z Reads: 38

```
Andy, you're a genius! I don't know why I didn't think of that before.

I'll get a Li-ion BMS from Bestech which is suitable for 10s4p and then adjust the cut off in my FOCBOX. Fairly sure I've already got the cut off set to 3.5v per cell anyway.

Can't remember the website right now but I was going to get the batteries from a website called Nikon or something? Do you have any suggestions where I can get 30Q cells from that are UK (or EU) based?

Thanks,
Daniel
```

---
## \#18 Posted by: Andy87 Posted at: 2018-08-14T13:51:08.999Z Reads: 35

```
Nkon.nl is a trusted good source.
```

---
## \#19 Posted by: MrDGOrman Posted at: 2018-08-14T14:35:49.932Z Reads: 33

```
That's the one! I'll check them out when I come to making my order.

Cheers,
Daniel
```

---
