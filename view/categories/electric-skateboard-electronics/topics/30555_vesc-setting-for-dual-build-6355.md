# VESC Setting for dual build 6355

### Replies: 26 Views: 2462

## \#1 Posted by: joeadams101 Posted at: 2017-08-14T06:03:10.187Z Reads: 261

```
Hello recently I upgraded to dual motors and dual focbox's. What would be the optimal vesc settings for this build:

2 6355 190kv
2 focbox's
16/36
Space cell 10s3p


Here is what I currently have as default:



<img src="/uploads/db1493/original/3X/e/3/e33f68d5e2fe2acd42fdb4ef20122b38e618d78f.png" width="690" height="429">
```

---
## \#2 Posted by: Tomer Posted at: 2017-08-14T06:37:42.029Z Reads: 228

```
Did you try these settings in real world?

I run a single sensored 6355 with:
Motor max - 60A
Motor min - 50A
Batt max - 50A (if I remember correct)
Batt min - -12A

With those settings I get pretty good results. When I'll add a second motor (very soon), I think I'll just cut everything to half. I'm not sure if it's the right way to go with but it makes sense to me. Or maybe just cut 
in half the Batt min and the Motor min.
```

---
## \#3 Posted by: joeadams101 Posted at: 2017-08-14T06:40:18.065Z Reads: 225

```
I kinda went my own way of doing it now. Going out to test it. Will post results in a bit
```

---
## \#4 Posted by: joeadams101 Posted at: 2017-08-14T08:00:31.591Z Reads: 216

```
Update:

Went with these setting and everything is working fine. Though I wasn't able to hit 30mph+ just around 28. Maybe I have to change a setting in here.

<img src="/uploads/db1493/original/3X/9/7/97e6af50b954536590cba692b21f91608f61f649.png" width="535" height="285">
```

---
## \#5 Posted by: Tomer Posted at: 2017-08-14T08:04:07.097Z Reads: 212

```
What is the motor KV rating? Which gears do you use?
```

---
## \#6 Posted by: joeadams101 Posted at: 2017-08-14T08:04:29.976Z Reads: 206

```
dual 6355 190kv and 16/36
```

---
## \#7 Posted by: Tomer Posted at: 2017-08-14T08:18:29.949Z Reads: 207

```
Forgot to ask wheels size. I assume they are 90mm?
```

---
## \#8 Posted by: Luke Posted at: 2017-08-14T08:37:23.194Z Reads: 207

```
I would change the settings a little by putting 20 amps for battery max per vesc assuming you have a 40 amp fuse in the battery pack.
You will also only want to set battery min (regen) -6 per vesc. Assuming your cells can handle 4 amp charging like the Samsung 25r cells then -6 is ideal.
I run 60 and -60 for motor max and motor min respectively. 
 whatever you chose, you should upload some updated screenshots so we check that they're all good
```

---
## \#9 Posted by: joeadams101 Posted at: 2017-08-14T16:55:59.555Z Reads: 183

```
Wheel size is 90
```

---
## \#10 Posted by: joeadams101 Posted at: 2017-08-14T16:56:56.162Z Reads: 180

```
Yeah i checked and it has a 40 amp fuse. Changing batt max to 20. Yeah the space cell has 25r
```

---
## \#11 Posted by: joeadams101 Posted at: 2017-08-15T03:35:36.673Z Reads: 171

```
Update: Changed batt max to 20 on both and change the Battery min (regen) to -6. What I encounter was brakes were much weaker, at almost max speed it will almost not brake. And if I held the brake too long it will like snap out of braking and I had to let of the trigger and brake again....
```

---
## \#12 Posted by: joeadams101 Posted at: 2017-08-15T05:38:11.494Z Reads: 167

```
Would that be caused by turning the regen to -6?
```

---
## \#13 Posted by: joeadams101 Posted at: 2017-08-16T02:22:08.493Z Reads: 163

```
bump. Anyone else thinks its the -6 regen?
```

---
## \#14 Posted by: SeanHacker Posted at: 2017-08-16T02:37:06.321Z Reads: 156

