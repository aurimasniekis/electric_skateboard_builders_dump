# First build &#124; turnigy 245kv 63mm motor &#124; 8s setup &#124; turnigy accucel 8 charger &#124; lipos 4sx2 6000mah &#124; torqueboards esc &#124; caliber trucks &#124; 83mm wheels &#124; torque board motor mounts and gear and pully

### Replies: 47 Views: 1887

## \#1 Posted by: s00cl0se Posted at: 2017-08-31T09:28:44.937Z Reads: 267

```
Good day to everyone. I have started my 8s build , will soon receive my mechanical parts . hopefully next month will place the order for the electrical parts from hobbyking , however I need help from the awesome people in this community. 

I live in UAE , will be glad to meet someone who live here ,and  shares the same interests as e board is something totally new here. 

finally the problems I  am having. hobby king can ship 3s 8000mah batteries but cannot ship 4s batteries. I dont know why . could be due to warehouse or w/e . also the turnigy 8s charger is out of stock since a month or so. I need your suggestion if I should lower my specs to 6s 8000mah(3sx2 8000mah) or wait for 4s to be available in EU warehouse and the charger and order it then . or 6s should be plenty enough? my area is almost flat. 

the second question is that if you recommend that i go for the 6s setup. should i switch over to esc from x car beast 150A . or stick to the vesc as torque boards states that they wont cover drv issues unless i pay 60$ for warranty (doesnt include shipping so basically 100$ if DRV issue occurs)

Also should i get 6374 192kv sk3 motor or stick to 245kv. 

I would be glad for the suggestions you provide and suggestions in changing my setup or anything will be greatly appreciated. 

thankyou
```

---
## \#2 Posted by: pat.speed Posted at: 2017-08-31T10:08:18.126Z Reads: 243

```
If you do switch to 6s I recommend the X-car Beast, I have the 120A and have been running it without issues for the last few months. Just make sure you get the programming card too. I would also stick with the 245kv motor unless you go with a 10s or 12s battery
```

---
## \#3 Posted by: s00cl0se Posted at: 2017-08-31T10:10:26.219Z Reads: 231

```
thanks for the reply, i was reading the article on choosing the battery and the guy suggested that taking 3s batteries and running them i series for 12s is recommended . what do you think. then with 12s i think i will have to move to 6374 192kv motor , or is this overkill.
```

---
## \#4 Posted by: pat.speed Posted at: 2017-08-31T10:13:40.019Z Reads: 219

```
Well it depends on how fast you want to go and how big the hills in your area are. The larger battery will get you better top speed and more range but will mean you will most likely need a BMS, Vesc and 170 - 190kv motor, Which will make the price a lot higher.
```

---
## \#5 Posted by: s00cl0se Posted at: 2017-08-31T10:19:04.092Z Reads: 212

```
i understand, i am looking for range , and i live in total flat area, also i dont mind giving the board a push for the start. someone said that 8s 245kv is the best in terms of cost and torque and speed. but 8s , i cant find the charger or ship the batteries. if you say that 245kv at 6s is strong enough for my needs , i am 150lb and flat roads. i am willing to go 6s with x car esc and save a lot of money, might even do two 6s in parallel for the awesome 16000mah. 

I really appreciate you helping me out btw. thanks a lot
```

---
## \#6 Posted by: pat.speed Posted at: 2017-08-31T10:24:44.274Z Reads: 203

