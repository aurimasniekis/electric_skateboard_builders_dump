# DOA DIYEboard esc?

### Replies: 21 Views: 885

## \#1 Posted by: uncosk8r Posted at: 2018-04-05T11:03:57.545Z Reads: 193

```
So, I finally received some parts from diyeboard today and while most of the parts seem to be in order and the housing looks pretty good (my 3d printed ones didn't last...), except the ESC appears to be DOA.

I've Verified 36V on the battery as well as on the input blobs of solder on the esc, but when I try to turn on the esc, nothing happens.

No lights, no sounds, no spark when plugging in the battery, nothing.

I can see a few solder pads that say "6s" and "7s", neither of which are bridged; If that makes a difference.

When I connect the battery, the voltage drops to 5v, and creeps up very slowly to about 22v.
Once the voltage has crept up, if the on button is pushed it starts to beep and light up (as the voltage rapidly drops back down) but then goes dark and quiet again allowing the voltage to creep back up.

If it makes a difference, this esc is the double hub motor version and appears to be the "v2" with the two layers of pcb soldered together at the corners with some pins.

This is a *BRAND NEW* esc that has not successfully turned on, even once.
      (They claim that they test parts before sending them out (to justify not having a warranty!), but I'm going to have to call "b**-****t" on that  because if they had so much as plugged this esc in, they'd have seen that it wont even power up!)


Does this place have a reputation for ripping people off like this, or are the likely to fix this?

Am I missing something simple, or is this esc as it appears, doa?

Where do I even start in troubleshooting it to try and get it working? (I have a hot air station and know how to use it, but haven't used it because I don't want there to be any question that the board was DOA and that I didn't do anything to destroy it.

I have a hot air station and know how to use it, but I think that a brand new out of the bubble wrap esc should at least work when its delivered. (and as such am assuming that I'm missing something or doing something wrong.....)
```

---
## \#2 Posted by: Guacamoleface Posted at: 2018-04-05T11:06:15.598Z Reads: 173

```
Just contact him, he seems very helpful to me. 

Shit happens during shipping.
```

---
## \#3 Posted by: uncosk8r Posted at: 2018-04-05T11:09:37.367Z Reads: 169

```
wow, that was a quick reply, thanks!

I sent an email to the address "info@diyeboard.com" but haven't gotten any reply; Is there another address that I should have used?

How else can I contact him?
If the one I've used is wrong, do you know the right one?
```

---
## \#4 Posted by: Guacamoleface Posted at: 2018-04-05T11:12:04.914Z Reads: 159

```
Im not completely sure to be honest with you. 

But if you go to their webpage you have the contact form aswell as they have a live chat, Try that!
```

---
## \#5 Posted by: uncosk8r Posted at: 2018-04-05T11:15:19.578Z Reads: 143

```
Oh, I didn't know that had a chat on their website, Ill try there now......

thanks
```

---
## \#6 Posted by: Ishayc Posted at: 2018-04-05T11:33:42.766Z Reads: 137

```
Talk to Jason, he’s their representative @diyeboard
```

---
## \#7 Posted by: telnoi Posted at: 2018-04-05T12:37:54.570Z Reads: 130

```
It has more solder bridges than that. I would first verify if you are actually using the correct voltage for what the esc has been set to. If not, who knows what might have happened.
```

---
## \#8 Posted by: pat.speed Posted at: 2018-04-05T12:42:18.992Z Reads: 127

```
What sort of battery are you using? And are you sure the button is plugged into the correct port?
```

---
## \#9 Posted by: TarzanHBK Posted at: 2018-04-05T13:16:12.037Z Reads: 118

```
[quote="uncosk8r, post:1, topic:51297"]
When I connect the battery, the voltage drops to 5v, and creeps up very slowly to about 22v.
[/quote]

That is a strange behavior. Check the Battery and charge it, to verify that you don´t have a defective one.
```

---
## \#10 Posted by: uncosk8r Posted at: 2018-04-05T14:07:12.915Z Reads: 103

```
well, no go on the chat on their website; it just kept timing out with a "no reps available send an email " message, but I did use their support form to submit a message in yet another place; I'll not assume that its like yelling at a brick wall until at least tomorrow or the next day....

@telnoi That makes sense, but I couldn't find any documentation about the newer two layer esc, and when I had a look over the pcb (with a usb microscope) I couldn't see any other bridges on the areas that I could access; Its possible that there are some in between the layers of pcbs, but I didn't want to start de-soldering it to separate them and risk giving @diyeboard any chance to say that it wasn't DOA and that I'd done something to kill it, and since I ordered it as a 10S esc, one would think that the bridges should should be set as 10s anyway.....

Can you tell me where to look for the other bridges you're talking about?

@pat.speed, I'm using a 10s3p battery that they sell, didn't even have to solder the connectors to it; specifically made for that setup and esc....I caved and bought their housing and battery since I was having problems with the terrible roads here combined with my 3dprinted housing causing the spot welds on my last battery to keep breaking.
;I'm certain that I've plugged the button into the right place, as it says "LED, GND, GND, POWER" on the board side connector and the connector doesn't fit anywhere else on the board.....I even connected the pins on the back of the connector momentarily (the button does exactly the same thing except at the end of some wire) to eliminate the connector being a culprit, to no avail.

@TarzanHBK, I agree, however, I'm fairly certain its not the battery as I also tested the ESC with another known good 10s4p pack that I've got and got the same results; Best I can tell is that its as a result of a capacitor charging up. (which makes sense in how it will start to power up for a moment as the voltage falls rapidly again)

The battery is at 36V....that should be more than enough to simply turn on the circuit as the cutoff voltage isn't supposed to be until around 3v per cell (30v)....I also tried testing with a fully charged 10s4p pack (which was at 41.8V) and it didn't make any difference....

I'd test that pack on something else, but unfortunately I don't have anything else that can handle that sort of voltage (not anything that draws a significant load anyway....) 


@diyeboard, can you shed any light on this? 
.......
```

