# 12S4P Battery Pack With PCB

### Replies: 82 Views: 1343

## \#1 Posted by: SanderG Posted at: 2019-04-26T17:19:01.051Z Reads: 247

```
So im starting to build my battery pack, gonna use Samsung 30Q cells (48 of them). I'm making this post to get some more info/tips of other people who have build some. I already got my parallel packs glued with hot glue, but maybe need to reinforce it more? More glue or silicone maybe?

Also gonna wrap the positive side with fishpaper and then glue the PCB on (Hot glue or silicone?)

![IMG_3432|375x500](upload://b6ofK2UwR3r5J5awR1Aqrh6w5wV.jpeg) ![IMG_3433|375x500](upload://2PREd6fcinWHzL0WK3TYVzuBbyp.jpeg) ![IMG_3434|375x500](upload://lcw1T9nSEUnUy0CcZPYKFuRj4cd.jpeg) ![43EF994A-EDAC-4EBF-94F1-95037C6E01C0|230x500](upload://fP2ocO94SrE5ON3JUJv6O2UsXMc.jpeg) 

And for my 12S layout i was thinking this would be the best for my deck. Whit tape is copper flex wire and the + and - terminal are on the right. (placement for the pack will be more to the front, unity and BMS will be in the back.

![IMG_3425|690x238](upload://icifUmBoTikAjSXQEgMEo2wxrku.jpeg) ![59|690x266](upload://uJ163Xv8pSjHn34jbMjdBeAQ6jE.png) 

So if anyone have some pics/info would help allot! Wanna make sure the pack will be good build.
```

---
## \#2 Posted by: Arzamenable Posted at: 2019-04-26T17:25:54.320Z Reads: 231

```
Hot glue works and is in many packs. Don’t use a ton, it sucks to pull it off if you need to. 

Silicone glue has the benefit of not exposing cells to heat and will also not melt if back gets too hot. It ultimately has better wear properties. 

A patient purists would pick silicone. I plan to use hot glue.
```

---
## \#3 Posted by: SanderG Posted at: 2019-04-26T17:50:00.606Z Reads: 227

```
Should i use silicone to glue the PCB to the cells? To maybe get the benefit of both?
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-04-26T17:55:57.764Z Reads: 227

```
silicon is actually sometimes too flexible for stiff packs
```

---
## \#5 Posted by: Arzamenable Posted at: 2019-04-26T17:58:38.152Z Reads: 227

```
If you are going to go the cost and time of using pcbs, continue this attention to detail and use a non acidic cure silicone. 

I forget that preferred type, but it won’t have acetic acid in it. I’ve read can corrode circuitry.
```

---
## \#6 Posted by: Fiori Posted at: 2019-04-26T18:05:02.936Z Reads: 216

```
I like your plan, looks very clean. I would recommend extra insulation in between cells. specifically on the positive end of the cells here:

