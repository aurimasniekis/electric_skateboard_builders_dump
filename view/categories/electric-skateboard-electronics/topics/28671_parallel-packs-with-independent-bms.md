# Parallel packs with independent bms

### Replies: 20 Views: 6046

## \#1 Posted by: krloz Posted at: 2017-07-26T09:42:11.323Z Reads: 282

```
I hope this hasn't been discussed somewhere else but I have searched and not found much. 
Up until now I have been using two 6s 5A lipo packs in parallel for 10A with a single bms. Balance leads paralleled also. 
I am now going to upgrade with a couple of 4S 5A packs to get a 10S2P 10A lipo pack. And as I have to change the bms I was thinking of separating the packs inn two. Each with its individual bms and paralleling only the outputs and charge inputs. Like in the diagram below.  Sorry for my crappy artwork.

<img src="/uploads/db1493/original/3X/7/3/736b30cdb4296b6950b32248dc1cac5643c5a182.jpg" width="666" height="500">

And now my reasons for doing this
I already have 2 10S bms. I was originally thinking of using only one
I should be getting double the charge current,  double the discharge current (if I ends up using bms for discharge) and double the balancing current (this last is what I like most)
Each set of two paralleled cells will not be balancing between themselves though the thin balance wires, during charge or discharge.  Only the bms balancing its own cells and the packs giving or taking power though their thick wires. 

What I an not fully sure is if one of the bms shuts of charging or discharging before the other one( the are not synchronized so this will happen),  what would happen around the parallel connections. 

Any one tried or knows? 
Thank you very much
```

---
## \#2 Posted by: Namasaki Posted at: 2017-07-26T15:13:13.651Z Reads: 242

```
I don't think you can run 2 bms modules together in parallel.
Not sure why you would want to either. 
You can connect two batteries in parallel and to one bms
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-07-26T16:22:00.072Z Reads: 231

```
can't you just wire the lipos in parallel and charge at 5 amps or less?
```

---
## \#4 Posted by: krloz Posted at: 2017-07-27T07:57:05.157Z Reads: 213

```
As I explained,  yes you can wire the packs in parallel to a single bms. That is my actual setup.  
After the diagram I explain why I would like to try this but my mayor concern is,  when you put together a lion pack, you wire cells in parallel with thick connections so they balance between themselves and then wire those in series to up the voltage.  If I wire 2 lipo packs in parallel I have each couple of paralleled cells balancing between themselves  through the thin balance leads.
Anybody else now if these would work or not.  I guess I could skip the discharge protection and have independent charge ports so as not to parallel the bms. Or maybe feed the charge to the bms through a diode
```

---
## \#5 Posted by: krloz Posted at: 2017-07-27T08:07:36.815Z Reads: 196

```
I hope that didn't sound mean. Not my intention at all. Any opinion is welcome.  I know what I ask is weird but I would like to try it unless anybody already has tried or knows if this would blow

@DavidBanner. @Namasaki
```

---
## \#6 Posted by: DavidBanner Posted at: 2017-07-27T08:14:29.733Z Reads: 174

```
you don't sound  mean at all :)

one idea that springs to mind is if you use a relay you could potentially electrically seperate the 2 packs during charging leaving each bms to do its own thing.

sparking might be an issue with a traditional relay? perhaps something like the vedder anti spark could be made?
```

---
## \#7 Posted by: krloz Posted at: 2017-07-27T09:10:04.531Z Reads: 170

```
That is a good idea. I don't think sparks will be a problem as im sure they're produced when you plug something power hungry,  like an empty pack of capacitors to something that can give bursts of power like lithium.
  I didn't understand why it would be good to separate the batteries while charging.  I am charging them though their bms so worst case if the batteries are connected is  If one charges faster than the other,  it would feed power to the other one via the big wires and charge it and the bms would perceive the same as if I was brake regen. Ie. Charging the batteries directly through its leads.
