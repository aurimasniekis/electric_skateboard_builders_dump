# A motor question before I pull the trigger

### Replies: 35 Views: 1929

## \#1 Posted by: Youssless Posted at: 2017-04-28T14:23:02.614Z Reads: 143

```
Hi guys,

I've had massive help from the community so far and I just need a pointer with this since there are more contradictions the more I read. 

Context: 95kg (get down to 75kg twice a year for fight weight), no steep hills, looking to commute for ~ 10 miles a day.

Parts:
Motor = (Sk3 6364 190kv) (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html1)
Pulley System = (12mm Enertion) (http://www.enertionboards.com/electric-skateboard-parts/12mm-wide-drive-pulley-kit/1)
Battery = (3x 30C 5Ah 3s in series) (https://hobbyking.com/en_us/turnigy-5000mah-3s-30c-lipo-pack.html1)
VESC = (DIY electric skateboards.com)(https://www.electric-skateboard.builders/t/sale-uk-vesc-motors-mounts-wheels-enclosure-gt2b-wheel-pulley-kits/21191)

Questions:

1) Higher KV motors provide higher speed on the eSK8 calculator and there was a thread by @chaka back in May 2016 claiming that the ideal KV for my 9s (33.3V) battery setup is ~ 257k according to the formula of 8570rpm/33.3V (voltage of batteries according to Hobbyking specs).

I'm looking to change the motor and get a SK3 6374 192KV according to advice I've received so far but wonder if I should opt for KV 6364 245KV according to Chaka's post so that I hit closer to that ideal range and have a higher top speed. 

1) Will I have enough torque with the 6364 245KV?
2) If I don't have enough torque, can I get away with giving the board a push-start? 

Thanks!

Youssless
```

---
## \#2 Posted by: jbalint1122 Posted at: 2017-04-28T14:53:33.711Z Reads: 123

```
I am also new to this, but SK3 6374 192KV should be about right torque and speedwise.
```

---
## \#3 Posted by: Youssless Posted at: 2017-04-28T16:06:28.332Z Reads: 115

```
But why? there are a fair amount of people, most of whom are very experienced based on their contributions to this forum and builds, who provide conflicting figures. The only one that's been explained is Chaka's post about the ideal KV to battery voltage (though I appreciate he doesn't delve into torque requirements, hence my question).

Why is 192KV best for a 95kg man like myself? can I not make do with a higher rated KV? Could I go higher but need to provide the board with a push-start?
```

---
## \#4 Posted by: Davey Posted at: 2017-04-28T16:50:01.801Z Reads: 108

```
I weight about 70kg and use a 430kv motor. This is way to much top speed and way less torque. Sure you can increase the kv but then need a push start. But if this isn't a problem you can go with a 245kv motor instead of 192kv. But the torque won't be better since the 245kv one is shorter and has more kv
```

---
## \#5 Posted by: jbalint1122 Posted at: 2017-04-28T17:42:26.419Z Reads: 102

```
I am only saying, that with a 192KV motor you still get good speed for regular commuting, but also have the torque for a standing start. Not to mantion, that maybe in the future you will want to go 10-12S, and for that voltage 245KV will probably be too high.

How fast do you want to go? 
Just asking because 192KV on 9s can get you up to more than 35km/h. If you want much more, and don't mind starting with a push, you can get the 245KV, it's your choice.

Are there any smaller hills or inclines near you?
If yes, that might be another reason to go with the lower KV.

Hope this helps!:slight_smile:
```

---
## \#6 Posted by: Ronny_CTS Posted at: 2017-04-28T17:49:04.711Z Reads: 91

```
Instead of buying that motor on hobby king perhaps you could join our group buy...its exactly for the same motor but it is being bought directly to the manufacturer (no hobby king intermediates) and therefore you can save a few dollars. 

https://www.electric-skateboard.builders/t/sk3-small-dual-motor-groupbuy/16671?u=ronny_cts
```

---
## \#7 Posted by: KTMinni Posted at: 2017-04-28T18:36:46.536Z Reads: 85

