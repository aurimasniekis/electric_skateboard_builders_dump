# Dual tacon Bigfoot 160, 10s5p,

### Replies: 18 Views: 843

## \#1 Posted by: Cnouizi Posted at: 2018-01-31T08:52:54.273Z Reads: 157

```
Before I hook stuff up and fry everything. I wanted to seek some advice from you guys since I am not eskate  savvy at all.

My build 
2 VESC from diyelectricskateboard (torqueboards)
2 tacon Bigfoot 160
10s5p battery pack from diyeboard 
Mounts and pulleys (14/16t and 36t kit)

Does everything look good? Do I need to change anything? Is everything compatible?

I ll take any advice I get! Thank you in advance.

Also, I am getting my extended battery range for boosted soon and I want to use the standard one for an eskate build. How do I go about that?
```

---
## \#2 Posted by: myreala Posted at: 2018-01-31T09:18:41.344Z Reads: 145

```
Diyelectricskateboard VESC are know to fail very often even in BLDC. I think even Maytech and hobbyking VESC has a lower failure rate than those.
```

---
## \#3 Posted by: Ishayc Posted at: 2018-01-31T09:28:30.832Z Reads: 137

```
Don't forget to limit the erpm to 60k in the vesc.
You motor is on the higher KV side(245kv).

What wheels do you have? 
16/36 pulleys with 245kv motor and 10s may cause voltage spikes.
Had the same issue with 97mm wheels. after I changed the pulleys to 15/44 problem solved.
```

---
## \#5 Posted by: Ishayc Posted at: 2018-01-31T09:32:23.885Z Reads: 119

```
The vescs are just fine. 
Run it in BLDC mode and you will be ok.
```

---
## \#6 Posted by: Cnouizi Posted at: 2018-01-31T09:33:11.253Z Reads: 111

```
Once these fail what would be a good VESC to buy? Enertion focbox?
```

---
## \#7 Posted by: Cnouizi Posted at: 2018-01-31T09:33:47.156Z Reads: 115

```
I have 90mm wheels that come from the torqueboards website
```

---
## \#8 Posted by: Ishayc Posted at: 2018-01-31T09:35:23.997Z Reads: 112

```
Then you might be ok. 
Just do your first runs extra careful, especially when braking.
```

---
## \#9 Posted by: Cnouizi Posted at: 2018-01-31T09:36:07.396Z Reads: 108

```
Awesome thank you very much.
```

---
## \#10 Posted by: myreala Posted at: 2018-01-31T09:49:59.191Z Reads: 108

```
When these fail, focbox is the most reliable one so far. You can also get the 6.4 version from stewii, that one is very promising.
```

---
## \#11 Posted by: aigenic Posted at: 2018-01-31T10:27:17.403Z Reads: 105

```
Diy you just say, that MayTech VESC is more reliable than DIY VESC?! :O Thats kinda bullshit...IDK about Hobbyking...if you can afford to go for FOCBOX, go for it :) VESC6 is even better, but pricey and you would have to W8 a long time...
```

---
## \#12 Posted by: pixelsilva Posted at: 2018-01-31T10:56:02.680Z Reads: 104

```
Although the Bigfoot 160 comes from the RC plane world is suitable for esk8 and is a little monster (Is the one I first considered for my build) but is a 245kv... a little high on kvs; normally one needs to shot for motors between 140kv to 190kv.
```

---
## \#13 Posted by: Cnouizi Posted at: 2018-01-31T20:51:54.300Z Reads: 75

```
thank you guys for the help. I ll definitely keep all this in mind. I ll go based on this for the next changes.

anybody have any ideas about boosted batteries and if it can be used in a diy?
```

---
## \#14 Posted by: aigenic Posted at: 2018-01-31T21:25:40.859Z Reads: 72

```
Do you mean Boosted board's batteries? They are made out of A123 26650 cells, LiFePO4, 2500mah, 60A discharge, they can be used, but they are bigger and heavier than Liion or Lipo cells...but theyy last forever :) They are also much more expensive and have lower voltage......there are some build with them already, but not much :)
```

---
## \#15 Posted by: Cnouizi Posted at: 2018-01-31T22:04:11.057Z Reads: 60

```
Thanks you. my question is can I just plug them with the VESC and it ll work?
```

---
## \#16 Posted by: aigenic Posted at: 2018-01-31T22:56:53.803Z Reads: 57

```
You have to configurate the VESC, change the BMS (boosteds BMS communicates with their ESC) and yea, it should work :) I am not VESC expert but as far as I know there shouldnt be any problem :)
```

---
## \#17 Posted by: ZackoryCramer Posted at: 2018-01-31T23:32:17.112Z Reads: 58

```
I don't know about you, but I've had a diyelectricskateboard VESC blown up on me, (it was on fourth of July too, great timing) I am not sure where I did wrong but I was resetting PPM and when I added current to the motor through BLDC tool, the whole board just went :fireworks: Not sure if it's a software issue or what but I've been extremely cautious of using BLDC tool afterwards.
```

---
## \#18 Posted by: aigenic Posted at: 2018-02-01T00:16:54.987Z Reads: 60

```
Ehh...Sorry to hear that...I personally blew MayTech and Vanda VESC...IMO all 4.12 VESC are not reliable...but the difference between DIY and MayTEch is, that DIY makes them according to Benjemins original plans, but Maytech decided not to use some of its components, which  is the reason why Maytech fail more often...

I dont say they cant last, but if you buy MayTech VESC be prepared that you will have to replace it sooner or later :)
```

---
## \#19 Posted by: ZackoryCramer Posted at: 2018-02-01T00:30:04.010Z Reads: 58

```
After all, Ben is just an esk8 enthusiasts who took his time to design such a great ESC for free. Kudos :+1: to him for creating this open source project.
```

---
