# Project Gozilla &#124; Board Undecided&#124; Carvon Hub Abec11 &#124; Dual VESC&rsquo;s &#124; Torqueboard 12s3p

### Replies: 31 Views: 3501

## \#1 Posted by: broshi Posted at: 2016-04-04T07:36:35.881Z Reads: 274

```
Hi I'm broshi and I'm looking to build my first Eboard. From New York currently live in Tokyo. 

I've been lurking for a bit and while I'm not that knowledgeable in elec/mech engineering I've done some DIY stuff in the past and confident I can get it right with a few mistakes along the way Would love feedback on some of the parts that I have chosen and would be great if I can get some input. 

Mainly building this board as a commuter. Weighing in at 160lbs and 170lbs geared and the steepest hill being <10%.Willing to spend $1200 ~ $1400 should be enough to get me a board that gets 10-15 miles and top speed 20mph right? 

I've already decided on the Carvon dual hub motors with Abec11s as easy setup and stealthy. 
http://bit.ly/1qiO1j0  @$700

So I've got around $700 left to work with. Let's get started

■Batteries/Enclosure
Trying to keep it simple but would be down to build my own. Looking at the new enertion space cell which I can fit my dual VESCs in http://bit.ly/1W4vse6. Don't know much about if this will allow the range/top speed I want. 

**Edit** Going with Torqueboards 12S3P pack http://bit.ly/1RFtIWE

■VESC
Kind of clueless here but sounds like Vedders or enertions look pretty good?

**Edit** Decided with torqueboard VESC since Dexter has helped me so much with the build and I'm buying other parts like the canbus from him.

■Deck
Was thinking of the vanguard since I don't think I'll mind the bounce that much. If I do do this I might design the electronics to imitate the boosted. 

**Edit** throwing the vanguard idea away since the flex is too complicated, looking for non flex or small flex decks. 

■Misc
Any suggestions for controllers and other materials, water proofing etc?

**Edit2**
Went with @MasterCho  gt2b casing mod sold here http://www.ebay.com/itm/252382292682
Thanks for shipping all the way out to Japan! 
Going to buy the gt2b from hobby king.
```

---
## \#2 Posted by: lox897 Posted at: 2016-04-04T08:18:07.682Z Reads: 239

```
I don't think the SPACE Cell will work well with a vanguard, it may be a bit too flexible. Most people have done a split enclosure design where one enclosure has batteries and the other has the esc. The SPACE Cell is a bit too long for this too work.
```

---
## \#3 Posted by: lox897 Posted at: 2016-04-04T08:25:39.476Z Reads: 240

```
Any suggestions for controllers and other materials, water proofing etc?

You have a few options for controllers: 
Enertion 2.4 ghz $100 USD
HobbyKing GT2B Under $30 USD
TorqueBoards 2.4 ghz Mini Remote $50 USD
Nunchuck (Wouldn't recommend this one, it can have drop outs and cause injuries.)

Water Proofing isn't really needed unless you intend to ride in the rain or when it's wet. Some other guys had some good water proofing techniques, they can chime in here.

You may need some loctite, bolts, connectors or other miscellaneous materials.

Also a side question, braking on hub motors will allow the batteries to charge right?
If you have regenerative braking enabled on VESC then yes.

Hope this helps.
```

---
## \#4 Posted by: broshi Posted at: 2016-04-04T08:42:41.332Z Reads: 215

```
hmm true, do you know of any battery compositions that I can make which will allow me to split?
```

---
## \#5 Posted by: lox897 Posted at: 2016-04-04T09:31:37.002Z Reads: 214

```
Most Vanguard builders used lipos and one of them wired it up to a charging port for one plug charging. You could even connect them to a bms. Or you could use a different deck.
```

---
## \#6 Posted by: cmatson Posted at: 2016-04-04T16:27:29.841Z Reads: 199

```
Some people (namely @evoheyax) have run into issues with the Space Cell/Carvon hub motor combo. 

Others, such as @RunPlayBack have had great experiences with the combo- 

I'd maybe look at getting the Pro4 Space Cell, two VESC's (from Enertion because they are only 89$ w/ free shipping), and something like a GT2B or Torqueboard's mini remote.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-04-04T16:42:09.717Z Reads: 211

```
Personally, I would have stayed away from the space cell had I known what I know now.

My problem seems to be I hit the 15 amp per motor limit of the space cell. This seems to for some reason to have broken one of my VESCs. That isn't to say it does work. It worked quite well, until it broke.

However, I would have built my own battery had I had the option of starting over again. 15 amps for the carvons dual is simply not enough fro any thing but flat ground riding. I will be trying 30 amps per motor later this week when I get another pair of VESCs, by slightly modifying the space cell. I still don't think that will be enough though for much hill climbing.