```
No problem man I am happy to help. Well I would think with that 6s and 245kv would be perfectly fine with your weight. The extra packs in parallel would be great. I run 5s (one cell died was 6s) and the batteries are only 5000 mah and I wish I could ride for longer. For my next build I am looking at changeable packs so when one is flat I can put another in. Can anyone just confirm that this would work fine maybe @lowGuido? Since you seem to be the 6s expert.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-08-31T10:34:03.100Z Reads: 189

```
just go with 6S.  chargers are cheap and easy to get. xcar beast is bullet proof, and with 280kv you can easilly hit 32km/h every day.
if you want range wire a couple of 8000mah packs in parallel for 40km range.
```

---
## \#8 Posted by: s00cl0se Posted at: 2017-08-31T10:38:00.555Z Reads: 184

```
lowguido is the reason i am building my e board :) . this guy is awesome . anyways i did the calculation . take it with grain of salt . a zippy 8ah 30c has continuous 240amp so it wont sag much. please correct me if i am wrong.  also it says that 6s 8ah will give roughly about 9miles , so 18 miles with 6s2p is awesome , just thinking how to integrate it with my setup. anyway will be glad to have @lowGuido , give his professional opinion. probably will buy like 2 imax charger and charge each 6s pack separately as i want to avoid parallel charging and save time.
```

---
## \#9 Posted by: lowGuido Posted at: 2017-08-31T10:40:09.126Z Reads: 174

```
I get around 22km with my 8000mah im not sure what that is in miles. about 13miles?
```

---
## \#10 Posted by: lowGuido Posted at: 2017-08-31T10:42:48.991Z Reads: 165

```
I swear I have about 5 imax B6 chargers at home and 2 at work. they are so cheap and you can never have too many LOL.
it certainly speeds things up having a few.
```

---
## \#11 Posted by: s00cl0se Posted at: 2017-08-31T10:45:30.690Z Reads: 150

```
thats awesome. 22km on 8ah makes me not even do 6s2p . just 6s1p will be enough then i guess. I will follow your youtube guide. if there is anything that i should be aware of let me know thanks a lot once again.
```

---
## \#12 Posted by: s00cl0se Posted at: 2017-08-31T10:49:13.721Z Reads: 145

```
Also i might get the hobby king mount and see how they perform on 63mm motor , maybe weld it to the caliber trucks even . will update on how they perform hopefully by end of september.
```

---
## \#13 Posted by: s00cl0se Posted at: 2017-08-31T10:55:09.070Z Reads: 148

```
@lowGuido  one more question. turnigy has a vesc for 85$ on hobbyking site , can you do a video on that. looks like a steal price. costs almost the same as the esc+programming card
```

---
## \#14 Posted by: lowGuido Posted at: 2017-08-31T11:16:53.605Z Reads: 154

```
I just got some torqueboards 218mm trucks and im gonna order some short belts and see how they go with the HK mounts..  

to be honest I probably wouldnt trust a hobby king VESC.. they are fragile enough from reputable sources.
but If i ever get some spare time, and a spare $85 to throw at it I'll give it a crack.

he thing is that I have used VESC from ollin and enertion and they are great but for 6S the Xcar really is unbeatable for reliabillity. and a VESC isnt required. I really dont see the need to go much higher than 6S either... I have built 6S boards that run up to 40km/h plus and climb hills. I have also built 12S boards that are totally overkill (for me anyway) so I'm not like some 6S only fanatic.. 

I just think for most circumstances (what I do anyway) 6S is enough.
```

---
## \#15 Posted by: s00cl0se Posted at: 2017-08-31T11:22:20.463Z Reads: 144

```
awesome , cant thank you enough .
```

---
## \#16 Posted by: s00cl0se Posted at: 2017-08-31T11:23:05.457Z Reads: 138

```
and looking forward for the hk mount  video , hopefully soon
```

---
## \#17 Posted by: bartroosen12 Posted at: 2017-08-31T12:07:07.502Z Reads: 138

```
Wow 6S 8Ah and around 22km that's so much!
I got 6S 10Ah and only getting around 14km and I don't have hills :open_mouth:
```

---
## \#18 Posted by: lowGuido Posted at: 2017-08-31T12:46:24.852Z Reads: 133

```
could be that I am using a 280kv and you are using a 236kv? or a different gearing ratio? or just some difference in ESC efficiency?
there are any number of variables,
```

---
## \#19 Posted by: bartroosen12 Posted at: 2017-08-31T13:35:33.673Z Reads: 135

```
Yeah maybe, I should be so happy if mine should do like 20km :grin: both builds are geared to 40km/h but yeah I got the FVT esc and maybe you got a very smooth running gear and I guess better wheels so wow really I'm impressed :wink:
And yep I'm running the 236Kv
```

---
## \#20 Posted by: stellaren Posted at: 2017-08-31T17:40:54.448Z Reads: 136

```
what do you prefer? fvt or x-car beast 120A?
```

---
## \#21 Posted by: itsmikeholland Posted at: 2017-08-31T17:44:58.239Z Reads: 123

```
unless you plan on riding straight line smooth surfaces, id 100% go with the lowest kv you can afford. i got the 149kv turnigy sk3 and have no idea where people got the idea that its remotely slow. higher kv will almost always run hotter, which is essentially energy that is not making it to your wheels. theyre inefficient and the higher theoretical top speed is nowhere near worth the inefficiency and lower torque.

