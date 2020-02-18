# Help setting current and voltage limits with my FocBox

### Replies: 8 Views: 582

## \#1 Posted by: Fulabi Posted at: 2018-10-08T18:33:26.238Z Reads: 108

```
Hi all,

I’m about to receive the final part of my build (the battery) and I’ll then be ready to finish up my DIY build. Could someone please help advise me on what I should set the current limits and voltage limits at on my FocBox using the BLDC tool?

I’m using the below parts:

**MOTOR:** https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

**Model:** Turnigy SK3 6374 (192kv)
**Watts:** 4032W

**BATTERY:** https://pwrboards.com/collections/battery-parts/products/batteri?variant=4137258745887

**Model:** 10s3p (Samsung 30Q) - charge only BMS
**Volts:** 42V
**Amps:** 60 amps

I'm looking for advice on what to input the below in the BLDC tool:

_**Current Limits:**_

_Motor Max:_
_Motor Min (regen):_
_Batt Max:_
_Batt Min (regen):_
_Absolute Max:_

_**Voltage Limits**_

_Minimum Input Voltage:_
_Maximum Input Voltage:_
_Battery cutoff start:_
_Battery cutoff end:_ 

I'm a fairly heavy rider (100kg) so want to be make sure the I setup everything safely so I don't put too much strain on the components voltage wise. 

Thank you in advance.
```

---
## \#2 Posted by: totalgeek9224 Posted at: 2018-10-08T18:36:28.663Z Reads: 95

```
Following this thread. Wish i had the answers for you bud. But i too am a novice seeking answers
```

---
## \#3 Posted by: barajabali Posted at: 2018-10-08T18:50:56.417Z Reads: 95

```
Running default numbers is a good place to start with a 10s system
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-08T19:28:48.682Z Reads: 92

```
You run single motor?
I would start with
Mmax 60
Mmin -50
Bat max 40
Bat min -12

You can start your battery cut off start at 3v per cell and battery cut off end at 2,8v per cell as it’s a LiIon pack. 
For your 10s it would be 30v start 28v end.

Edit: don’t change the max and min input voltage settings. The stock settings fit.
```

---
## \#5 Posted by: Fulabi Posted at: 2018-10-08T20:12:06.521Z Reads: 86

```
Hi Andy,

Thanks for the feedback, much appreciated. 

Just co confirm yes running a single motor.
```

---
## \#6 Posted by: baxtred Posted at: 2018-10-08T20:32:43.166Z Reads: 84

```
Andy and I have slightly different opinions although here's what I recommend.

Mmax: 80A
Mmin: -80A
Bmax: 45A
Bmin: - 12A

Bascially just matching specifications. Motor is rated for max 80A, so 80A for max/min. Battery is 15A at 3P, so 45A. And a continuous charge of 4A per parallel group, so 12A.

These are the maximums you can do (well "safely"). If you have too much power or too much braking, you can always reduce this values. 

I'd personally start cutoff around 3.2v/cell and end at 3.0v/cell. A little more conservative than Andy although both will work. You'll get a few percent more range on the lower voltage cutoff at the expense of slightly reduced battery life.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-09T04:38:19.073Z Reads: 65

```
Good add on @baxtred 
I gave him just a starting point.
For sure he can set maximums but in my opinion better start low and adjust after to the right settings.
I for example had issues with motor max 80a as the motor got too hot (was a sealed 6374 thou).
If the focbox run cool with 40a you can go up with the amps. Don’t think that 45a is the limit.

For sure it’s not bad to set it more high but the 18650 you can drain till 2,5V. As the cut of starts at 3v you will not get a crazy voltage sag as you anyhow can’t accelerate hard. So I doubt that you will get spikes lower than 2,7v.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-10-09T04:46:18.098Z Reads: 61

```
With single that‘s fine.
As you probably already understood it’s everything relative. You can always adjust all settings in the limits of your hardware.
If you have a Bluetooth module I would recommend you to track your rides. With this data you can set up your max save values.
If your motor doesn’t get hot rise motor amps to 80a max.
If your breaks not strong enough, rise your motor min (or better to say make the value smaller as it’s a negative value).
Theoretically you can also set your bat min values to like -20a if you don’t break long hills it shouldn’t affect your battery.
Get temp data from your focbox. As long as it stays in the 40-60 degree range it’s all fine and you can slowly rise your bat max values.
With the right cooling or heatshink case you could get them even up to 60a 😉
```

---