The bottom line, you want more amps getting to those motors, especially since those motors can run up to 80 amps each. With the VESC, 50 amps each motor which means I can run 100 amps total, instead of the 30 amps total I'm running at now. And the only way to do that is by building your own battery pack (either from cells or from smaller batteries in parallel and/or series)
```

---
## \#8 Posted by: willpark16 Posted at: 2016-04-04T16:58:16.718Z Reads: 201

```
Make a 18650 pack and solder the cells, this way you could arrange the cells in a way to fit your vanguard and not worry about deck flex.
```

---
## \#9 Posted by: lox897 Posted at: 2016-04-04T21:22:19.594Z Reads: 190

```
18650s are big in a good configuration. It would almost be the same as the SPACE Cell. You could use 26650s like Boosted.
```

---
## \#10 Posted by: barajabali Posted at: 2016-04-04T21:47:35.537Z Reads: 187

```
dont get the vanguard deck... i have it its just a pain to work around...  Just go with a stiff deck.

you can spend that money somewhere else on the board

And damn. $700 bucks on carvons stuff is pricy. why not do a cheaper satellite motor mount?
```

---
## \#11 Posted by: evoheyax Posted at: 2016-04-04T21:59:26.180Z Reads: 188

```
I think that hub motors are great in the sense that they are plug and play. Satalite motors need to be built and constantly adjusted. You also have belts that break very easily if you don't have them perfectly adjusted and if your not using a wide enough belt on a single drive system, belts will also break easier. There's a lot of headaches created by the belt and pulls system, which is why I think you see such a focus on hub motors lately.

Hub motors have their own headaches though, as I am finding out. Most important, you have no gearing... This is why geared hub motors seem to be the holy grail of eskate propulsion systems. But those likely also have their own problems that have yet to be seen since starry is the only ones making these for their own board.

My point though, is that hub motors are easier for those with no eskate experience to get up and running. However, $700 for Carvons is way too much, I thought $500 was a bit high when I got mine.
```

---
## \#12 Posted by: broshi Posted at: 2016-04-05T01:02:28.470Z Reads: 176

```

@evoheyax

in your dream machine post here: http://bit.ly/1RYuTTi you said

But the results are amazing. I can go 20+ mph up 20% grade hills without issue, have tested to 30 mph on flat ground with plenty of throttle left.

I wanted to ask so if I get a stiffer board and build my own battery pack would I be in the clear?
```

---
## \#13 Posted by: broshi Posted at: 2016-04-05T01:06:56.981Z Reads: 180

```
I'm in Tokyo where the cops in the cities stop people on bikes with headphones. I want it to be as discrete as possible so I thought a hub motor might have been a better choice for me. I definitely understand how $700 on the hub motors is kind of expensive but taking into acount

 - stealth
 - plug and play
 - Just need to get enough amps to it to climb hills
 - Only have hills that are <10% around here

made it an acceptable investment for me
```

---
## \#14 Posted by: AbrownMN Posted at: 2016-04-05T01:28:19.725Z Reads: 175

```
I'm assuming you already have due to how similar our builds are, but if you haven't already you may want to check out my build thread, and look at all of RunPlayBack's build/blog as well for ideas on how to put everything together as he has a lot of pictures of everything going together. These should both be very helpful for you. If you want specific advice on components let me know. I've done hundreds of hours of research at this point :stuck_out_tongue: Thanks to wonderful, helpful people on here I have got everything I need coming very shortly! Jerry at Carvon, and Dexter (@torqueboards) have been extremely helpful for me among many others here. I would highly recommend buying from either of them. I have a controller, 12s battery, cable, and VESC's coming from Dexter still, but I know it's all going to be awesome! Good luck man, let me know if you need anything.
```

---
## \#15 Posted by: barajabali Posted at: 2016-04-05T01:35:23.999Z Reads: 169

```
Well as long as you have justification for it then it's a good idea for your situation
```

---
## \#16 Posted by: evoheyax Posted at: 2016-04-05T01:41:14.270Z Reads: 179

```
So everything I poted is correct except hill grade. I did calculations on a hill myself. I came to 20% grade. Looking the above sea level difference map for that street, it says 7% grade. Which is right idk, I think it's really somewheres in between, maybe really 10%, but I think I did those calculations wrong. My point is that they are ok for climbing hills, especially hills under 10% grade. But with more amps, you should have less issues with hills. And the space cell won't give you those amps.