---
## \#11 Posted by: TarzanHBK Posted at: 2018-04-05T14:38:19.299Z Reads: 92

```
If you tested it with another one, i´m pretty sure the ESC is broken somewhere...
```

---
## \#12 Posted by: XTLA Posted at: 2018-04-05T14:44:40.469Z Reads: 91

```
Try to reach jason@volansboard.co
```

---
## \#13 Posted by: uncosk8r Posted at: 2018-04-06T01:25:23.040Z Reads: 83

```
well, it seems that although the battery seems ok (it reads just under 36v) the charger they sent may also be defective.......

I've tested the esc with another known good battery, but had no change in the results, so there is definitely a problem with the esc, but it appears the charger is defective also.

Plugged in, the green light goes on and the output reads 42V, but despite lifting the battery voltage slightly (by 1/2 a volt) the led doesn't turn red and it does not draw *any* more current vs just plugged in when plugged into the battery. (my inverter has a digital ammeter....)
I left it plugged in to both 240v ac and to the battery overnight thinking that the draw was low because it was full and the current was past the "starting to taper" point, but the battery voltage and the "sitting on the charger voltage" was actually slightly (0.2v) *lower* when i checked it this morning. (the charger doesn't appear to actually start the charge cycle...)

(EDIT, Ive tested the charger and the esc independently with a known good and working battery; I'm confident that the problem isn't the battery)

I mean, I can just rig up another charger and would probably use the house-bank driven charger 90% of the time anyway, but Ive paid good money to get parts that work without having to do that; It's just not acceptable that not only one, but 2/3 of the non "simple piece of plastic" parts are DOA.



@XTLA thanks, I'll do that now; hopefully he will be able to salvage this situation!
```

---
## \#14 Posted by: Sender Posted at: 2018-04-06T02:23:54.232Z Reads: 78

```
I hate to say it, but this sounds eerily like a "buy cheap, buy twice" sort of situation. I hope I am wrong though.
```

---
## \#15 Posted by: uncosk8r Posted at: 2018-04-06T05:14:28.867Z Reads: 74

```

@Sender 

 An item not lasting is one thing, but one that doesn't work at all out of the box is quite another; this was sold as an esc, and as far as function is concerned it is a paperweight.
```

---
## \#16 Posted by: uncosk8r Posted at: 2018-04-07T02:44:02.454Z Reads: 67

```
Well, they have finally started replying to my emails.

Still no solution, but at least they seem to have quit with the  "we test before we send out, so its not defective" line. (but only after I made/posted a video demonstrating the problem; which they demanded despite the fact that every shred of info in the video was already in the previous email I had sent....)
```

---
## \#17 Posted by: pat.speed Posted at: 2018-04-07T03:21:33.936Z Reads: 62

```
That’s normal for them, they always ask for video evidence because it could help them to diagnose what’s actually wrong, or if there is a simple fix before shipping it back to China. It also does take a day or two for them to respond sometimes but apart from that they seem very helpful
```

---
## \#18 Posted by: banjaxxed Posted at: 2018-05-14T21:58:37.995Z Reads: 57

```
I've just hit the same problem, looking for 10s, desoldered the 7spins and hookedmy known good 10s pack and beepbeepbeep ad nauseum,any fix? maybe it's only something fixable via firmware
```

---
## \#19 Posted by: hyperIon1 Posted at: 2018-05-15T01:47:58.330Z Reads: 54

```
yea, ill put my 2 cents  in, there service/support via email sucks , no return policy on anything electric, BS. I bought two 12s4p batteries from them and could even get them to full charge, then week and half of argument via email on if I was plugging it in correctly.......
only returned the batteries after I threatened to open them up in from of a video camera. RMA the next day..... last time I bought from them, end of story
```

---
## \#20 Posted by: hyperIon1 Posted at: 2018-05-15T01:53:19.595Z Reads: 52

```
This was before we started offing custom packs built to suit, we walk you through the process answer any questions and you get pics of your build as its being done.... you see whats in your battery pack as its being built, quality and attention to detail is our SOP.
```

---
## \#21 Posted by: banjaxxed Posted at: 2018-05-15T09:58:32.073Z Reads: 41

```
Well it seems I fixed the beepbeepbeep problem, but unfortunately by killing it somehow.
no lights,no knowledge on these escs bah
```

---
