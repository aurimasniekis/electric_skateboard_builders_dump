# Changing TORQUE Rocket Dual/Single to FOC

### Replies: 9 Views: 823

## \#1 Posted by: afrokid Posted at: 2017-05-10T17:56:06.236Z Reads: 126

```
Hey peeps,

 I am currently on one motor right now since my other was sent in for a new one to dexter. So I decided to try FOC mode instead of BLCD mode out. It was a thousand times better in the way the board accelerated and deacellerated. My board randomly stopped working today on my way to work today. it still powers on and my remote does to. Just when I throttle nothing happens? I think maybe my vesc turned off? will have to look at when I get home. Not sure what setting I should adjust any one know here. I guess will Ask dexter later other wise but figure i should check with the community.

<img src="/uploads/db1493/original/3X/9/a/9acfbe17eefe2864c999651027a27a1857a88444.png" width="690" height="362"><img src="/uploads/db1493/original/3X/c/5/c5f1ec45029ca74d92e6dbf2be5206e96cc915f7.png" width="690" height="373">

I changed my setting based on what was already set for my torque by default and change bat cut start and end. all based on this video
https://www.youtube.com/watch?v=xSCEFK7Zljw
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-10T17:57:59.562Z Reads: 116

```
Turn on the VESC, try to slightly throttle, go to Terminal tab and type "faults". Report back.

If you have a DRV8302 fault, you burned your DRV chip and it'll have to be replaced. This is why a lot of people don't use FOC. I'm personally waiting until VESC6 to even touch FOC.
```

---
## \#3 Posted by: afrokid Posted at: 2017-05-10T18:13:30.038Z Reads: 108

```
Oh ok I was looking all over for any cons to FOC interesting cause in my opinion its a way better way for the board to work. this is from a new to DIY type of person.

So will probably have to buy a new VESC is there any company that has a VESC that works well with FOC also was thinking about setting up the Sensor motors in the future would this still be an issue using those ?
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-10T18:21:23.988Z Reads: 98

```
You should probably wait until the VESC6 comes out to use FOC, but you could try Ollinboard's VESC as they're very high quality. If you set up BLDC correctly, it should be comparably good and has higher top speed. While I haven't tried FOC, I have tried sinewave ESCs before.
```

---
## \#5 Posted by: Surfer Posted at: 2017-05-10T18:41:02.287Z Reads: 88

```
Also vesc-x is FOC proof, cheaper than vesc 6 and already available.
```

---
## \#6 Posted by: Stef Posted at: 2017-05-10T20:41:52.300Z Reads: 80

```
Is this a well known fact or your personal experience? I have two vesc-Xs and would not want to kill them with FOC.
```

---
## \#7 Posted by: Daan_vZon Posted at: 2017-05-10T22:41:32.977Z Reads: 70

```
Is using FOC so risky? Will might have to consider switching back to BLDC mode if it has such a high chance on damaging the VESC.
```

---
## \#8 Posted by: evoheyax Posted at: 2017-05-11T01:11:32.789Z Reads: 65

```
FOC is risky on VESCs that are not upgraded. I have 8 Chaka vescs running in FOC, and not a single issue. It depends on the manufacturer, and BOM they are building the VESC on. Chaka for example modified the BOM, which has increased reliability. Not all VESCs are created equally unfortunately.

@Stef FOC should not be an issue. The problems that caused this were specifically addressed in the VESC-X., just as they are in the VESC 6, which is not out to the public yet.
```

---
## \#9 Posted by: afrokid Posted at: 2017-05-11T15:37:03.561Z Reads: 40

```
 OK update it was probably my fault on top of FOC being risky my battery is 12s and I was following what the torque video was saying. I accidentally changed my Battery cut off start
Battery cut off end to way to low of a value you can see in screenshots. The battery he was using in the video was a 4s. 

The good news though is dexter is hooking it up even though it was my mistake and he will replace my vesc. What a homie :) Just gotta say dexter is super dope I swear I have been bothering him all week about DIY Logic and not once has he gave me cold shoulder on customer service help. 

Will probably stay in BLDC mode for now. Might order some extra vesc to try FOC mode out again in the future. Its just so much better than BLDC in the way the board worked.
```

---
