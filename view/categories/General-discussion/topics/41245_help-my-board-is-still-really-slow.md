# Help! My board is still really slow!

### Replies: 33 Views: 2210

## \#1 Posted by: mikeydog43 Posted at: 2017-12-17T06:39:22.632Z Reads: 241

```
Hi guys/gals

Fairly new here, but definitely have been reading before I was even a member. I read another post about someone else's board being slow but it seemed they got it figured out with gear ratios. I have a pennyboard that I put bigger trucks, 270kv motor, 70mm wheels, and had a 16:48 gear ratio on a 6S battery with the same ESC as the Meepo board. Was getting about 7-8mph full charge...

Recently upgraded to 90mm wheels, 15:36 gear ratio on a HTD 5m belt, and it is way more sturdy than what I had. I am STILL getting only 8-9mph full charge and I did gain more torque going uphill but where is the speed! I used a calculator at a low 60% efficiency and it says I should be getting 15.8 MPH....What am I doing wrong?
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-12-17T06:42:14.394Z Reads: 233

```
post a picture of your setup, it'll help us pinpoint the problem.
```

---
## \#3 Posted by: scepterr Posted at: 2017-12-17T06:42:38.222Z Reads: 228

```
Isn't the meepo 10s? I would say low voltage is your issue
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-12-17T06:44:36.609Z Reads: 223

```
he should still be doing better than 9mph with 6s and that motor/gear ratio.
```

---
## \#5 Posted by: scepterr Posted at: 2017-12-17T06:45:17.590Z Reads: 213

```
On those ESC, I dunno, they have a fixed voltage setting and cutoffs
It might be that it's a 7S version...6S would work but in low power
```

---
## \#6 Posted by: mikeydog43 Posted at: 2017-12-17T06:45:59.529Z Reads: 209

```
<img src="/uploads/db1493/original/3X/d/1/d1115fea4c0932ea4f6b169b177a7ff704d9507c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/a/dac6ee3e01c82cff1ac00a60df04c1e78d971977.JPG" width="666" height="500">

kind of in shambles at this point, I took everything off but these were some pictures without the ESC in, I can put it back together and take some more tomorrow. But that ESC lets you choose 6S 7S or 10S
```

---
## \#7 Posted by: scepterr Posted at: 2017-12-17T06:46:31.298Z Reads: 203

```
Are you sure you chose 6S?
```

---
## \#8 Posted by: mikeydog43 Posted at: 2017-12-17T06:47:28.355Z Reads: 202

```
yep, I had an earlier problem where I didn't realize it was on 7s, and it keeps beeping until you have the right setting on for the battery
```

---
## \#9 Posted by: MysticalDork Posted at: 2017-12-17T06:48:21.091Z Reads: 199

```
have you checked your battery voltage and current?
```

---
## \#10 Posted by: mikeydog43 Posted at: 2017-12-17T06:50:36.859Z Reads: 194

```
When I charg on the imax b6, I stop them at 12.6V but I have not checked current on them yet. I used a voltmeter before when they weren't on full charge but still had a little over 11V on each
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-12-17T06:51:16.961Z Reads: 190

```
what batteries are you using? Do you have a photo of them?
```

---
## \#12 Posted by: scepterr Posted at: 2017-12-17T06:52:10.884Z Reads: 187

```
Nvm, it's late 😋
```

---
## \#13 Posted by: mikeydog43 Posted at: 2017-12-17T06:52:36.154Z Reads: 185

```
<img src="/uploads/db1493/original/3X/8/e/8e48c949ab1d1c1bef79eebf293e71f69f85d449.JPG" width="666" height="500">
```

---
## \#14 Posted by: mikeydog43 Posted at: 2017-12-17T06:53:10.926Z Reads: 179

```
And I connect them in Series not parallel so definitely have 6S
```

---
## \#15 Posted by: MysticalDork Posted at: 2017-12-17T06:55:08.734Z Reads: 181

```
Haha, good to know. Had a fellow on here a while back that had his pack all kinds of miswired. Do you notice any improvement when the batteries are fully charged, rather than nearly dead? (11v is getting near the bottom.)
```

---
## \#16 Posted by: scepterr Posted at: 2017-12-17T06:55:10.086Z Reads: 178

```
Silly question, does your remote have a speed mode switch?
```

---
## \#17 Posted by: mikeydog43 Posted at: 2017-12-17T06:59:56.632Z Reads: 172

```
I haven't ridden too much since the 90mm upgrade but it seems full charge did nothing since I only gained a MPH on full charge and bigger wheels from the 70mm. The remote does have a fast and slow mode and i was on the fast mode when i tested
```

---
## \#18 Posted by: pennyboard Posted at: 2017-12-17T07:22:21.239Z Reads: 171

```
Are you sure you’re not hitting the erpm limit on your Esc? 270kv and 6s might get you there.
```

---
## \#19 Posted by: Wilsonliang777 Posted at: 2017-12-17T08:41:45.898Z Reads: 165

```
I think the meepo board uses hub motors so the esc is designed for hub motors with a max rpm limit.   I have one of there ESC.  My set up is 10s 7000mah, 40/20 gears and 90mm wheels and dual 200kv motors.  I get like 19 to 22mph.   And I use the same brand of batteries as you
```

---
## \#20 Posted by: bigben Posted at: 2017-12-17T09:18:14.007Z Reads: 168

```
Can you show the wiring in the box with the batteries connected?
```

---
## \#21 Posted by: pat.speed Posted at: 2017-12-17T11:29:05.615Z Reads: 145

```
I'm pretty sure @Wilsonliang777 has the right idea. If it is the esc from banggood I'm pretty sure that is the hub motor version
```

---
## \#22 Posted by: mikeydog43 Posted at: 2017-12-17T13:29:27.867Z Reads: 137

```
@pennyboard I am not sure how to tell if I am or not from the ESC. The motor definitely spins up good and then maxes out really fast but I don't get why it is different from other set ups. Is it a possibility that the ESC is mostly just ideal to be set up on 10s basically? I will put it back together and take a lot more pictures today (soon).
```

---
## \#23 Posted by: Okami Posted at: 2017-12-17T13:35:39.953Z Reads: 140

```
Did u buy from person or ebay? Maybe @dickyho has experienced this..