Since you want stealth, the vesc's and their FOC mode will be a must. And car ones aren't the best hub motor for stealth but a step up from a satalight configuration.
```

---
## \#17 Posted by: broshi Posted at: 2016-04-05T04:20:18.501Z Reads: 171

```
Yeah haha your (@AbrownMN post is what finally made me realize, fuck it I have some christmas cash left over and will just spend it on beer if I don't build something awesome.

That aside, what made you decide on the torqueboards 12S3P battery? A lot of people in my thread are concerned about the amp out put of the space cell and wanted to know why you ended up choosing dexters battery pack.
```

---
## \#18 Posted by: AbrownMN Posted at: 2016-04-05T13:40:48.874Z Reads: 179

```
Good deal! Glad I could give you the push you needed to do this! I literally **just** pulled my Carvon motors out of the delivery packaging, I am so stoked! I chose a 12s pack at the recommendation of Jerry himself from Carvon. He said others had experienced cutoffs on his dual hub motors with the space cell and other 10s packs, and I wanted to make sure I was getting all the power I needed all the time. Like you, I wanted the build to be solid, easy to put together and maintain. His pack is the only 12s3p pack I have seen that is all set up and ready to go. Plus, he is a great guy and has been a wonderful help throughout my build ( as you know if you read my thread) so I wanted to give him all the business I could.
```

---
## \#19 Posted by: LukeM Posted at: 2016-04-12T02:33:49.580Z Reads: 165

```
@broshi I highly do not recommend with going with the same board boosted uses. The Vanguard flex. It does not feel stable at high speeds and cannot make quick turns and is a hassle to carry.
```

---
## \#20 Posted by: broshi Posted at: 2016-04-12T06:07:02.097Z Reads: 171

```
Yeah seems to be so. I'll definitely avoid it. I guess I just test rode the boosted for the first time in Japan the other day and got excited. I don't really skate so I didn't know how a stiff deck would feel.
```

---
## \#21 Posted by: RunPlayBack Posted at: 2016-04-12T16:11:26.857Z Reads: 157

```
As far as stealth goes, the Carvon hubs on FOC is about as quiet as you'll get. I ride my board every day in the city and with some well timed kick pushes, no one has any idea that it's an electric until I throttle it up on a straightaway. The police here aren't as strict but I ride on the sidewalk sometimes and having a quiet board makes it less obnoxious around pedestrians. I actually got a compliment from a super purist middle aged skater yesterday. He said eboards have always been ridiculous to him until I let him ride it and it just clicked for him. Like it was a hybrid of electric and natural skating, most of it due to the feel of the FOC and hub combo.
```

---
## \#22 Posted by: broshi Posted at: 2016-04-13T01:21:40.179Z Reads: 151

```
Man you're getting me even more excited when all my shipments are 3+ weeks out!! 

You're videos also helped me in finally taking the dive to build once since boosted is really hard to get shipped to Japan. 

I might ask a ton of questions since its my first build ever so please help me out when it all comes in!
```

---
## \#23 Posted by: Surfnerd Posted at: 2016-04-26T09:53:32.760Z Reads: 148

```
[quote="RunPlayBack, post:21, topic:2154"]
I ride my board every day in the city and with some well timed kick pushes, no one has any idea that it's an electric until I throttle it up on a straightaway.
[/quote]

what is so diffent that it´s quiet? i don´t get FOC......how is the control system different?
```

---
## \#24 Posted by: RunPlayBack Posted at: 2016-04-26T16:57:32.121Z Reads: 146

```
The setting is more efficient at driving power from the VESC to motor. Instead of BLDC where it's on/off on throttle, it feeds the energy gradually.
```

---
## \#25 Posted by: broshi Posted at: 2016-05-15T13:22:15.770Z Reads: 155

```
<img src="/uploads/db1493/original/2X/0/0a7bf8edc527ad2e9c7453714b2d762a4ba08ca5.jpg" width="666" height="500">


Just got the enclosures from @mastercho theese babies are looking solid. 
First time ordering 3d printed but these things are seriously smooth. 

Can't wait to get all the parts in 2-3 weeks
```

---
## \#26 Posted by: Eboosted Posted at: 2016-12-12T05:32:58.866Z Reads: 95

```
Did ever finish this build?

I'm looking for feedback and comparisons from Carvon hub motors vs a regular belt system, hope your build went well
```

---
## \#27 Posted by: saul Posted at: 2016-12-12T07:47:39.714Z Reads: 90

```
for dual they will be about equal. for a single the hub can only do small hills.
```

---
## \#28 Posted by: broshi Posted at: 2016-12-12T11:51:28.162Z Reads: 88

```
I have all the parts but I blew on of the VESCs out while testing out different settings. 

So I cant comment much on the torque of a dual.
```

---
## \#29 Posted by: Eboosted Posted at: 2016-12-12T14:42:39.838Z Reads: 85

```
Did you know exactly why you blew your VESC? Can you comment on that? What version of VESC was it?
```

---
## \#30 Posted by: broshi Posted at: 2016-12-13T00:01:58.270Z Reads: 82

```
Yeah i put too much amps with no load to see how fast the wheels would spin. Did it for around 5 seconds and it smoked.

I have the DIY electric skateboards VESCS.
Getting a replacement chip for the specific chip I blew now
```

---
## \#31 Posted by: Arzamenable Posted at: 2017-02-25T23:35:16.403Z Reads: 62

```
I'm in Okinawa and haven't had any issues with the Japanese cops. 

I just stuffed an evolve carbon GT into a rifle case and threw it in with gear thats being shipped over to mainland Japan. Do you think they will hastle me near Fuji? I'll be goofing off up there for a month or so.
```

---
