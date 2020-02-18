# Anyone using Bestech HCX-D336 BMS?

### Replies: 6 Views: 555

## \#1 Posted by: Zyb Posted at: 2017-12-26T20:41:23.762Z Reads: 97

```
Im about to start with my build and im trying to choose a BMS. I know theres another popular Bestech model but HCX-D336 is only 8mm tall which is perfect because i want to make my battery enclosure as small as possible. Do you guys think thats an ok choice? Btw im thinking to use it with 10s4p configuration with prob 190kv 6355 motor(s)

http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D336.html
```

---
## \#2 Posted by: thisguyhere Posted at: 2017-12-26T21:05:36.950Z Reads: 92

```
looks good I suppose. 

70a discharge rating will be lower than what your pack, assuming you're using 20a continuous cells, can output at 4p. 

if you use this bms make sure you set your battmax setting appropriately (70a total) to avoid cutouts. 

assuming you're planning to use the bms for both charge and discharge?
```

---
## \#3 Posted by: Zyb Posted at: 2017-12-26T21:12:24.214Z Reads: 85

```
im totally new in this hobby, im not sure about what that battmax means i guess its in VESC settings. i read everyday in this forum about all sorts of things, slowly getting somehere :) im thinking to use samsung 30Qs they are rated at 15A so that would make 60A discharge i will get 10A headroom if that makes any sense.
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-12-26T21:18:15.940Z Reads: 82

```
the 30q are safely rated at 20a, but it'd be good treat them as if they're 15a.  good to leave headroom like you said.

yea, batt max is a vesc setting, it limits how much current the controller will pull from your battery pack.  so...set it 60a total across the two motors (30a each) and you should be good.

also, keep in mind there's a 2qt minimum order when ordering from bestech.
```

---
## \#5 Posted by: Zyb Posted at: 2017-12-27T12:52:32.702Z Reads: 54

```
ok got it :slight_smile:  i just got a response from bestech saying this model is discontinued. i thought it was perfect for me. the popular option at 80A is HCX-D223v1 but its really tall 25mm compared to what i chose which was 8mm. i think the next best thing is this one (13mm tall) with built in e-switch but rated at 60A http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCB-D345.html

theres this one rated at 60A aswell looks slim enough in the pictures http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html but people say if you go out with full charge and try to brake, it will cut off the power to prevent overcharging the batteries. this particular scenario is not happening with bestech products. other than that its not bad for its price i think.
```

---
## \#6 Posted by: pjotr47 Posted at: 2018-02-04T20:28:16.031Z Reads: 35

```
I have 3pieces laying arround and at all of them the e-switch is not working good. I want to suggest to don't order this model
```

---