My idea to separate the bms charging ports is so no power would flow around when one of them cuts off for full charge
```

---
## \#8 Posted by: DavidBanner Posted at: 2017-07-27T19:26:15.322Z Reads: 153

```
I'm guessing from the lack of replies that no one (who has read this thread) has tried what you are suggesting or is willing to take a punt as to what might happen.

my logic in suggesting the isolation of packs/BMS is this: I like to simplify where possible, more complexity and more parts introduce points of failure and quite often cost. As running a single BMS with a single pack is a known quantity with lots of documentation and real world advice available, if it were me I would be aiming for that. Especially as mistakes made here can mean killing your board's expensive electronics or in the worst case a fire in your house while charging.

Cool thread though, I'd love for someone to come along and give a definitive answer and/or elegant solution which I could learn from.
```

---
## \#9 Posted by: willpark16 Posted at: 2017-07-28T00:35:37.135Z Reads: 140

```
Eon boards cruiser model
```

---
## \#10 Posted by: krloz Posted at: 2017-07-28T09:26:30.542Z Reads: 144

```
@willpark16
 
Ok. Been looking at that now for a while.  Very interesting design.  Do you actually own one of this or seen one? Would you know if the packs are connected In parallel simply by a couple of thick wires.  And if you plug in for charge do both packs charge at the sane time? 

This would answer all my doubts add this was basically my initial idea.  Included the plug and play batteries. 
Thanks for the info
```

---
## \#11 Posted by: krloz Posted at: 2017-07-28T09:27:55.897Z Reads: 129

```
It is true that it looks like something not a lot of people have tried.  The problem here is I'm not very much into keeping simple  xd
Thanks anyway. Will post if I finally try anything
```

---
## \#12 Posted by: darkkevind Posted at: 2017-07-28T09:39:40.880Z Reads: 130

```
You can definitely share one charging device/source to two BMS'.

I think that's basically what you want to do isn't it? You'll need a power brick that's capable of a amps of charge. What is the charge rate of each BMS?
```

---
## \#13 Posted by: krloz Posted at: 2017-07-28T09:46:39.399Z Reads: 127

```
@darkkevind 

The bmss I have are rated for 5A charge and 60A discharge. So using both I could charge each pack at 1C and use the discharge protection. Only one bms output (60A) would be excessively near my batt vesc limits.
And I can actually provide 42V 10A to my board xd
```

---
## \#14 Posted by: darkkevind Posted at: 2017-07-28T10:08:01.770Z Reads: 131

```
Discharging at 60A is fine. As long as your motor max in VESC settings aren't higher than the motor's max rating.

You'll need at least a 2A power brick then, 10A if you want to use the full charging current potential of your BMS'.
```

---
## \#15 Posted by: krloz Posted at: 2017-07-28T11:37:00.944Z Reads: 126

```
My max battery is actually 50A. Per vesc though, driving dual here so....
```

---
## \#16 Posted by: willpark16 Posted at: 2017-07-28T17:06:38.772Z Reads: 121

```
I'll look for u
```

---
## \#17 Posted by: cicero Posted at: 2017-10-30T04:24:16.525Z Reads: 96

```
Did this end up working out for you? I was looking into doing the same thing but I can't tell from these comments if you ended up wiring the two separate packs with bms in parallel successfully
```

---
## \#18 Posted by: krloz Posted at: 2017-10-30T09:25:33.036Z Reads: 94

```
Believe it or not.  Still on my to do list.  Doing a hell lot 
Of changes in my board with near to none time. I will tell what I find out. I do have all the various batteries and bmss in a box
```

---
## \#19 Posted by: NYCeboardDude Posted at: 2017-11-28T19:06:40.845Z Reads: 83

```
I wired 2 10s2p battery packs in parallel. They each have their own bms and roughly same voltage every time I connect. Few months now no issues.
```

---
## \#20 Posted by: yanggatang Posted at: 2019-01-15T22:46:44.243Z Reads: 42

```
Do you charge them separately?
```

---