Sort of sounds likeu got hub motor version, which has way less rpm per motor when spinning the wheels.. ive heard the ebay esc is also limited to 40kph or so, so in your case u get 3x lower limit
```

---
## \#24 Posted by: mikeydog43 Posted at: 2017-12-17T14:13:13.326Z Reads: 133

```
I was unaware of a difference between hub motor version, and I can't find a lot of info on these things.
This is from the right seller - but the listing has changed, and it is not the same version. But that is what I am currently on.
https://www.ebay.com/itm/For-Hub-Motor-Dual-motors-longboard-skateboard-control-modula-ESC-Substitute/332377676534?hash=item4d6340daf6:g:leIAAOSw3ZtaKl7T

And I have also used the banggood version with the same results.

https://www.banggood.com/Electric-Skateboard-Longboard-Controller-With-Remote-Dual-Motors-ESC-Substitute-p-1202299.html?rmmds=search&cur_warehouse=USA

And here are some pictures
<img src="/uploads/db1493/original/3X/5/5/5501b0c6ee190dee3da13a9022fbf48a521f4b9f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/1/81591b4d41cda4afbc07e08c402fdabe1fde66db.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/1/4151d89bc4882a0546473027ce7be5a087e28582.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/4/c/4cc06b73165206a4eab7ac7658ed1cf8c9e13ea7.JPG" width="375" height="500">
```

---
## \#25 Posted by: mikeydog43 Posted at: 2017-12-17T14:20:12.941Z Reads: 120

```
Battery 1: 12.41 volts
Battery 2: 12.38volts
after series connector: 24.8 volts

So it is definitely getting good power
```

---
## \#26 Posted by: Wilsonliang777 Posted at: 2017-12-17T16:03:11.338Z Reads: 119

```
Banggood sells the hub motor ESC, That is 99% for sure.  And the eBay listing you posted also said hub motor.    So the solution to your problem is to buy hub motors or increase voltage to 10s or keep increase gear ratio or buy new not hub motor ESC.  

  When I use the esk8 calculator to figure my speed I set the my motor kv to 120kv instead of my real motor kv of 200kv.  And the result is pretty correct.
```

---
## \#27 Posted by: banjaxxed Posted at: 2017-12-18T13:56:05.666Z Reads: 104

```
This? The product spec says nothing about it being for hub
https://www.banggood.com/Electric-Skateboard-Longboard-Controller-With-Remote-Dual-Motors-ESC-Substitute-p-1202299.html

Edit:ok I spent more time looking through the product description and although it doesn't say it there the reviews/Q&As seem to indicate this is for hub motors...blueergh
```

---
## \#28 Posted by: Wilsonliang777 Posted at: 2017-12-18T16:34:56.507Z Reads: 94

```
Banggood is not that good with details.  They don't change listing or correct them.  And CS agents don't know the items that they are selling because  they sell so many things.  They do have a good refund and keep the item police.
```

---
## \#29 Posted by: mikeydog43 Posted at: 2017-12-19T16:05:54.535Z Reads: 82

```
So it didn't let me post I had to wait for 14 hours etc... but what it sounds like is that if its an ESC for hub motors, then use hub motors. :/ just ordered a set and I really hope it will fix this issue. Will update when I get them.
```

---
## \#30 Posted by: saul Posted at: 2017-12-19T20:15:17.927Z Reads: 75

```

wow it looks like **you cut off alot from the truck** to get the mount on.
I wouldn't go above 10mph on that! full size unmodified trucks have already snapped!
```

---
## \#31 Posted by: mikeydog43 Posted at: 2017-12-19T22:59:32.685Z Reads: 72

```
@saul unfortunately cheap motor mounts will do that haha but I've never had an issue with it so far.
```

---
## \#32 Posted by: Jreamer Posted at: 2017-12-19T23:06:21.962Z Reads: 66

```
My guess would be the problem is this esc is for hubs. That means that the ESC is expecting a 1/1 gearing ratio and you do not have that.
```

---
## \#33 Posted by: saul Posted at: 2017-12-20T12:10:41.691Z Reads: 62

```
[quote="mikeydog43, post:31, topic:41245"]
I've never had an issue with it so far.
[/quote]

yea but you do, you won't see it coming. thats the problem!
```

---