```
Rough idea of it:

Higher voltage = lower kV

Lower voltage = higher kV

Because kV means rpm/volt it would mean if you raise your voltage you need to lower your kV to keep a good torque/speed ratio.  

TL;DR for 10S the ideal kV is around 180-190 so if you go 9S  you increase the kV to keep the torque and speed the same
```

---
## \#8 Posted by: bigben Posted at: 2017-04-28T18:39:49.596Z Reads: 82

```
@Ronny_CTS I believe @Youssless is based in the UK. Is there an option to the uk? 
I would be interested if so?
```

---
## \#9 Posted by: Hummie Posted at: 2017-04-28T18:41:36.245Z Reads: 79

```
you can get as much torque from either it'll just take more amps from the 245kv.  if you want low speed torque you can also adjust the esc motor amp setting.  id just get it and you wont have a problem with the adjustability of the esc or cogs if need be.
```

---
## \#10 Posted by: Youssless Posted at: 2017-04-28T21:02:04.768Z Reads: 71

```
Thanks but where did you get the figure from? I'm only asking since it contradicts what Chaka's post was talking about.
```

---
## \#11 Posted by: Youssless Posted at: 2017-04-28T21:02:42.424Z Reads: 70

```
Indeed, good memory.
```

---
## \#12 Posted by: rwxr Posted at: 2017-04-28T21:05:45.370Z Reads: 67

```
Unrelated to your motor question, but just so you know, you will probably need to cut off a piece on both sides of your hanger if you're going with caliber trucks and enertion wheel pulleys due to them having an integrated bearing.
```

---
## \#13 Posted by: Youssless Posted at: 2017-04-28T21:10:13.234Z Reads: 65

```
Ooooh, this is something I forgot about. Is the mount only compatible with caliber II's? I think there was a guide I'll search for.
```

---
## \#14 Posted by: rwxr Posted at: 2017-04-28T21:11:56.041Z Reads: 62

```
Which motor mount are you planning on using?
```

---
## \#15 Posted by: Youssless Posted at: 2017-04-28T21:12:30.084Z Reads: 62

```
Enertion, bought it from the same guy I got the VESC and remote from.

Here: https://www.electric-skateboard.builders/t/sale-uk-vesc-motors-mounts-wheels-enclosure-gt2b-wheel-pulley-kits/21191
```

---
## \#16 Posted by: rwxr Posted at: 2017-04-28T21:15:39.676Z Reads: 57

```
Enertion motor mount only fits caliber 2's. What trucks do you have?
```

---
## \#17 Posted by: Youssless Posted at: 2017-04-28T21:16:56.426Z Reads: 62

```
Don't have them yet. Trying to find caliber II's that aren't £120+

I'll need to saw off part of each side?
```

---
## \#18 Posted by: rwxr Posted at: 2017-04-28T21:22:13.445Z Reads: 63

```
https://www.proto-boards.com/product-page/caliber-ii-fifty-degree-trucks

http://www.trampaboards.com/caliber-ii-longboard-trucks--10-inch-wide-with-a-50-baseplate-mount-for-fast-carvy-turns-p-12891.html

@longhairedboy cuts calibers on a daily basis and I'm pretty sure there are some guidance in one of his build threads
```

---
## \#19 Posted by: Youssless Posted at: 2017-04-28T21:28:02.074Z Reads: 59

```
Wow thanks! 

I've been looking, I'll need to see if I can get my hands on the right tools. Checking @longhairedboy's builds to see if he mentions how much to take off (roughly).
```

---
## \#20 Posted by: rwxr Posted at: 2017-04-28T21:28:50.525Z Reads: 60

```
https://www.electric-skateboard.builders/t/cutting-hanger-aluminum/15178

Here you go
```

---
## \#21 Posted by: rwxr Posted at: 2017-04-28T21:30:35.957Z Reads: 54

```
Found his video tutorial:

https://www.electric-skateboard.builders/t/enertion-truck-axel-not-long-enough/8793/12?u=rwxr
```

