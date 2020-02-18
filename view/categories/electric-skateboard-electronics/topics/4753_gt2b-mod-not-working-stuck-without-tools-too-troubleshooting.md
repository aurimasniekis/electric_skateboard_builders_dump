# GT2B mod not working (stuck without tools too) - troubleshooting

### Replies: 13 Views: 1114

## \#1 Posted by: cmatson Posted at: 2016-06-15T23:08:08.694Z Reads: 150

```
So I got down to Australia, went to use my board, and my remote won't turn on- completely DOA. 

I plugged it into the wall, and the **green light immediately came on saying it was fully charged** (and I charged it before I left). I left it on the charger though for a couple hours just to make sure. 

So from there _I thought it may be the switch_, so I cut it out and simply put the two wires together.. no luck. **no lights, just nothing.** And it isn't just the leds because it won't control the board and the receiver light is flashing signaling a lost connection. 

Today, I just fiddled with it again- this time, I turned it on (by again, shorting the wires) and a **red light** came on. This normally means it is dead or out of charge, which is weird considering the day before. I would have charged it, but had to leave for my internship this morning and didn't want to leave it plugged in all day. 

SO have any of you experienced something similar, or have any suggestions? 
-it's not the switch
-green light while charging
-red light when turned on

I wish I had a multimeter to see if the battery was dead, in which case I could just switch it out assuming the charging function isn't working...

thanks guys, it really sucks at the moment to have taken shit outa my bag before the trip just to bring my board and stay under the checked bag weight limit, and now that I'm here it doesn't work :pensive::worried:
```

---
## \#2 Posted by: Chris_KP Posted at: 2016-06-15T23:34:39.254Z Reads: 137

```
l if your down south of syd any time soon ill hook you up lol
```

---
## \#3 Posted by: cmatson Posted at: 2016-06-15T23:41:10.086Z Reads: 130

```
good to know- 

right now I'm in Baulkham hills, and I'll be staying in Freshwater for all of next week, and finally Mosman the last week before heading to Adelaide. 

All of those are North Sydney though..  anyways, thanks for the help- I may just have to uber to a hobby shop and use some giant ass rc remote. 

I'm also going to see if Jason might be able to hook me up, and since I'll be seeing him in Adelaide in 2.5 weeks, I'd be able to give him back a remote then. With all of his testing on different remotes, I'm sure there might be just one I could rent from him while I'm here.
```

---
## \#4 Posted by: cmatson Posted at: 2016-06-16T05:04:03.607Z Reads: 105

```
would there be an easy way to charge the battery without going through the normal charging circuit? 

I can easily get to it, but I'm just thinking this has to do with the battery being dead, and for some reason it won't charge.
```

---
## \#5 Posted by: barajabali Posted at: 2016-06-16T06:04:19.049Z Reads: 103

```
Yes. I charge one of my super old gt2b mods without a usb or anything! 

I just striped the end off of a usb cable and used a multimeter to identify positive and negative then just used a signal wire terminal instead of the usb terminal for charging and I just charged it with a regular phone block 5v. 
So I basically run 5v straight to the battery to charge it
Works like a charm as has been for over a year lol
```

---
## \#6 Posted by: cmatson Posted at: 2016-06-16T06:08:54.231Z Reads: 101

```
sounds good- I'll probably have to pull some macgyver shit to get it done while I'm here in Australia.

lol literally all I brought was a screw driver to install my Space Cell in the enclosure.
```

---
## \#7 Posted by: barajabali Posted at: 2016-06-16T06:18:57.912Z Reads: 95

```
Oh man I never travel with my boards without everything I would ever need to fix them. I learned my lessons before
```

---
## \#8 Posted by: cmatson Posted at: 2016-06-16T07:07:52.046Z Reads: 91

```
My issue was being on the borderline weight limit for my checked bag.. I'm here for 5 weeks doing an internship (so I need dress attire and casual clothes) with one checked bag. So all I could take was the board and the remote.

As it is I had to move my shoes and shirts to my carry on because the checked bagh was over weight to start.
```

---
## \#9 Posted by: Chris_KP Posted at: 2016-06-16T07:11:53.684Z Reads: 88

```
If you in sydney and you need a remote go check out this shop called Hobby Co in syd
```

---
## \#10 Posted by: seanpain4 Posted at: 2016-06-16T11:18:56.475Z Reads: 84

```
Why.... that could have caused a lot of issues. You're lucky it didn't puff up or blow.
```

---
## \#11 Posted by: FLATLINEcustoms Posted at: 2016-06-16T13:36:13.758Z Reads: 81

```
Could it possibly need to be re-binded to the receiver?
```

---
## \#12 Posted by: barajabali Posted at: 2016-06-16T15:10:07.387Z Reads: 82

```
Not really just monitor the voltage...  I know batteries. it wasn't gonna cause any problems.  The charger got the cell up to 4.2 volts and charged at 1 amp.  

It's just like charging it off a power supply

Also the battery has an over charge and under charge circuit built into it right on top. You just need to solder onto those connections and you're golden it will cut off if it charges too high.
```

---
## \#13 Posted by: cmatson Posted at: 2016-06-20T06:56:30.990Z Reads: 67

```
ok, so I went by an electronics store because the guy I'm staying with had to buy a PC part, and they happened to have some mini multimeters for $5. 

got one, tested the 18650 battery, and it was 1.2v... fuk. I think my GT2B hasn't been correctly charging it or discharging it, so it didn't realize the voltage was dropping until it literally couldn't turn on. After all, I charged it full before I left, and it was for sure green and had plenty of time on the charger. 

next step: I ripped open one of those lipstick sized battery backups (so damn hard to do with that all metal casing... my god) for iphones and took out the 18650- it was at a happy 3.7v

I just briefly hooked it up, and was able to get the remote working- even so, I have no way of soldering it, so the only testing was done by holding the stripped wire tips onto the ends of the battery. 

So bare minimum I'll be able to fix it at the Enertion HQ when I have access to a soldering iron. 

But, all this won't really matter since there is an enertion remote on its way to me as we speak to get me by until I can fix this little POS.
```

---
