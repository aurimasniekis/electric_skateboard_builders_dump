# Regenerative Braking and BMS

### Replies: 20 Views: 2244

## \#1 Posted by: goldrabe Posted at: 2017-10-26T13:11:20.942Z Reads: 234

```
Dear builders,
i have an offer for a Samsung 30Q 10S5P battery pack for 260US$. It comes with a BMS which can handle 60A. Now my question is, can every BMS handle regenerative braking? I understand that the VESC limits the power which goes back to the battery, but do i need a BMS which is enabled for regen. braking?
My second question is that 260US$ price point, do you think it's too good to be true? I found the battery on Alibaba, judging the conversation i had, they seem to be trustworthy. I really appreciate all the advice and knowledge from the more experienced builders here!
Thanks
```

---
## \#2 Posted by: telnoi Posted at: 2017-10-26T13:18:04.141Z Reads: 232

```
Some BMS will cause issues/reason why most go with Bestech. Searching the forum, you will come across several threads highlighting issues with BMS and regenerative braking. Those who have issues typically only use the BMS for charging, not for discharge.

That said..that pack capable of 75A discharge. If you are running dual VESC or similar, it would be somewhat of a shame to get a BMS that is rated lower.
```

---
## \#3 Posted by: goldrabe Posted at: 2017-10-26T13:26:20.151Z Reads: 225

```
Thanks for your reply,
i have searched and found the threads you are pointing to but was not able to find an ansswer to my question. For the maximum of 60A, my motors max is 20A and i run double hubs so combined 40A, my assumption was that 60A will be enough.
```

---
## \#4 Posted by: telnoi Posted at: 2017-10-26T13:31:26.771Z Reads: 205

```
In that case, yes..the BMS will deliver enough. 
My motor max is 70 for example, so it's a whole different story.

I personally have a cheap ass li-ion pack with crappy bms and it so far supported -12A regen. You might get lucky...though I would ask the seller what BMS is integrated.
```

---
## \#5 Posted by: goldrabe Posted at: 2017-10-26T13:43:03.221Z Reads: 191

```
Thanks again,
the seller didn't had a clue about regen. braking, she asked me to explain what it is. They use a chinese BMS the brand name is CNWPOWER, i looked on their homepage but it's just in Chinese.
But i assume that the BMS is somehow limiting the amount of energy going back into the battery right? If i am lucky the limit might be high enough for decent braking. Is that correct?
```

---
## \#6 Posted by: Colson003 Posted at: 2017-10-26T13:53:24.985Z Reads: 179

```
Could we get a link to the battery?
```

---
## \#7 Posted by: goldrabe Posted at: 2017-10-26T14:01:22.281Z Reads: 178

```
It's just a generic photo of a shrink wrapped battery which says 10S5P 15Ah e-bike battery. They can build it to the shape of your liking.
They can offer different kind of cells for their packs i also asked for Sanyo 20700B and Samsung 35E the Sanyo was too expensive the 35E is 17.5 Ah at the same price. 
So, there is not much information to gain from the link.
```

---
## \#8 Posted by: telnoi Posted at: 2017-10-26T14:04:41.171Z Reads: 168

```
Yes, or it will blow up/overheat...which sometimes happens.
Does not look like you will get an answer from the reseller.

If it fails or you get VESC fault codes, you can bypass the BMS for discharging. That should also take care of regenerative braking. At worst, you will be looking at a BMS replacement of around 90 USD (from memory)...or it will simply work.

Three options basically.
```

---
## \#9 Posted by: goldrabe Posted at: 2017-10-26T14:09:06.693Z Reads: 149

```
In this case because of the lack of limitations?
```

---
## \#10 Posted by: telnoi Posted at: 2017-10-26T14:11:31.379Z Reads: 145

```
What I have noticed is that most of these packs are delivered with a 2A charger, thus for the BMS to work they essentially only have to include one with a very low rating. For ESK8, we use much higher settings. I imagine the rest will be turned into heat.
```

---
## \#11 Posted by: goldrabe Posted at: 2017-10-26T14:19:05.655Z Reads: 141