![123456|375x500](upload://xQRb9O6XHjUAsC2uR23NjkbIqrG.jpeg)
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-04-26T18:06:04.214Z Reads: 206

```
it does not matter there, it only matters between every p group, if the negative shorts in parallel nothing will happen
```

---
## \#8 Posted by: Fiori Posted at: 2019-04-26T18:06:37.748Z Reads: 200

```
It does matter. It can short on the can of the cell next to it.
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-04-26T18:07:01.217Z Reads: 200

```
yeah and it wont matter cause the negatives are connected anyways :grinning:
```

---
## \#10 Posted by: Fiori Posted at: 2019-04-26T18:07:26.502Z Reads: 196

```
Wrong.....

10
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-04-26T18:07:38.014Z Reads: 187

```
it only matters when a negative from another p group shorts with the p group next to it
```

---
## \#12 Posted by: Fiori Posted at: 2019-04-26T18:07:53.816Z Reads: 184

```
False information.
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-04-26T18:08:15.717Z Reads: 186

```
[quote="Fiori, post:10, topic:91834"]
Wrong…
[/quote]

not. if a negative touches another negative in the same p group nothing will happen if the cells are connected in paralell

if you think about it, the bottem terminal is techinically the whole can
```

---
## \#14 Posted by: Fiori Posted at: 2019-04-26T18:09:21.801Z Reads: 179

```
Dude. It shorts that individual cell. I know for a fact. I have burnt cells to prove it.
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-04-26T18:09:57.132Z Reads: 181

```
it wont short thats the thing cause the bottem terminal is the can and your connecting it in paralell :rofl:
```

---
## \#16 Posted by: Andy87 Posted at: 2019-04-26T18:10:26.280Z Reads: 185

```
You always want to build a flexy pack. Even if it’s a stiff deck. Some kind of flex as min between the p groups is more than healthy.
```

---
## \#17 Posted by: Fiori Posted at: 2019-04-26T18:10:55.068Z Reads: 188

```
You clearly don't get it. Keep giving dangerous advice though, hopefully you feel good about it.
```

---
## \#18 Posted by: AlanZhou Posted at: 2019-04-26T18:12:11.723Z Reads: 187

```
Eh?

![IMG_20190426_141150|666x500](upload://vG6K8XRrczH2ZZdtzjIUfvey5mi.jpeg)

and now i have to rewrap two cells
```

---
## \#19 Posted by: Arzamenable Posted at: 2019-04-26T18:12:32.819Z Reads: 182

```
@AlanZhou, in his defense, on the positive end, you could have part of the adjacent negative can slide out and get crushed into the positive top, but If youre pack has shifted this much, you board has had a real bad day.
```

---
## \#20 Posted by: AlanZhou Posted at: 2019-04-26T18:13:11.453Z Reads: 183

```
fair enough, but hes thinking that if the can touches in paralell the battery will short but in fact it wont as shown by my demonstration
```

---
## \#21 Posted by: AlanZhou Posted at: 2019-04-26T18:14:46.606Z Reads: 180

```
[quote="Fiori, post:17, topic:91834, full:true"]
You clearly don’t get it. Keep giving dangerous advice though, hopefully you feel good about it.
[/quote]

maybe read up about cells a little more, the advice that I was giving was not wrong, as you can see in the photo the positive and negatives are touching between cells without issue, cause that's how cells in parallel work :sweat_smile:
```

---
## \#22 Posted by: Fiori Posted at: 2019-04-26T18:15:33.962Z Reads: 175

```
Read up on cells? LOL. I'm done replying to you.
```

---
## \#23 Posted by: AlanZhou Posted at: 2019-04-26T18:15:45.882Z Reads: 171

```
didn't you see the photo?

the cell only shorts if one cell slides up closing the circuit
```

---
## \#24 Posted by: Andy87 Posted at: 2019-04-26T18:16:31.463Z Reads: 176

```
@SanderG which do you have a picture of the pcbs you will use? There are some designs which have a copper field in the middle as well. If that’s the one you use than take care that no of the nickel or wires you use is hanging over the copper fields on the end. Hard to explain, hope you got it non the less.
```

---
## \#25 Posted by: Fiori Posted at: 2019-04-26T18:17:21.031Z Reads: 173

```
I don't need your photo. You still don't understand, which is a re-occurring thing around here with you apparently. .
```

---
## \#26 Posted by: Arzamenable Posted at: 2019-04-26T18:17:33.469Z Reads: 175

```
For the OP, anything is possible. Focus efforts on avoiding the common badness. 

Fishpaper around p groups is a solid choice. Insulated spacing between each cell in a p group is maybe a lot. I’m sure someone will post a pic of a short caused by this situation. But if you are using pcbs too, this shouldnt ever happen.

@Fiori, I’m totally open to your concern. Hit us with details if you experienced a short that extra insulation would have prevented.
```

---
## \#27 Posted by: AlanZhou Posted at: 2019-04-26T18:17:46.601Z Reads: 177

```
The cells would short if it touches side by side like this 

![IMG_20190426_141711|666x500](upload://zSkpc1295D3nLbe8oeVS67i25Fb.jpeg)

if the cells are connected in paralell as indicated by blue it wont matter if the can touches

![proven1|666x500](upload://5hOVmcdYyYDkfOefZoa0rJhL0QA.jpeg)

the second cell if touched not on level will act as a bridge causing a short, indicated by yellow and red

![proven2|666x500](upload://gaj0bz2QBSImu0EGbNR1FVhTqvy.jpeg)
```

---
## \#28 Posted by: AlanZhou Posted at: 2019-04-26T18:18:15.760Z Reads: 168

```
so am i supposed to wrap every cell in a extra layer of fish paper? (not saying its bad) also you said i was wrong 
:expressionless:

its a reoccurring thing that people dont take in information
```

---
## \#29 Posted by: SanderG Posted at: 2019-04-26T18:23:45.899Z Reads: 165

```
Yea the flex of mine is gonna be the flex copper wire between the serie connection, so each P group can flex (but will not need flex tho)
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-04-26T18:24:47.166Z Reads: 168

```
hmm really never knew, i dont like flexy packs for some reason idk, but still trying to figure out the layout for my 13s10p
```

---
## \#31 Posted by: neiru37 Posted at: 2019-04-26T18:26:21.102Z Reads: 167

```
[quote="Fiori, post:8, topic:91834"]
It can short on the can of the cell next to it.
[/quote]

I'm going to have to agree with Alan here. Shorting negative terminals within p groups doesn't really matter. Shorting a positive terminal with any negative terminal within the p group or within the cell itself does. And if we're talking about 2 p groups next to each other then yeah the negative terminals between those shouldn't touch too.
```

---
## \#32 Posted by: Fiori Posted at: 2019-04-26T18:26:21.772Z Reads: 158

```
It would take a slight shift to cause that to short. I prefer to insulate it because its the safe thing to do. I care about safety, maybe you don't. Iv'e seen it happen. 

You really want to rely on your pack staying perfectly level for safety? I don't.
```

---
## \#33 Posted by: SanderG Posted at: 2019-04-26T18:26:30.512Z Reads: 152

```
Yea i have a copper field in the middle, i can wrap each middel in fishpaper, thanks for the tip!!
```

---
## \#34 Posted by: AlanZhou Posted at: 2019-04-26T18:26:55.451Z Reads: 155

```
[quote="Fiori, post:32, topic:91834, full:true"]
It would take a slight shift to cause that to short. I prefer to insulate it because its the safe thing to do. I care about safety, maybe you don’t.

You really want to rely on your pack staying perfectly level for safety? I don’t.
[/quote]

hmm i thought you didn't understand, but i know a little shift can cause a short thats why i explained it.

but i was a little aggravated when you blatantly said my information was wrong :sweat_smile:
```

---
## \#35 Posted by: Fiori Posted at: 2019-04-26T18:27:58.496Z Reads: 156

```
Because it was wrong. It can short. It's still wrong...
```

---
## \#36 Posted by: AlanZhou Posted at: 2019-04-26T18:28:22.524Z Reads: 162

```
![proven1|666x500](upload://5hOVmcdYyYDkfOefZoa0rJhL0QA.jpeg) 

@Fiori do you see my cells shorting?
```

---
## \#37 Posted by: Fiori Posted at: 2019-04-26T18:28:33.714Z Reads: 160

```
You're like a brick wall.
```

---
## \#38 Posted by: AlanZhou Posted at: 2019-04-26T18:28:42.587Z Reads: 161

```
hehe :rofl:
```

---
## \#39 Posted by: Andy87 Posted at: 2019-04-26T18:29:56.114Z Reads: 158

```
There is always a little flex on every pack. That can kill your welds over time. You don’t need a crazy flex pack but to make the series connections with silicon wire instead of welded nickel is not a bad idea.
```

---
## \#40 Posted by: Andy87 Posted at: 2019-04-26T18:30:22.632Z Reads: 156

```
Thats pretty good 👌
```

---
## \#41 Posted by: AlanZhou Posted at: 2019-04-26T18:30:40.195Z Reads: 154

```
[quote="Andy87, post:39, topic:91834"]
You don’t need a crazy flex pack but to make the series connections with silicon wire instead of welded nickel is not a bad idea.
[/quote]

i would do that but then i can only mount my battery on one side

i would also like to do cell fusing if there is a easy solution for double stack
```

---
## \#42 Posted by: Andy87 Posted at: 2019-04-26T18:33:08.223Z Reads: 147

```
It shouldn’t be an issue as the middle copper field is usually covered, but who knows, vibration and stuff can damage that. Just make sure no nickel or something else is hanging over and you good. No need than for extra cover in the middle
```

---
## \#43 Posted by: lazarus Posted at: 2019-04-26T20:13:30.126Z Reads: 141

```
PCB sandwich with cells on both sides? That was my plan, with a printed bridge over copper bus to prevent any contact between PCB and cells on top.
```

---
## \#44 Posted by: AlanZhou Posted at: 2019-04-26T20:15:31.091Z Reads: 141

```
or normal fuse wire but make sure they dont touch each other? inslate the first layer fuses with fish paper and then do the second layer of fuses on top of the fishpaper? for the second layer of cells 

sorry for bad explanation
```

---
## \#45 Posted by: Jumpman Posted at: 2019-04-26T20:20:53.986Z Reads: 139

```
Sorry for bringing it back, but if the top outer ring of the cell really was positive, then there wouldn’t be any danger of shorting with nickel strips.  Pretty sure it’s negative.
```

---
## \#46 Posted by: AlanZhou Posted at: 2019-04-26T20:24:31.688Z Reads: 137

```
[quote="Jumpman, post:45, topic:91834"]
Pretty sure it’s negative.
[/quote]

the top outter ring is negative
```

---
## \#47 Posted by: Jumpman Posted at: 2019-04-26T20:41:36.565Z Reads: 127

```
Thanks.  I wasn’t really sure what was causing a short in your example with the slipped cells, so I guessed you were saying the top outer ring was positive.

I agree with your suggestion of fishpaper between parallel groups.
```

---
## \#48 Posted by: AlanZhou Posted at: 2019-04-26T20:42:29.483Z Reads: 127

```
yeah since the top ring touches and the can touches it basically makes the cells turn into one (parallel)
```

---
## \#49 Posted by: Schtekarsten Posted at: 2019-04-26T20:48:35.610Z Reads: 133

```
alkohol dissolves hotsnot.
works like magic! 
Pretty sure it weakens the heat shrink of the batteries though but hey... :crazy_face:
```

---
## \#50 Posted by: RedBaron Posted at: 2019-04-26T23:20:55.806Z Reads: 134

```
You can let those cells touch because only this part of the battery is positive. (See picture)
![20190426_161922|500x500](upload://pWK8lRl2EZIDmngrewnf5IjAosF.jpeg)
```

---
## \#51 Posted by: AlanZhou Posted at: 2019-04-26T23:22:14.613Z Reads: 133

```
yes i know, that was my point to him, if the negative casing touches nothing happens
```

---
## \#52 Posted by: RedBaron Posted at: 2019-04-26T23:23:22.705Z Reads: 134

```
I mean they can still touch like this picture and not short.
![proven2|666x500](upload://gaj0bz2QBSImu0EGbNR1FVhTqvy.jpeg)
```

---
## \#53 Posted by: AlanZhou Posted at: 2019-04-26T23:23:38.304Z Reads: 128

```
oops didnt know what my brain was on
```

---
## \#54 Posted by: mishrasubhransu Posted at: 2019-04-26T23:51:11.026Z Reads: 127

```
@Fiori, sorry, dude. You are wrong here. Alan discharges his batteries till 2.5V(sorry Alan :P) and thinks it's all right, but as far as safety of cells in parallel groups touching each other is concerned. It's safe.
```

---
## \#55 Posted by: AlanZhou Posted at: 2019-04-26T23:55:33.198Z Reads: 124

```
[quote="mishrasubhransu, post:54, topic:91834"]
Alan discharges his batteries till 2.5V(sorry Alan :P)
[/quote]

errrkrkkrkrkrkrkk
```

---
## \#56 Posted by: KaramQ Posted at: 2019-04-27T00:30:04.239Z Reads: 123

```
Ahhh, I can’t stand you no more man, your literally going to end up like me if you keep messing around
```

---
## \#57 Posted by: Fiori Posted at: 2019-04-27T01:03:25.673Z Reads: 126

```
I always thought that if you connected these parts like this, that it would short the individual cell:

![oops|500x500](upload://qIZCVgkhgfRBhBzYiNm1nT1rzMG.jpeg) 

But after going into my garage and trying it with some wire, it turns out I am wrong. 

We're all wrong sometimes, I'll admit it,  today it was me. ![surp|640x360](upload://mfflQlaomxtwNSyroL1fRYJvFBz.jpeg) 

That being said, I obviously know the negative cans can safely touch each other, that was never my point. I always feared this happening(but apparently it's not a concern): ![proven2|666x500](upload://gaj0bz2QBSImu0EGbNR1FVhTqvy.jpeg)
```

---
## \#58 Posted by: ducktaperules Posted at: 2019-04-27T01:17:43.703Z Reads: 126

```
I wwas about to rage about your stubbornness but then got to this post.

[quote="Fiori, post:57, topic:91834"]
it turns out I am wrong.

We’re all wrong sometimes, I’ll admit it, today it was me.
[/quote]

Im impressed, its not often we see that here :slight_smile: 

Anyway, for those that are interested about how the cell is constructed there is an awesome picture of one cut in half.

https://i2.wp.com/www.electricbike.com/wp-content/uploads/2017/07/Battery18650D.png?fit=715%2C681&ssl=1

Hope this provides some clarity about whats connected to what.
```

---
## \#59 Posted by: AlanZhou Posted at: 2019-04-27T01:26:30.817Z Reads: 123

```
i call fake news :rofl: you can cut a cell in half.

jkjk

I feel lied too, so a 18650 is just a cell with more cells in it? :face_with_raised_eyebrow::thinking:
```

---
## \#60 Posted by: Sners Posted at: 2019-04-27T01:34:19.184Z Reads: 135

```
like paper rolled into a straw

![IMG_4480|690x248](upload://dvfymhkC58T7gtL302etB9Cv8t5.jpeg) ![IMG_4481|653x396](upload://iScJmXUiM1rm4WmX0cnJLh0Kjcf.jpeg)
```

---
## \#61 Posted by: ducktaperules Posted at: 2019-04-27T01:38:31.854Z Reads: 136

```
it is one cell, but more surface area is better so they just make i big flat cell and roll it up
http://cdn.shopify.com/s/files/1/0674/3651/files/opening-cells.jpg?3554169202426396855

phone batteries are the same just folded flat rather than rolled
http://batteryuniversity.com/_img/content/pack5(1).jpg


intresting cell tear down here: (good stuff at round 24:30)

https://youtu.be/gYFuVbZmu5M?t=1478
```

---
## \#62 Posted by: Fiori Posted at: 2019-04-27T01:39:58.124Z Reads: 134

```
I am stubborn :stuck_out_tongue:

But at the end of the day, people getting the correct information is what I care about most.
```

---
## \#63 Posted by: SanderG Posted at: 2019-04-27T11:01:30.919Z Reads: 130

```
Okay so no fishpaper is needed in between the cell, just ring on the top of each positive end is okay.
And gonna wrap each parallel pack with fishpaper and then glue the PCB on top like this.

![image|624x499](upload://w1S7nkpnd49cKgYzT7I4nUc8VjO.jpeg)
```

---
## \#64 Posted by: AlanZhou Posted at: 2019-04-27T14:16:00.038Z Reads: 124

```
what size of fish paper is that? I can never find it (not talking about the positive terminal ring)
```

---
## \#65 Posted by: SanderG Posted at: 2019-04-27T14:20:32.496Z Reads: 125

```
Its just a roll of 63mm wide, 0.2mm thick fishpaper on a roll cut down to size.

![42|690x285](upload://u5zatPNs4poIlz6Wneh4hUwEhcK.png)
```

---
## \#66 Posted by: AlanZhou Posted at: 2019-04-27T14:22:00.451Z Reads: 125

```
also why did you not spot weld on the cutouts? but instead spot weld on the nickle beside it? those cutouts are meant to increase strength

![spot%20welded|624x499](upload://6VfsILzlIJrVLbG3scebJquQ52L.jpeg)
```

---
## \#67 Posted by: SanderG Posted at: 2019-04-27T23:10:40.194Z Reads: 122

```
That is just a pic i found on another post, i will do it different. I will use normal nickel strips from each battery to the PCB.
```

---
## \#68 Posted by: SanderG Posted at: 2019-04-28T13:23:53.305Z Reads: 110

```
Anyone here has some inspiration pictures of packs build with PCB's? :)
```

---
## \#69 Posted by: M.Hboards Posted at: 2019-04-28T13:29:47.437Z Reads: 111

```
[quote="SanderG, post:68, topic:91834"]
Anyone here has some inspiration pictures of packs build with PCB’s? :slight_smile:
[/quote]
Yup hope this helps-
![0329191311|690x328](upload://1TSje9r0JFjziS4kpbwFWcYhWyF.jpeg) ![0329191229a|690x328](upload://f1HeJkCMpe704mWjCbyX26UFVPA.jpeg) ![0329191316|690x328](upload://38pgKViPHBWPXTeHcMcKOQHRdU7.jpeg) ![0331192234|690x328](upload://enyQzc0DLpqn5MLei8tjvd4ch2A.jpeg) ![0329191315|690x328](upload://7NBNUi9RmxXEHYBMEj7l16HYshG.jpeg) ![0331192215a|690x328](upload://fpARmDJ9Q3ce9zFyToiDfVClwpR.jpeg) ![0331191701|690x328](upload://9jDIwaB9nJ4Ah6MvdAXzkVL3i4N.jpeg) ![0401191900|690x328](upload://7ITyUojZDYBljNBAf5428m5Phrb.jpeg) ![0329191610|690x328](upload://6gQUdCSTDMrf31VRpN3u6rj84lD.jpeg) ![0331191655|690x328](upload://mk3eLPX8Lh8gXrM0xcEXqra2ghG.jpeg) ![0329191616|690x328](upload://9YMplYp9YZBUf4YavIE3AlNxfiV.jpeg) ![0331191756|690x328](upload://qvboOctBr2gb6LW6m1kqNYUge1W.jpeg) ![0401191901a|690x328](upload://hHqaGyXyaveKrp3kQgEejYI1t6q.jpeg) ![0329191610b|690x328](upload://qnvlZ32jKiU3PLIlAxbQdNxcjH.jpeg) ![0331191704|690x328](upload://i3NKoHNjVXNloTzk0hkMEaLdE3W.jpeg) ![0401191901|690x328](upload://4WAnbVv8dinOmZmjdvAmXPevXSF.jpeg)
```

---
## \#70 Posted by: SanderG Posted at: 2019-04-28T13:32:41.228Z Reads: 103

```
Did you put fishpaper between the PCB and battery or did you just silicone it on? looks really good!
```

---
## \#71 Posted by: M.Hboards Posted at: 2019-04-28T13:33:30.559Z Reads: 100

```
I siliconed it on.
```

---
## \#72 Posted by: SanderG Posted at: 2019-04-28T13:35:07.083Z Reads: 96

```
Cool! You also soldered the nickel strips on the pcb? why not spot welds only? To weak?
```

---
## \#73 Posted by: M.Hboards Posted at: 2019-04-28T13:40:33.376Z Reads: 100

```
 The tack to the pcb is strong however the layer of copper on the pcb is very thin so a slight pull on the nickle will pull up the copper on the pcb.
```

---
## \#74 Posted by: SanderG Posted at: 2019-04-28T13:41:53.822Z Reads: 104

```
Oh thats bad, and will it handle the current if its that thin?
```

---
## \#75 Posted by: M.Hboards Posted at: 2019-04-28T13:48:34.904Z Reads: 102

```
I believe it could handle the current as many other people do rely solely on the pcb . I solder as well for the piece of mined that my nickle isn't comeing off the pcb  but don't quote me on the pcb able to handle the current by itself as i haven't tested it myself.
```

---
## \#76 Posted by: SanderG Posted at: 2019-04-28T13:52:03.026Z Reads: 100

```
Another question, Is fishpaper needed between the PCB and batt? or has this no use?
```

---
## \#77 Posted by: M.Hboards Posted at: 2019-04-28T14:01:42.955Z Reads: 101

```
I don't believe fishpaper between the pcb and batt would serve a purpose as the PCB is not conductive.
```

---
## \#78 Posted by: SanderG Posted at: 2019-04-28T17:41:29.621Z Reads: 105

```
Glued the PCB on the cells with silicone :) now we wait!

![IMG_3457|690x318](upload://cx5trhl5K9wMdjwkHDLdKEQqqvl.jpeg) ![IMG_3458|230x500](upload://aW4n64A2HW86r8ajvdn031ntRlO.jpeg) 
![IMG_3455|375x500](upload://gpewrdEfJDTdAxRtkgPX9H6f7LC.jpeg)
```

---
## \#79 Posted by: SanderG Posted at: 2019-05-05T10:53:44.138Z Reads: 95

```
Do you guys glue the pack to the deck? Or how do you keep it in place?
```

---
## \#80 Posted by: legend27 Posted at: 2019-05-05T11:23:50.006Z Reads: 95

```
After my battery has been shrink wrapped I use dual lock. Best stuff ever. it's not moving anywhere. I recommend mounting it to your deck depending on what enclosure you got.

https://www.aliexpress.com/item/3M-brand-tape-SJ3550-dual-lock-self-adhesive-fastener-3M-tape-250-type-mushroom-black-15/1000001467327.html?spm=a2g0s.9042311.0.0.27424c4dQEYeUr
```

---
## \#81 Posted by: SanderG Posted at: 2019-05-05T13:09:49.039Z Reads: 94

```
Starting to look good ;) first wrapped the connections with capton tape and then wrapped it up a bit with the reinforcement tape.

Should i do fishpaper first and then the PVC heatshrink? Or first heatshrink then fishpaper? (Im gonna wrap each pack with heatshrink and also heatshrink the total 12s4p)

![image|375x500](upload://fIgxE2fEL2IrkLxa9oHevlkMNBs.jpeg) ![image|666x500](upload://pPtQz2szNSdjrYfhQlDxuQ5Al0V.jpeg) ![image|666x500](upload://xwtP9AQJgAayGCxvXXnqHGVWa3f.jpeg) ![image|666x500](upload://x0UP2TvKYX6X9Nokd8cCgRMYZjV.jpeg)
```

---
## \#82 Posted by: SanderG Posted at: 2019-07-02T19:30:04.360Z Reads: 60

```
So i need some help, already got the pack done, only need to connect the balance leads and series connection. The pcb is gonna go face down to the deck so the pack can flex a bit. But what would be a good way to connect the balance leads (i do not wanna cover up the pcbs with allot of fishpaper). Would i be safe to put the ballance leads in a bundle in the middle? Vibrations can rub the leads together and short them? Any recommendations?

![image|374x500](upload://tZnh4u4gVAt32V7hCfFvx0VtMHj.jpeg) 
![image|374x500](upload://seuKtBDhzINtW3iJBeVWt4Ikdqq.jpeg) ![image|281x500](upload://iHJHPxoWhfxH1dpzssgj4fGZROL.jpeg) ![image|375x500](upload://8FKERzabrtScwFEEwW7SAdDn5G5.jpeg) ![image|375x500](upload://p9EFLVNOLzVKB0PQky1nH7wFnjN.jpeg)
```

---