---
## \#22 Posted by: Youssless Posted at: 2017-04-28T21:34:40.459Z Reads: 50

```
Lol, forget Google, I shall just bother you for an eternity now!

Thank you, you've been super helpful!
```

---
## \#23 Posted by: rwxr Posted at: 2017-04-28T21:38:25.671Z Reads: 51

```
No problem. This forum has taught me a metric shitton of stuff and everyone has been super helpful, so I'm just trying to give back where ever I can :)
```

---
## \#24 Posted by: Youssless Posted at: 2017-04-28T21:45:17.781Z Reads: 49

```
Hopefully I'll be able to pass it forward. I'll look out for someone with a dremel though from this video: https://www.youtube.com/watch?time_continue=195&v=t6V4nBUFeYk it looks like I only need to do one side instead of both?
```

---
## \#25 Posted by: rwxr Posted at: 2017-04-28T21:48:19.635Z Reads: 49

```
Ah yes, one side for single motor. Both sides for dual motors
```

---
## \#26 Posted by: Namasaki Posted at: 2017-04-28T21:49:52.211Z Reads: 48

```
[quote="Youssless, post:1, topic:21964"]
1) Higher KV motors provide higher speed on the eSK8 calculator and there was a thread by @chaka back in May 2016 claiming that the ideal KV for my 9s (33.3V) battery setup is ~ 257k according to the formula of 8570rpm/33.3V (voltage of batteries according to Hobbyking specs).
[/quote]

I believe the main purpose of Chaka's thread on correct motor kv and voltage is to avoid exceeding the Vesc erpm limit, not necessarily finding the best balance of torque/speed. 
So, it's basically giving you the upper safe limit.
Also, when you calculate for erpm, you need to use full charge voltage, not nominal voltage.
A 9s Lipo at full charge will be 37.8v
8570rpm/37.8v=226kv
```

---
## \#27 Posted by: Youssless Posted at: 2017-04-28T21:52:22.017Z Reads: 46

```
You strike again! thanks @Namasaki!

I'm the type of person who needs reasons behind decisions. Thanks for this one, its helped clear up my head a little.
```

---
## \#28 Posted by: Hummie Posted at: 2017-04-28T23:38:09.342Z Reads: 44

```
Still waiting to see 6s vs 12s efficiency with same motors with the 12s having duty cycle limited to 47.5.  Such an easy test but my battery is soldered together 
With also no wind, a circle course and measuring the distance traveled till 100watthours spent. That would be the clincher.
```

---
## \#29 Posted by: KTMinni Posted at: 2017-04-29T01:47:49.917Z Reads: 38

```
I am not sure who exactly has said this but I've seen it a few places.  But the I just remembered that for 10s 180-190kv was best(because my board is a 10s)
```

---
## \#30 Posted by: Hummie Posted at: 2017-04-30T18:34:41.255Z Reads: 40

```
with the esc running close to the erpm limit it is most efficiency.  how efficient is still to be seen.
```

---
## \#33 Posted by: Youssless Posted at: 2017-04-30T21:39:46.752Z Reads: 38

```
What would you recommend? I live in the UK and options are limited.
```

---
## \#34 Posted by: KTMinni Posted at: 2017-05-01T01:40:09.058Z Reads: 38

```
Have you checked out alienpowersystems?
```

---
## \#35 Posted by: Iam319 Posted at: 2017-05-01T04:34:13.714Z Reads: 33

```
Does this rule apply to hub motors as well? Im ordering a 90mm 60kv hub motor using a 10s2p battery.
```

---
## \#36 Posted by: Youssless Posted at: 2017-05-01T09:20:52.025Z Reads: 31

```
Yes but I've been warned about how difficult it can be to find pulleys with 10mm bores and since options are limited here I decided to opt for the SK3 motor.
```

---
## \#37 Posted by: KTMinni Posted at: 2017-05-01T11:05:17.319Z Reads: 28

```
Fair enough, I haven't ordered from them.  The shipping was $60 to the US so that was a no go.
```

---