```
Here's what your settings should look like with your setup. 

Motor max 60 (if the board is too powerful at slow speed reduce it, if it's too weak you can go up till 80)
Motor min -50 (if the brake is too powerful reduce it, if too weak you can go up till -80)
Battery max 30 (if the board is too powerful reduce it. You can go up to 40 max with your battery type if you like)
Battery min -10 (correct would be -8 but to have some space in times of crisis)
You will be surprised how powerful it will be.
```

---
## \#15 Posted by: joeadams101 Posted at: 2017-08-16T02:39:16.488Z Reads: 153

```
Interesting. I thought I had to split the values between the motors....each one caps Max Amps: 80 Amps. The batt is a 10s3p which has a 40 fuse. Am I wrong?
```

---
## \#16 Posted by: SeanHacker Posted at: 2017-08-16T02:40:53.188Z Reads: 152

```
I have the same setup. Other than I upgraded to a 10s4p Samsung 25r. I also use a 40amp fuse with my vedder switch and have had no issues at all. These are the settings I've been using and got from @Ackmaniac and they have been working like a dream.

I said 30 because its always good to got easy at first. If you want more you can bump your Batt max to 40 for each vesc and that would make 80 amps.
```

---
## \#17 Posted by: joeadams101 Posted at: 2017-08-16T02:44:20.114Z Reads: 148

```
Let me try those settings to mentioned then. Brb! Will update soon
```

---
## \#18 Posted by: SeanHacker Posted at: 2017-08-16T02:46:56.284Z Reads: 146

```
Sounds good dude. I think you're going to be impressed. Its just about perfect in my opinion. I hit 30mph no problem and have a nice cruiser with those settings/setup. Let me know how they work for you.


<img src="/uploads/db1493/original/3X/b/f/bf578e88eecd5b1535fd371f27ec604fe6ea9271.jpg" width="281" height="499">
```

---
## \#19 Posted by: joeadams101 Posted at: 2017-08-16T03:05:10.105Z Reads: 141

```
:O holy shit
```

---
## \#20 Posted by: joeadams101 Posted at: 2017-08-16T03:06:18.455Z Reads: 136

```
The acceleration is HUGEEEEEE my board does a fucking wheelie if I max trigger it from 0. @SeanHacker
```

---
## \#21 Posted by: SeanHacker Posted at: 2017-08-16T03:18:56.437Z Reads: 135

```
Hahaha. Yeah it can do that. Make sure you have set your ppm settings (Min/Center/Max) also. 

Is the board too powerful for you now? You can also use @Ackmaniac firmware and BLDC_Tool also if you like. Its really awesome and you can set your own throttle curves how you like it.
```

---
## \#22 Posted by: joeadams101 Posted at: 2017-08-16T03:24:41.839Z Reads: 137

```
Yeah I need to set those up properly although I believe they are fine. Any tutorials u know about for that? 

It is kinda at the beginning. But I can get used to it hahahaa
```

---
## \#23 Posted by: SeanHacker Posted at: 2017-08-16T04:30:31.303Z Reads: 137

```
Yep. Tons of info on setting those up. This is this 1st thing I get after using the search here https://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes-ppm/244
```

---
## \#24 Posted by: Battosaii Posted at: 2017-10-27T19:15:26.381Z Reads: 118

```
i was about to make a new thread to ask the same questions and i found this one.... @SeanHacker holy shitballs batman i feel like i just put a turbo on my Honda civic its way way faster. Wow is all i can say. I feel like i have to learn how to ride an esk8 all over again but i absolutely love it! I feel like i can take just about any board out there and im 130kg i almost want to know what 80amps feels like lmao
```

---
## \#25 Posted by: SeanHacker Posted at: 2017-10-27T19:25:13.655Z Reads: 113

```
Glad those settings are working good for ya dude.
```

---
## \#26 Posted by: ROFEN13 Posted at: 2018-01-24T14:57:14.639Z Reads: 89

```
What were your final settings on this? I have a similar board and am curious. Thanks!
```

---
