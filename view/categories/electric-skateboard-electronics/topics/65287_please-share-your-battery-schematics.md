# Please share your Battery schematics

### Replies: 13 Views: 522

## \#1 Posted by: ElskerShadow Posted at: 2018-08-18T18:23:57.576Z Reads: 146

```
Hey guys

I recently started building batteries, I am confused about how to link P between them. I can't figure out how to make a good schematic I can follow so I don't mess up. Right now I have done many mistakes and have welded/unwelded many cells. Destroyed some as well. I really wan't to learn ! 
Seeing schematics of any kind for any battery in any configurations would be greatly appreciated so I can understand better the logic behind a battery build. 
Thanks a lot !
```

---
## \#2 Posted by: Sebike Posted at: 2018-08-18T18:25:54.345Z Reads: 146

```
are you doing it with one flat layer or two? how many in series?
```

---
## \#3 Posted by: Acido Posted at: 2018-08-18T18:45:14.549Z Reads: 136

```
![2017-09-10_094459|690x303](upload://cHbJ1PqGF63nVv480bZrxjrLRMu.jpg)
```

---
## \#4 Posted by: ElskerShadow Posted at: 2018-08-18T19:33:39.785Z Reads: 125

```
I plan to do many different thing, 
Right know I am struggling with a 13s7p 
I will share pictures but don't judge the shitty work I'm just trying to learn with shitty cells I have salvaged from an electric scooter so it's a bit nasty 
I will not use the said pack because I did too much wrong thing I want to build it see if it works and then build the same from scratch
![IMG-20180818-WA0008|690x388](upload://1hzGS3KqXR2S3mgpJAa4jUPPf4V.jpg)
![IMG-20180818-WA0007|690x388](upload://nT5NwyNp7QwpszL8aIZjK2ySzzR.jpg)
```

---
## \#5 Posted by: L3chef Posted at: 2018-08-18T19:39:26.407Z Reads: 119

```
Here's 2 great thread regarding spotwelding, battery design amd how to avoid misstakes.
https://endless-sphere.com/forums/viewtopic.php?f=14&t=84412&hilit=Copper+bus+bar&sid=3985ad7ea8b0242d9c4918ca2b3191cb

https://endless-sphere.com/forums/viewtopic.php?f=14&t=68005
```

---
## \#6 Posted by: Skifree Posted at: 2018-08-18T20:07:00.549Z Reads: 113

```

![image|690x348](upload://xM0VAFFKDTCpHfq1jW991VbUKri.jpg)

it looks like you started to do it correctly, you have joined all the individual cells together fine with just the single nickel strip. But then you just connected them all together into one big cell...

But (If you were doing it in several cell series) the connection between the series is not enough, assume that each cell can deliver 15 amps, that means that all the cells together can deliver 105 amps (15 amps x 7 cells). So the strip at the first arrow will have to be able to handle 105 amps of current.
the connection between your second and third series is only 2 nickel strips, that means that together the two strips will need to handle 105 amps.
The connection between your third and fourth series looks to be only a single strip as well, once again it will need to carry 105 amps.

you have your individual cell series welded together fine, but what is really important is the connection between the series. I see a lot of packs on here being built with an 8 awg wire between packs, that will be able to support the 105 amps. 

@L3chef listed some awesome threads to read up on. get to know your batteries as much as possible, you don't need a fire to take away all your hard work!

Check out @Eboosted https://www.electric-skateboard.builders/t/eboosted-enclosures-thread/38073/772?u=skifree for just one example of a build.
```

---
## \#7 Posted by: oyta Posted at: 2018-08-18T20:50:09.459Z Reads: 97

```
https://www.electric-skateboard.builders/t/8s-4p-battery-help/25062/2?u=oyta
```

---
## \#8 Posted by: ElskerShadow Posted at: 2018-08-18T21:32:03.411Z Reads: 90

```
Thanks guys I am digging all the info you gave me ! 
I'm starting to figure out how to do everything properly
```

---
## \#9 Posted by: Eboosted Posted at: 2018-08-18T21:44:04.529Z Reads: 84

```
@ElskerShadow

Please use fish paper between P-Groups, this extremely important to avoid fires, remember there is a pretty high tension between P-Groups, just imagine in a 13S battery pack, P-Group 1 against P-Group 13, just divided by a thin layer of heat shrink :scream::scream::scream:

Even though, this battery is for an e-bike, a lot less vibrations than an esk8, there's always the risk of a crash that could lead to tear the heat shrink and subsecuent short.
```

---
## \#10 Posted by: ElskerShadow Posted at: 2018-08-18T21:47:27.257Z Reads: 82

```
[quote="Eboosted, post:9, topic:65287"]
Please use fish paper
[/quote]
Yeah someone told me that as well but when typing fish paper I could only find the little rings for the positive side. Do you have a ebay/AliExpress link maybe ? I will buy some asap
Edit: it's even better than for an ebike but for a converted motorcycle so I must do my best to make the safest battery ! 
10s are easy but this 13S makes my brain boil haha
```

---
## \#11 Posted by: L3chef Posted at: 2018-08-18T21:52:14.731Z Reads: 81

```
Here's where I get mine at.
https://www.ebay.com/itm/8x-Fish-Adhesive-Paper-Electrical-battery-Pack-Insulating-24-24-0-03cm-Insulator/321559730848?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649
```

---
## \#12 Posted by: Eboosted Posted at: 2018-08-18T23:19:13.195Z Reads: 75

```
This is the one I use, it's a US base company so it might be trickier to get them in EU

https://www.ebay.com/itm/122286559751
```

---
## \#13 Posted by: mynamesmatt Posted at: 2018-08-19T02:38:00.184Z Reads: 64

```
![Screenshot_20180819-123714_Gallery|690x353](upload://At2DLt7CGxFnSY5J4w8fyd1rOt9.jpg)
```

---