```
My pack will be delivered with a 3A charger. But is that related to the amount of regen braking you will get?
```

---
## \#12 Posted by: telnoi Posted at: 2017-10-26T14:24:49.536Z Reads: 140

```
Not necessarily, but since we know nothing about the BMS used your guess is as good as mine/ours.
Normally depending on the brand and type number, you will find specifications/amp ratings for charging and discharging.

Your best option is to post the link to the pack and hope for feedback from someone who has the exact same pack in use. Also include the name of the pack in the topic title and ask for feedback on that pack specifically.
```

---
## \#13 Posted by: FredSaberhagen Posted at: 2017-10-26T14:43:59.709Z Reads: 130

```
The issue with regen is current going back into your load shows up as a higher voltage (current times resistance)

Therefore having your bms in series  (discharge) will also add some resistance and you'll see a higher voltage at the VESC for a given amount of regen current.

A 5p pack should take lots of regen current ... no idea what happens to your bms if there's a higher voltage or reverse current.  For 250 bucks I say just try it!
```

---
## \#14 Posted by: Jinra Posted at: 2017-10-26T15:04:24.657Z Reads: 120

```
$260 it's an amazing deal for 50 cells :scream:
```

---
## \#15 Posted by: Fatos Posted at: 2017-10-26T15:24:15.810Z Reads: 125

```
First of all. That price is crazy. Where did you get the cells dhgate?  Are they genuine?

Best BMS for regenerative breaking are those wich have same port for charge and discharge. That way they will be able to stop charging I'm case a cell is getting overcharged. 
Connectting the batteries directly to motors, is something lots of people here do. But I'm guessing they like to live dangerously. :slight_smile:. If my board takes on fire in a public place, I'd rather be telling to police that I have a bms on my pack.
Not talking about the other advantages by using a quality BMS. Like protection against short circuit, overdischarge , overcharge, balancing control , temperature control.
```

---
## \#16 Posted by: Acido Posted at: 2017-10-26T18:48:08.286Z Reads: 116

```
Im soon starting a battery shop
my services are about 20$ so its like nothing and you are ensured with legit batteries and not some generic Chinese shit that will blow up anytime
```

---
## \#17 Posted by: Fiori Posted at: 2017-10-26T19:37:11.571Z Reads: 109

```
I would be slightly weary about that price to be honest. Unless they are HUGE factory buying in heavy bulk, I don't know how they can get the price that low. That's AT LEAST $200 worth of cells alone...
```

---
## \#18 Posted by: goldrabe Posted at: 2017-10-26T21:56:23.532Z Reads: 107

```
Yes they are a huge factory and because i contacting them via Alibaba they think i am a wholesaler who wants a sample unit. But somehow it sounds to good to be true.
Doing the deal with PayPal and checking the battery for safety and genuineness might be the way to go.
But if i have to buy another BMS for 90 bucks then the deal isn't that good. This way i can start dying my battery in the first place.
```

---
## \#19 Posted by: willpark16 Posted at: 2017-10-27T07:16:27.494Z Reads: 94

```
I'd say don't do it that's less than the parts required to make the pack unless the cells are fake or the bms is crap
```

---
## \#20 Posted by: goldrabe Posted at: 2017-11-03T00:17:03.614Z Reads: 74

```
O.K. i got the seller to send me the BMS spec sheet. It would be really helpful if a person with more knowledge then i have could tell me if this BMS is good in general and allows for regen. braking!
I really appreciate every ones help so far!
Thank you very much.

<img src="/uploads/db1493/original/3X/0/9/09bf2b0728215b12d3b7df39eb5e43cd3f523f54.jpg" width="353" height="500"><img src="/uploads/db1493/original/3X/0/6/0635bbf5ba6fc2dab9ff6222badf84c7a82f5b11.jpg" width="353" height="500"><img src="/uploads/db1493/original/3X/f/d/fd470ae7ebc1e6ff046cd5073bccf8ae0a217267.jpg" width="552" height="499">
```

---
