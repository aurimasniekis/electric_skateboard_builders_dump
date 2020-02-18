# NEW BATCH 6-12s open source DieBieMS

### Replies: 42 Views: 4075

## \#1 Posted by: fedestanco Posted at: 2018-04-14T13:35:12.424Z Reads: 545

```
As you might know last year I decided to make a first, beta production of this open source project: https://github.com/DieBieEngineering/DieBieMS designed by the forum member @JTAG 
It definitely took a while since any imaginable delay occurred and piled up (even the first national strike of the logistic company UPS :persevere:). 
Now that some users had the chance to try this BMS on their board, the response has been pretty good so far and no major problems have been reported.
The setup is dead easy via usb and vesc tool: simple commands on the terminal will allow you to set up your custom battery configuration and will let you know the detailed status of your battery
![image|516x500](upload://tdjYNhT6HLQtDWdVk5nVYpbv9Jv.png)

And you can avoid wasting money on antispark switches and voltage meters
![IMG_20171213_222225|375x500](upload://pLIPWeOVRcBwRr9BectdjwOC4GJ.jpg)![IMG_2067|375x500](upload://q3fYObd7Ts324yV15AWIPJy7Kr1.png)

I am looking into doing some changes on non critical components for example putting XT90 instead of LOAD screwholders, finding a cheaper sound buzzer, removing unnecessary connectors.
This way I can keep the price steady (last time was 104eur) and include compensation for the creator and myself.

**The quantity I am willing to reach is at least 30 pcs. If you are interested, please sign up here  https://goo.gl/forms/W4weN1iovSiYuST23**

![24331746_107633256692475_1204786687859752960_n|667x500](upload://6hqZSYzfde4s1yNlVQ7Jwu4Q8g1.jpg)

Pics stolen from @longhairedboy @chinzw @lock
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-04-14T13:59:54.146Z Reads: 486

```
For Those of us that are not fimiliar with this bms, What is the max discharge it can handle, or is it bypassed?
```

---
## \#3 Posted by: Pantologist Posted at: 2018-04-14T14:04:08.512Z Reads: 473

```
http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/26?u=pantologist
```

---
## \#4 Posted by: deucesdown Posted at: 2018-04-14T17:27:36.983Z Reads: 434

```
I've been drooling at these forever. form filled out. Thanks for doing this!
```

---
## \#5 Posted by: uigiroux Posted at: 2018-04-14T17:31:50.604Z Reads: 425

```
Order placed, can't wait I've been wanting one of these since I first saw the thread!  How much would be saved going with XT-90 instead of LOAD screwholders?  I was hoping to have that feature...  Any way to make that optional...?
```

---
## \#6 Posted by: moon Posted at: 2018-04-14T17:32:02.283Z Reads: 415

```
Anyone have the dimensions. I think is saw it earlier when I browsed the other thread, is it 15mm thick?

Sorry didnt mean to reply to you :smile:
```

---
## \#7 Posted by: Minim Posted at: 2018-04-14T17:32:19.016Z Reads: 398

```
What is ETA on this? I’m interested for my build but I want to complete it before the summer comes by :)
```

---
## \#8 Posted by: fedestanco Posted at: 2018-04-14T17:55:00.745Z Reads: 391

```
@uigiroux not much since the screwholder were already very efficient (175 max load by datasheet or 120a by mouser). The reason I want to eliminate them is that they are damn expensive and non-existing in China. 

@moon 140 x 60 mm

@Minim once the minimum quantity is reached, let's say end of April. Give around 5-6 weeks for production, 1 week to ship stuff to me, 1 week for me to have all orders out (since this time I wont have to install firmware and extra components)
```

---
## \#9 Posted by: Brad Posted at: 2018-04-14T18:24:03.211Z Reads: 360

```
Do you mean you will solder wires onto the load terminals where the LOAD screw holders were and solder the other end onto an XT90?

I'm having trouble imaging you directly putting an XT90 plug straight onto the BMS PCB...
```

---
## \#10 Posted by: fedestanco Posted at: 2018-04-14T18:39:36.176Z Reads: 340

```
Nope that would be a mess.
I will change the screwholders footprints to become solder pads for wires.
Then the 10awg coming from the xt90 will be soldered on these pads.
```

---
## \#11 Posted by: Brad Posted at: 2018-04-14T18:52:39.053Z Reads: 322

```
Yes that is what I imagined, just different wording describing the same thing.
```

---
## \#12 Posted by: CamBo Posted at: 2018-04-15T02:33:06.424Z Reads: 306

```
Hey @fedestanco, how difficult is the program interface for this? And is there a manual we can check out?  

It looks awesome, I am just worried running it will be over my head.
```

---
## \#13 Posted by: ervinelin Posted at: 2018-04-15T02:40:52.808Z Reads: 293

```
Form filled up!!!
```

---
## \#14 Posted by: uigiroux Posted at: 2018-04-15T02:56:55.814Z Reads: 296

```
About how much do you estimate these will cost with the changes made to reduce the price?
```

---
## \#15 Posted by: fedestanco Posted at: 2018-04-15T11:40:44.915Z Reads: 307

```
The only steps you will have to follow are these ones:

