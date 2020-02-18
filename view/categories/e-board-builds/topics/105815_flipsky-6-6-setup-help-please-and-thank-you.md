# Flipsky 6.6 setup Help Please and Thank you

### Replies: 9 Views: 155

## \#1 Posted by: VIZOVIZOVIZO Posted at: 2020-02-06T16:33:44.147Z Reads: 52

```
I![image|375x500](upload://sqdHVRILyh6pdosm6QrFcVWhPpQ.jpeg) ![image|375x500](upload://227h6KNeXWz2Z7cCZsXS3WXG7tf.jpeg) ![image|375x500](upload://bvfXXkOfWub1sli7ZXUfEl2TmzX.jpeg) ![image|375x500](upload://ezKwEeDtrC7fuaDa0kktkTSkfeh.jpeg) ![image|375x500](upload://vgjXvSwh8WGzFVjo5THhZZfiiUe.jpeg) ![image|666x500](upload://5RZ3QTprFqzzfzM2EstApveRAff.jpeg) ![image|375x500](upload://eSvHLnuypE72UBoxY460IPe7F1L.jpeg) 

![image|375x500](upload://asbWIeCuq3ZJM2vwBld5esDk1gs.jpeg) 


Thank you for looking at this thread. 😊


So here’s my dilemma, for some reason my VESC  6.6 won’t power up and stay on when I push the power button for the anti-spark switch.....

Now the VESC does light up for about two seconds and then the power dies out (this is something that happened very recently which now I’m baffled by).

The other thing is I want to know how I can set up the VESC so I can get more power to the motors.

I use the quick set up configuration and everything works but I have very little low in torque. I mean it really takes forever for me to get to a good decent rate of speed.

I’ve got a 16 tooth gear on the motors and a 58 gear  on the 7 inch all-terrain tires.


Unlike most riders I’m a big guy(6’5” 270 pounds) so I’m wondering if I need lower KV motors to get more torque?

The board itself probably weighs close to 45 pounds it’s not lite at all.

I used to have an evolve carbon GT and I remember even with the weight I’m at now that board would move me along EASILY!

As you can see from the photos my battery is a 
12S5P (I don’t know if I said that right , You get the idea). 

The board is just a blank deck that I bought off of eBay that I had to reinforce with fiberglass and I had to slightly modified the battery box to accommodate how big/thick the battery is.

Thank you all again who looked at this post
```

---
## \#2 Posted by: Wilsonliang777 Posted at: 2020-02-06T22:05:07.740Z Reads: 37

```
It's hard to say why you have low torque becasue we don't know the setting on the vesc and what amp your battery could provide.
```

---
## \#3 Posted by: AgressivStreetLamp Posted at: 2020-02-07T00:12:25.668Z Reads: 34

```
Hey dude,
First and foremost go to forum.  they will respond with more expertise and faster.
also, you dont have a VESC, you have a FSESC. VESC is by Trampa 
On to your issues
Your power problem sounds most like a loose connector or low battery. Or you might try holding the power longer

For more torque just increase the amps. Youll have to know what sort of amps your battery can do but you can set the battery amps to around 50 at least. and motor amps can go high, like 100A though it wont matter becasue its limited by the battery amps

another method would be to change gearing. although that gearing sounds ok so try the new settings first
```

---
## \#4 Posted by: AgressivStreetLamp Posted at: 2020-02-07T00:15:50.313Z Reads: 33

```
looking at this link:
https://matrixbatteries.en.alibaba.com/product/62045234654-807343280/44_4v15ah_lithium_ion_skateboard_battery_12s5p_battery_pack.html

it is rated only for 4.5A , youll need at least 10x that to work properly
Chances are your problems are from a complete garbage battery thats not providing enough power
```

---
## \#5 Posted by: VIZOVIZOVIZO Posted at: 2020-02-07T03:32:40.943Z Reads: 30

```
OMG thank you so much for finding the missing piece of the puzzle!  

When I bought that battery I was thinking "wow this is a huge freaking battery! It'll do...) 

#FAIL

What would be a good/high Amp output batter for duel 6374 motors?  

I bet I could even take that batter apart and have it reconfigured what do you think?

Thank you guys again for your help TYTYTYTYTYTYTYTYYTTY
```

---
## \#6 Posted by: AgressivStreetLamp Posted at: 2020-02-07T04:24:22.528Z Reads: 30

```
Not a problem

[quote="VIZOVIZOVIZO, post:5, topic:105815"]
What would be a good/high Amp output batter for duel 6374 motors?
[/quote]

Realistically youre looking for something around 80 amps  if you're looking for torque and want to really use the power. the more the better
I would suggest finding a 12s5p made with specifically Samsung 30Q cells. since that is the size you have anyway. The important thing is to make sure the cells used to make the pack are good. 30Q are the standard for our application and a 12s5p will blow your mind as far as power is concerned
```

---
## \#7 Posted by: VIZOVIZOVIZO Posted at: 2020-02-07T08:51:42.242Z Reads: 30

```
Again I can’t thank you enough for your counsel you really help me out.
```

---
## \#8 Posted by: MrDrunkenMobster Posted at: 2020-02-07T13:50:42.857Z Reads: 26

```
[quote="AgressivStreetLamp, post:3, topic:105815"]
go to forum. 
[/quote]

👆 Seriously, this. If you are wondering why this forum seems so dead, is because we are all over on the new forum now.
```

---
## \#9 Posted by: AgressivStreetLamp Posted at: 2020-02-07T15:00:10.173Z Reads: 24

```
Just want to make sure you know that this forum is closing soon. So head over to forum. 
Enertion is belly up and they own this place. Best move your things now. 
Im me when you've registered and I'll help you out.
I'm sure we can find you a battery
```

---