should mention that im also 150lbs, though I ride a combination of steep hills and some amazing smooth flat surfaces. id always go with higher efficiency, especially if youre in the UAE where its hot as balls. last thing you need are parts that waste off the energy from your battery as heat.

im running 10s4p 360wh battery with a chaka vesc, 83mm wheels (soon to be 76mm), 16/32 gearing, and a 149kv 6374. im in the mindset of prioritizing torque and efficiency
```

---
## \#22 Posted by: lowGuido Posted at: 2017-08-31T18:51:51.964Z Reads: 129

```
I prefer the xcar 150A. I have never used the 120A. I just stick with the 150A because I like that extra bit of headroom. 

@itsmikeholland we are discussing 6S systems so 260kv or upwards in order to get a nice top speed.
if you have a 10S system then of course you can get speed out of a slower 149kv but thats not what we are discussing here.
volts x KV = RPM
10S x 149kv = 1490rpm
6S x 260kv = 1560rpm

so they work out around the same ball park RPM in the end.

then there is gearing.. thats another can of worms.

the whole "higher voltage is always more efficient" thing is a bit of missinformation thats spreads across this forum a lot too. it's a theory that relies on you pulling the same watts to compare the two which can be true, but can also be false. it all depends.. there are so many variables.
```

---
## \#23 Posted by: stellaren Posted at: 2017-08-31T18:56:54.654Z Reads: 115

```
well, when i have all the money to buy everything I'll make  apost to seek your advide hehe. thanks
```

---
## \#24 Posted by: itsmikeholland Posted at: 2017-08-31T19:23:33.256Z Reads: 119

```
i meant to say that lower kv/higher torque is more efficient, didnt mean to imply higher voltage. sorry for the confusion! 6s with 149kv would still be more efficient than 6s at 245kv, while he will have a higher top speed its still gonna burn a lot of heat getting there. on perfectly smooth ground Ive hit 26mph at about 70% throttle when my theoretical top speed is only around 23mph, and my average cruising speed is around 12mph with a total average speed usually around 8mph. in my case it makes sense to get smaller wheels and such because i have essentially 10-15 mph of headroom thats not being used and im lose efficiency. guess it all depends on how he will be using it.
```

---
## \#25 Posted by: s00cl0se Posted at: 2017-08-31T23:49:25.949Z Reads: 116

```
so i dont understand why do people tell me that 190kv requires a full 10s or 12s to work perfectly at its max, while 245 will be too hot at 10s hence use 6s with higher kv. also everywhere i calculate the 245kv has higher top speed.

please correct me if i am wrong

edit: read lowguido's post and thats why i am leaning towards 245kv . i am sure that 245kv at 12s will burn me with it lol

edit 2: so should i go for 6374 @ 192kv ? i think its a bigger motor than 6364 245kv . again correct me if i am wrong. please convince me to not buy 245kv , thanks
i already have ordered 83mm wheels so cant go down there.
we are talking 6s here , thanks
```

---
## \#26 Posted by: s00cl0se Posted at: 2017-09-01T00:14:02.336Z Reads: 103

```
@lowGuido  
a few questions , if it doesnt matter , will be glad to know your preference : 
Q1: xt-90 or xt-60 adapters.? 
Q2: antispark xt-90 (5$)or normal one similar to one in your video?
```

---
## \#27 Posted by: itsmikeholland Posted at: 2017-09-01T00:16:52.536Z Reads: 102

```
this all boils down to how you will be using your board. I use my to commute around west La and Santa Monica and hardly get it above 18mph when I have the road to myself and usually cruising at 12mph on average. Therefore even with 6s I would still go for the 190. Theoretical 16 mph top speed using calc.esk8.it though I personally have been able to exceed the top speed it predicted for me because Im pretty light and my board is small. It would be wasteful to put together a 28mph board and only ever be riding it at 12mph. 

If you just want to go fast in an empty parking lot on your days off then by all means go for 245kv. 