1)you need a specific version of the vesc tool that I am going to send you via email
2)connect the vesc via usb while it’s still connected to the battery pack
3)go to the connection tab; if you can find a “usb serial” device, connect to it. If you don’t find any available device then you need to install these drivers https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers and try again
4)once you are connected, go to the terminal tab; type `help` and enter; this lines will show up:

![image|516x500](upload://tdjYNhT6HLQtDWdVk5nVYpbv9Jv.png)

As you can see you can type (for example) `config_set_ah 20` and enter. The bms will now consider your battery as a 20ah battery. The other commands work in the same way.
After you are done with the customizations type `config_write` and enter.
That's it

@uigiroux the goal would be for the price to be <=104eur including the donation, cables and VAT.
Tomorrow I will get a quotation for a custom fuse-holder which is a feature I really want to keep
![fuse-holder|604x500](upload://cs3NnJJyGNm6iUxNrb4Ss2R9meY.jpg)
```

---
## \#16 Posted by: ervinelin Posted at: 2018-04-15T11:47:21.833Z Reads: 283

```
This looks like a dream come true. A few quick wuestions.

Will orders outside the EU be VAT free? 

What's the expected delivery date should we hit 30 orders.

Lastly, I put my name down for 2 but I think I only need 1. Can you correct that on your end?
```

---
## \#17 Posted by: fedestanco Posted at: 2018-04-15T12:04:16.298Z Reads: 281

```
[quote="ervinelin, post:16, topic:52240"]
Will orders outside the EU be VAT free?
[/quote]
Yes. 

[quote="ervinelin, post:16, topic:52240"]
What’s the expected delivery date should we hit 30 orders.
[/quote]

[quote="fedestanco, post:8, topic:52240"]
Give around 5-6 weeks for production, 1 week to ship stuff to me, 1 week for me to have all orders out (since this time I wont have to install firmware and extra components)
[/quote]

PM me your email so I can remove your form and you can compile a second one.
```

---
## \#18 Posted by: riva_00 Posted at: 2018-04-15T12:42:01.906Z Reads: 253

```
Form filled, Thanks for your hard work @fedestanco & @JTAG
```

---
## \#19 Posted by: Prism Posted at: 2018-04-15T20:32:14.114Z Reads: 253

```
What a convenient timing! Signed up for one.
I'm starting with my own project soon, been browsing this forum a lot to get ideas and inspiration. This BMS caught my attention and I always wanted to use one for my battery pack.
Thanks for doing this group buy!
```

---
## \#20 Posted by: Deckoz Posted at: 2018-04-15T21:15:57.142Z Reads: 253

```
Just submitted.

How many away are you?  And what is the turn around time once completed? I am also outside of EU and want to make sure VAT is excluded in the price?

@fedestanco

Also keep us updated as to how close we get..I will be willing to change my quantity as I'm sure others might if we get close to the quantity needed...
```

---
## \#21 Posted by: fedestanco Posted at: 2018-04-15T21:30:47.470Z Reads: 228

```
I have just checked and we definitely passed the 30 units goal :sparkler:

I was hoping for some more time to make some changes to the pcb though, so I can't really gather payments untill the new design is ready.

Unfortunately only registered companies are legally allowed do the "VAT discount" trick so I fear that you will have to pay full price; I will get more informed on the topic though.
```

---
## \#22 Posted by: Deckoz Posted at: 2018-04-15T21:36:21.199Z Reads: 221

```
Nice...well. That's good news on the quantity. 

As far as VAT...I'm not sure if your close to @Kug3lis  (Not trying to sign you up for anything) but maybe he might be interested in getting some for his store/exporting for a small fee... Just an idea.... If you two are close enough to one another .. 

Otherwise ~$128 USD isn't that terrible.
```

---
## \#23 Posted by: uigiroux Posted at: 2018-04-15T21:39:02.398Z Reads: 231

```
Wait even in the US we'd have to pay the VAT?

![Screenshot_20180415-163809|690x368](upload://tuxBuavZVnnDbwjfVkdt5XBumCg.jpg)
```

---
## \#24 Posted by: fedestanco Posted at: 2018-04-15T21:40:24.671Z Reads: 228

```
It is included in the price. No last second surprises.

@Deckoz kug3lis is in Croatia and I am pretty sure he doen't want to work for free; generally speaking the best way to save on the price is to do group shipping since I can ship about 30 bms' with UPS tracked for 20eur to the US.

EDIT: kug3lis shop is in Lithuania.
```

---
## \#25 Posted by: uigiroux Posted at: 2018-04-15T21:48:55.598Z Reads: 219

```
104€ = $128
I don't mind spending that much for this I think it's definitely worth it, but I thought the changes that were being made were to make it cost less?  So then regardless of where we live well be paying the VAT tax?  I don't understand that?  It was just said earlier that if we're not in the EU we wouldn't have to pay that tax..?  What changed in the last hour or so?
```

---
## \#26 Posted by: Lobap Posted at: 2018-04-15T21:59:22.036Z Reads: 211

```
Form submitted!  Thanks!
```

---
## \#27 Posted by: fedestanco Posted at: 2018-04-15T22:08:06.804Z Reads: 213

```
First of all 104 is the abs max. I am working hard to make it sub 100 without compromizing donations and quality.

This is a brief explaination of VAT: 
VAT is a tax meant to pay for some of the nice services that are free in Europe that are not available in other countries.If you don't live here it's undertandable that you don't want to pay it because you don't use such services.

The actual refund of VAT is where things get nasty: if I were a registered company (and I am not) I would have to pay the VAT in advance for you, send the proof of export to my government, and then get back the money from my government. 

If the fact that I am not able to get the tax refunded bothers you, it makes prefect sense so you you are free to leave this GB, buy all the stuff from mouser and make your own board and you will be sure that Italy's government gets 0%.
```

---
## \#28 Posted by: Minim Posted at: 2018-04-15T22:10:36.302Z Reads: 199

```
Great. Signed up for one :slight_smile:
```

---
## \#29 Posted by: uigiroux Posted at: 2018-04-15T22:11:43.466Z Reads: 216

```
No no I'm didn't mean it in any offensive way, I sorry if it came off that way I just wanted to know what the reason was.  I'm very much looking forward to this and have been for some time so definitely have no problem paying that.  Like I said, I just wanted to know what changed and the reason, that's all.  Thank you for your reply and for making this all come together, I'm very excited to get this BMS!
```

---
## \#30 Posted by: Kug3lis Posted at: 2018-04-15T22:52:10.051Z Reads: 211

```
I live in UK, but the shop is operated from Lithuania ;)
```

---
## \#31 Posted by: fedestanco Posted at: 2018-04-15T22:59:01.057Z Reads: 212

```
haha I didn't even get one right...
```

---
## \#32 Posted by: fedestanco Posted at: 2018-04-16T23:25:57.314Z Reads: 212

```
Hi guys,  
today I received the terrible news that I took a barely sufficient grade in one of my engineering exams.
I am committed to spend any spare minute of the upcoming months to study the subject and try the exam again in June.

I am therefore forced to put this GB on pause unless someone trusted and experienced on here wants to step up.
I deeply apologize for the time you spent filling up the form and I am expecially sorry if your partecipation was business related.

Federico
```

---
## \#33 Posted by: akhlut Posted at: 2018-04-16T23:27:00.170Z Reads: 202

```
School is more important.
```

---
## \#34 Posted by: moon Posted at: 2018-04-16T23:37:59.615Z Reads: 210

```
Hope you do better in the next exam :sunny:

And maybe there is someone out there capable of this kind of GB
```

---
## \#35 Posted by: Pimousse Posted at: 2018-04-17T07:24:07.387Z Reads: 204

```
I wish you all the best to succeed !
@akhlut is definitely right ! School is the #1 priority.
```

---
## \#36 Posted by: linsus Posted at: 2018-04-17T07:49:44.185Z Reads: 208

```
But you passed? you just want a higher grade?
My proffessor used to tell me I studied "bit too much again" when i was one or two points over passing :rofl:
```

---
## \#37 Posted by: banjaxxed Posted at: 2018-04-17T11:24:05.124Z Reads: 208

```
Shelve it man, lessen distractions
```

---
## \#38 Posted by: Eboostin Posted at: 2018-05-31T04:58:11.079Z Reads: 212

```
Is school out yet? Time to make some more BMS? 

Hope the exams went well for you @fedestanco!
```

---
## \#39 Posted by: fedestanco Posted at: 2018-06-02T14:59:11.172Z Reads: 211

```
Hi guys,
the exams will end 27th of july, but there is good news if you want to get one bms:
this guy is willing to sell a few and the quality looks very good.

https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/279?u=fedestanco

If you planned to get on this GB I would suggest to go with him instead PAYING WITH PAYPAL SERVICES to be safe.
```

---
## \#40 Posted by: Prism Posted at: 2018-08-09T19:51:11.951Z Reads: 199

```
Hey @fedestanco, hope your exams went well.
Just to clear thing up, will you continue this group buy? 

[quote="fedestanco, post:32, topic:52240"]
I am therefore forced to put this GB on pause unless someone trusted and experienced on here wants to step up
[/quote]

because you said you pause it, not cancel it. 
I just wanna know if I have to look for a different bms or can still count on this one.
```

---
## \#41 Posted by: moon Posted at: 2018-08-09T20:06:52.646Z Reads: 200

```
I think @Samau18 was running one?
```

---
## \#42 Posted by: oyta Posted at: 2018-08-10T12:43:32.707Z Reads: 189

```
https://www.electric-skateboard.builders/t/diebiems-v0-8-2nd-batch-total-48pcs-closed/58327?u=oyta

He did two batches I think. Maybe running a third if enough interest.
```

---
