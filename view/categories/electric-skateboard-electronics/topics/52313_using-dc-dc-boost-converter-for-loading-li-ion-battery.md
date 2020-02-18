# Using DC-DC boost converter for loading Li-Ion battery

### Replies: 23 Views: 1950

## \#1 Posted by: Nexo Posted at: 2018-04-15T11:12:48.607Z Reads: 165

```
Hi there,

I just wanted to ask what is your opinion about using converter like this:

https://scontent-arn.xx.fbcdn.net/v/t1.15752-9/30740242_1568855723161805_3250981589542240256_n.jpg?_nc_cat=0&oh=25a299903893334c7a0ceec84b784e05&oe=5B75208A

for loading 12s Li-Ion pack via BMS.

Main problem in my opinion is, that this converter will give constant 50.4V@10A when set at powered properly. As far as I know, li-ion should be charged in 3 steps, pre-charge, charge, and then lovering amps to get to 4,2V slowly.

But this forum is of course to ask, discuss and get other's opinion, so tell me what you think :smiley:
```

---
## \#2 Posted by: pat.speed Posted at: 2018-04-15T11:19:24.524Z Reads: 157

```
As long as it is a cc/cv charger it will work. If not, no it won’t although you could always use that first and then into a buck converter that has cc/cv. 

Or yanno get a brick charger although a bit expensive for 12s
```

---
## \#3 Posted by: Nexo Posted at: 2018-04-15T11:31:05.067Z Reads: 157

```
https://pl.aliexpress.com/item/WAVGAT-1500W-30A-DC-DC-Boost-Converter-Step-up-Power-Supply-Module-In10-60V-Out-12/32828748704.html?aff_platform=link-c-tool&cpt=1523744597346&sk=EI6YZJU&aff_trace_key=d36006221edb4e67bd6afcf795b33fef-1523744597346-05103-EI6YZJU&terminal_id=b0e1c7ed837a4dbd9fd264d2eadc36bf

take a look :slight_smile:
```

---
## \#4 Posted by: Acido Posted at: 2018-04-15T12:01:42.907Z Reads: 140

```
you are trying to charge your battery with this?
```

---
## \#5 Posted by: Nexo Posted at: 2018-04-15T16:52:55.760Z Reads: 128

```
just asking

I saw one guy using something like this for charging e-bike battery

https://www.youtube.com/watch?v=vGrBT_P9Xfc&t=1s
```

---
## \#6 Posted by: JdogAwesome Posted at: 2018-04-15T21:58:16.748Z Reads: 109

```
From the looks of it yes that is a Constant Current, Constant Voltage boost converter so it should work well for charging your battery.
```

---
## \#7 Posted by: b264 Posted at: 2018-04-15T22:10:40.566Z Reads: 103

```
I would not charge a lithium battery with this because there is a lack of information about what it does.  It seems like it's not the correct thing, despite the words "constant current" being on the page after automated translation.

You should not charge lithium batteries with power supplies.
```

---
## \#8 Posted by: Eboosted Posted at: 2018-04-16T02:28:47.227Z Reads: 97

```
Have you seen this? This is what you need:

https://www.electric-skateboard.builders/t/my-adjustable-portable-charging-station/52289/2
```

---
## \#9 Posted by: Nexo Posted at: 2018-04-16T04:48:53.635Z Reads: 85

```
it is completely the same, isn't it?
```

---
## \#10 Posted by: Eboosted Posted at: 2018-04-16T06:44:51.044Z Reads: 83

```
No. I think there are differences, but the one I got has voltage calibration from 12 to 60v
```

---
## \#11 Posted by: ARetardedPillow Posted at: 2018-04-16T07:05:49.702Z Reads: 81

```
http://www.electric-skateboard.builders/t/programmable-supply-power-60v-15a-35/36797?u=aretardedpillow
```

---
## \#12 Posted by: haand22 Posted at: 2018-04-16T12:54:16.532Z Reads: 72

```
Made a guide a while ago:
https://www.instructables.com/id/How-to-Charge-Your-Lithium-Battery/
```

---
## \#13 Posted by: Nexo Posted at: 2018-04-22T21:12:10.601Z Reads: 58

```
ok, but lets make things clear: can POWER SUPPLY and BMS be used as charger for battery pack? :face_with_raised_eyebrow:
```

---
## \#14 Posted by: bartroosen12 Posted at: 2018-04-22T22:11:47.644Z Reads: 56

```
Just buy one of these and you will save a lot of time using these constant current modules 😉
http://s.aliexpress.com/mqq6VnmU?fromSns=
I got the 10S version and it works perfectly fine ✌🏼
```

---
## \#15 Posted by: Nexo Posted at: 2018-04-22T22:32:03.749Z Reads: 54

```
https://pl.aliexpress.com/item/XINMORE-50-4V-8A-7A-Lithium-Battery-Charger-for-44-4V-Li-ion-Polymer-Scooter-E/32824774541.html

you are right...there is no point to make life harder :stuck_out_tongue:

just ordered 8A version :wink:
```

---
## \#16 Posted by: hyperIon1 Posted at: 2018-04-22T22:34:17.666Z Reads: 52

```
Just throwing something out there but what would you think about a wireless charging system? 
I’ve been talking to our design guy about one
```

---
## \#17 Posted by: Grolletje Posted at: 2018-04-23T11:57:52.517Z Reads: 46

```
I guess it would then take several days to charge, because of the low current supply. the phonechargers are also only 1,5 A where the normal plugs are over 3A
```

---
## \#18 Posted by: JdogAwesome Posted at: 2018-04-23T13:43:07.252Z Reads: 44

```
I think it would be a cool project however the inefficiencys would be your main problem and wouldn't make it commercialy viable. 

@Grolletje I don't think he means using a phone wireless charger lol. And if you did mean that then no, just no.
```

---
## \#19 Posted by: Grolletje Posted at: 2018-04-23T13:47:13.346Z Reads: 44

```
haha I was looking for an example :joy:
```

---
## \#20 Posted by: hyperIon1 Posted at: 2018-04-23T14:00:00.689Z Reads: 41

```
That’s for a phone. The Guy doing my designs is working on a project for high efficiency wireless charge bank for hand held devices. the discs are rated 3a and the volts are adjustable. just what he is working on. 
I asked him if it was possible, he said it is would just take some engineering. 
like a wall mounted close contact charging system.
just wanted some feed back........ thx
```

---
## \#21 Posted by: Grolletje Posted at: 2018-04-23T14:12:47.745Z Reads: 40

```
It sounds super awesome! 3A is more than enough if you do not want super fast charge (I mean for charging on the go)
```

---
## \#22 Posted by: hyperIon1 Posted at: 2018-04-23T14:19:52.131Z Reads: 34

```
It was funny the way it came up. I was in his office and he had these copper coil discs. I was like what the hell is that. He started to tell me and I instantly thought of a wall hanger with a positioned pad to wirelessly charge. With a receiving pad in you enclosure. 
Still kicking it around.
```

---
## \#23 Posted by: curry Posted at: 2018-12-11T12:25:38.190Z Reads: 16

```
https://www.amazon.com/gp/product/B07JZDSB7N
This is the [original item](https://www.amazon.com/gp/product/B07JZDSB7N) where I bought. Hope it can help you.
```

---