Another thing I want to point out is that right now we're having a heat wave and its 90 degrees outsise which is making even my 149kv motor get hot quicker and Im losing significantly more energy than my rides usually consume.
```

---
## \#28 Posted by: s00cl0se Posted at: 2017-09-01T00:21:58.992Z Reads: 101

```
I am running 83mm wheels, so will 280kv be enough to push it , and i have a 42inch longboard with caliber trucks.
```

---
## \#29 Posted by: s00cl0se Posted at: 2017-09-01T00:33:35.184Z Reads: 115

```
hmm i understand, tbh i live in university campus and the nearest market is like 6km. i am looking for speed as my area is not closely packed and basically roads are empty most of the time i will link a picture , and hopefully you can deduce what might be the best option for me. i really prioritize distance and speed as i am on roads dedicated to cars, 
link:https://www.google.ae/url?sa=i&rct=j&q=&esrc=s&source=images&cd=&ved=0ahUKEwi90c-E3oLWAhWDLVAKHZqZASgQjBwIBA&url=http%3A%2F%2Fcollections.uiowa.edu%2Fweb-images%2FinternationalPrograms%2Fofsa%2F356%2Fprogram%2Funiversity.jpg&psig=AFQjCNFaKUf78qF5tdB4-KTQrebgoTvGHg&ust=1504312245006829

the picture shows the end of a long stretch of road and that building in the picture  is the beginning of another university .


edit : holy friking sht , 90 degrees and ur motor overheating , what will happen to 245kv lol  its on avg above 100 here lol. @lowGuido please can you reasses if i should still stick to 245kv and get +5-10 kph or go down to 192kv
```

---
## \#30 Posted by: itsmikeholland Posted at: 2017-09-01T00:45:41.955Z Reads: 115

```
that road looks amazing! I personally would still go for 190kv, but maybe thats just because with where I live I dont get to take it very fast. I also have a VERY tiny board that saves me a lot of weight which is how Im able to go faster than normal with a lower kv motor ;) <img src="/uploads/db1493/original/3X/4/6/464a43c206e397cce6935db6d0d368dcb20eb155.jpg" width="375" height="500"> I think youll be happy with either way, its not like picking one over the other will be a fatal mistake or anything. another thing to consider is that if you want to upgrade in the future to 10s or 12s with a VESC you may run into problems with the 245kv motor and will also be in the situation Im in where my board is not set up perfectly for how I use it. I personally can get closer with smaller/lighter wheels, a lighter carbon fiber board, and eventually less cells in my battery because the board is so lightweight and efficient for how I use it. Definitely consider everybody elses input as well though, they have a lot of valuable info and experience to consider as well.
```

---
## \#31 Posted by: s00cl0se Posted at: 2017-09-01T00:49:05.059Z Reads: 108

```
i might as well make a good income when i sell it and just build a complete new 12s dual 150kv setup , which very unlikely i wont as a good toyota yaris 2008-2009 cost me 3200$ in mint condition and petrol cost like 50cent a litre , so a dual motor board cost around 1500$? XD

