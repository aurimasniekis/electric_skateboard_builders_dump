# Battery + Charging/Storage Questions

### Replies: 3 Views: 408

## \#1 Posted by: kidcisco Posted at: 2017-06-26T19:39:27.476Z Reads: 77

```
So I just purchased all of the parts for my first build and I received my 2x 3s (Turnigy 5000mah) batteries and iMax B6 charger first. The sticker on the two batteries said they were shipped at 30% and after reading lots of scary stories about LiPo's online I want to make sure I take care of the batteries as best as I can but I'm really confused right now. 

I think I need to charge these batteries up to a specific storage level. What level is that (3.8v??) and how exactly would I do that using this charger? I don't anticipate all of my parts coming in for a week or two so the batteries will most likely be sitting for a bit until I get everything ready. Do I even need to worry about charging them to storage levels or just keep them in the box at 30%? 

The plugs on the battery do not match up to the plugs on my charger. The balance lead does but the thick black/red wires have male and female banana plugs and none of the adapters I got with the charger will work with this. I planned on originally wiring these in series and soldering together so I'm not sure of a short term solution besides snipping the connectors and just using the included alligator clips. 

My power adapter (found one at a thrift store since the iMax didn't come with one) is 3A so I don't think I can charge these at 1C (is that correct)...will this be a problem?

Sorry, just worried because of all the nightmares I have heard involving lipos and I don't want to burn the spot down, lol. Any assistance is greatly appreciated.
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-26T20:26:12.825Z Reads: 61

```
Good to be cautious and a bit paranoid with these things a puncture or charging or discharging too quickly can be problematic.  That said you should be good with 1C charge rate, that's typically a safe rate for RC lipos (I generally use 3.6A on a 5Ah battery, only issue with going higher is the charger overheats and does a thermal shutdown/restart).  Regarding the ends of the plugs you can get a banana plug to female XT60 or XT90 or whatever the battery has (maybe deans, if you post a link can check them out).

You could just hook the alligator clips into the plug but if they touch while it's connected you're gonna have some toasted alligator clips and maybe worse on your hands so be careful if you go that route and make sure everything is in a place it won't accidentally get moved (not that this has happened to me... ending in a very bright and scary flash as a wire turned to a fuse in front of me).

If you start to clip the plugs off make sure you are super cautious about what you're doing, don't cut across both cables at once, cut one, wrap it in electric tape so it can't touch anything then cut the other, make sure when you reattach them to something you also do this one at a time, if the leads touch you've suddenly become a novice arc welder in the worst way possible.  Think through and diagram what you're going to do before you start cutting anything.  Alternative to cutting things off you can just buy some female plugs and make a cable that puts the batteries in series without needing to chop anything off, you can probably find premade cables with XT-90 plugs for putting batteries in series or parallel as well.  This way for charging you just take the extra cable off and charge each battery.

---

Also when you connect the battery to the balance charger you should be connecting both the big cable and the balance lead cable if that wasn't obvious at first.  I believe it will charge the cells through the balance cables and uses the main cable across all the cells to pull the charge back down to get things more balanced if one cell is substantially higher than the others.

Regarding the storage level stuff I wouldn't worry about it too much for the couple of days the storage level I believe is around 3.7-3.8V.  The cells charged at 30% won't drain quickly without any load on them the storage option is good if you plan to shelf the thing for a couple of weeks or more, basically you don't want to leave it fully charged for a long time or it wears on the battery.
```

---
## \#3 Posted by: kidcisco Posted at: 2017-06-28T18:20:55.250Z Reads: 30

```
Thanks for the tips. All good and important info that helped out a lot. I checked the voltage of both packs and they are 3.7-3.8 each cell so I will probably leave them till I start assembling and I will charge them all together with the balance charger. I didn't even think about cutting both the + and - wires separately, good thing! LOL
```

---