edit: all that heat thing u made me wanna think twice lol . well i will have a story to tell about 245kv in an oven.
```

---
## \#32 Posted by: itsmikeholland Posted at: 2017-09-01T00:55:03.337Z Reads: 99

```
dual 149kv is my dream! Ive been toying with the idea of a dual diagonal build but Id have to get another @chaka vesc, there are some pretty steep hills I still cant get up here in LA. let me try to find a screenshot of the intersection of La Cienega and Sunset Blvd. If i can get up that hill, I can basically conquer all of LA :smile:
```

---
## \#33 Posted by: pat.speed Posted at: 2017-09-01T05:46:13.342Z Reads: 95

```
Personally I think 6s and 245kv will more than please. I also would not think that it will get hot as long as you use appropriate gearing. With 83mm wheels it won't require as much torque and should stay relitivly cool. I see many people running 270kv motors and they are fine
```

---
## \#34 Posted by: lowGuido Posted at: 2017-09-01T06:16:04.846Z Reads: 95

```
I use 280kv all day every day. It works fine and doesnt get hot. I use a 12 tooth pinion and a 30t wheel pulley.  If you choose to go for a lower kv you might be able to upgrade to bigger batteries later or something.. personally i have built more 6S 280kv boards than I can poke a stick at. None of thwm have any problems being hot or slow.
XT60 is fine for 6S you dont need anti spark because 6S spark is small enough to deal with.
```

---
## \#35 Posted by: s00cl0se Posted at: 2017-09-01T07:17:59.929Z Reads: 97

```
thanks a lot for the input @lowGuido .  imade  my decision to go for 245kv , just waiting for 20 sept gonna order everything at once. found a similar to torqueboards mini remote for 20$ on bangood.com . really awesome price. and i dont have a drill press so found a gear tooth pulley and belt for 83mm wheel for 20$ on ebay , exactly similar to torqueboards. with 15mm belt btw . and still looking for caliber mounted motor mounts , probably will make my own and weld it the blow torch way. if i fail i will order one from protoboards (cheaper shipping so save money) . almost 60$ but what can i do :( . wait i forgot that i was gonna order the 8$ motor mount from HK lolz
```

---
## \#36 Posted by: lowGuido Posted at: 2017-09-01T08:02:47.222Z Reads: 94

```
What trucks you using? A word of warning about blow torch brazing .  I found it would crack after a while. And the excessive heat required to braze would weaken the truck. Either find someone who can TIG ir MIG it for you.
```

---
## \#37 Posted by: s00cl0se Posted at: 2017-09-01T12:08:19.887Z Reads: 90

```
oh , its caliber 2 trucks. hmm i have to think of a strong motor mount without breaking the bank. beacuse i was gonna weld hk mounts to make them super strong.
```

---
## \#38 Posted by: pat.speed Posted at: 2017-09-01T21:58:31.932Z Reads: 90

```
Can you send a link of the pulleys I think they could be by a dodgy seller
```

---
## \#39 Posted by: s00cl0se Posted at: 2017-09-01T23:30:07.411Z Reads: 92

```
hmmm dodgy seller , ohh ebay moneyback guarantee yay , alibaba sells it way cheaper btw i just realized . its sold by like 20 different sellers so i will just go for the one with the highest rating .
edit: http://www.ebay.com/itm/DIY-Electric-Skateboard-Parts-Pulleys-and-Belt-For-83-90-97MM-Wheels-Kit-Tool-/292197534013?hash=item440854893d:g:zvkAAOSwsVNZev3O
```

---
## \#40 Posted by: pat.speed Posted at: 2017-09-02T00:11:48.690Z Reads: 83

```
Oh that's not the same kit I was thinking of. Just be aware that there is a kit on eBay that is dodgy. That one seems fine and I might even look at buying it for my next build
```

---
## \#41 Posted by: s00cl0se Posted at: 2017-09-02T00:17:43.439Z Reads: 76

```
can u link it please , or even a picture
thanks
```

---
## \#42 Posted by: pat.speed Posted at: 2017-09-02T00:35:09.354Z Reads: 83

```
Here, many people have brought this and said it is terrible quality

http://m.ebay.com.au/itm/DIY-Electric-Skateboard-ABEC-Flywheel-Pulley-Kit-15mm-Wide-Belts-/182618936000?hash=item2a84efd2c0%3Ag%3AjxsAAOSwjvJZP6e6&_trkparms=pageci%253A6f949229-8f76-11e7-bb68-74dbd180f307%257Cparentrq%253A40025b4c15e0abc10c5caeb8fffd19e2%257Ciid%253A3
```

---
## \#43 Posted by: s00cl0se Posted at: 2017-09-02T10:09:39.801Z Reads: 83

```
Yeah u r right , these are fake 12t 9m pulley
```

---
## \#44 Posted by: FinnishSnowmobiler Posted at: 2017-09-02T13:24:52.794Z Reads: 83

```
X-car beast makes a horrible screeching noise when braking...
```

---
## \#45 Posted by: lowGuido Posted at: 2017-09-03T00:04:15.602Z Reads: 82

```
Yeah. It does. But you get over it.
And it lets dumb pedestrians know you are coming.
```

---
## \#46 Posted by: Cobber Posted at: 2017-09-03T01:20:53.261Z Reads: 81

```
Cool :sunglasses: 

Built in horn :tada:
```

---
## \#47 Posted by: s00cl0se Posted at: 2017-09-17T00:00:54.476Z Reads: 67

```
today i got my 42 inch deck, it feels really big tbh. should i make it smaller 3-4 inches? or thats too small?
```

---
