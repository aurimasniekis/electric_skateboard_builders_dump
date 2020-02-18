# FOC for my first time.. VESC 4.12 DRV Error&hellip; FoCMe

### Replies: 33 Views: 2887

## \#1 Posted by: longboardshort Posted at: 2018-03-19T13:27:40.100Z Reads: 340

```

Here are all my settings, I ran FOC for my first time yesterday, and within 2 hours got the infamous 8302 error... I was really enjoying the smooth acceleration too. Running 10S, TB6355 190kV motor, 16/36 gearing.  Any other info that would help?  Please let me know.   Back to BLDC mode I guess.. once I get this vesc fixed.

On another note, does anyone know or offer DRV chip replacments?  I am near DC, prefer in the states, but will ship out if need be.

Cheers
![26 AM|690x347](upload://u1HXMxWRDiMwBLyhLBRw6ZC6j6C.png)![06 AM|690x354](upload://7ClgSDuB6LwXfS4m74ioU63ED5U.png)![16 AM|690x349](upload://wGdHyiprikSMFaLYcUYp6OTYgP0.png)![31 AM|312x500](upload://2zLnzHt2Q5aJaSZSmaSUiTwYcP1.png)![45 AM|690x347](upload://zWbuTrIQMv8dPq0wt3AYVSZ6kuY.png)![00 AM|690x347](upload://s1iwDeMlOqdaXgTBdumJYReYlM4.png)
```

---
## \#2 Posted by: Tuomalar Posted at: 2018-03-19T13:32:49.033Z Reads: 308

```
Running FOC after reading thousands of posts about huge possibily of drv error using FOC with 4.xx vesc is like telling kids not to run in stairs. Despite what you say they do it and and hurt themselves.
```

---
## \#3 Posted by: FredrikHems Posted at: 2018-03-19T14:05:15.424Z Reads: 308

```
What kind of vesc was it? I guess the 4.12 from DIY or maytech..
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-03-19T14:36:08.558Z Reads: 300

```
There should be a general disclaimer to not run FOC on anything but Focboxes and VESC6 and derivatives. MAYBE maytechs. But absolutely not TB’s.
```

---
## \#5 Posted by: Acido Posted at: 2018-03-19T14:38:40.990Z Reads: 297

```
i think that has been said enaugh, even the sellers say that, but not in a way like it will blow up your vesc but in a way that its not the products fault but yours
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-03-19T15:29:17.059Z Reads: 285

```
They should at least take down the tutorial for running FOC.I'ts been shown that their ESC's can't handle it. Why give a keyway?
```

---
## \#7 Posted by: ZackoryCramer Posted at: 2018-03-19T15:33:07.912Z Reads: 274

```
The title is too gold. 😂
@Jc06505n aggreed. Took my TB from that deceptive tutorial.
```

---
## \#8 Posted by: longboardshort Posted at: 2018-03-19T16:37:06.435Z Reads: 261

```
"What kind of vesc was it? I guess the 4.12 from DIY or maytech…"

It was a 4.12 from DIY

I have read of people swearing by only FOC from Vescs other than focbox, but alas I learned the hard way.  I agree about the general disclaimer comment though.

On that note, does anyone recommend anyone/any service to replace the DRV?  I have two replacement chips already ordered, but I don't have the skill for replace it yet.  Thanks in advance.
```

---
## \#9 Posted by: skatardude10 Posted at: 2018-03-19T17:26:55.674Z Reads: 246

```
I'd like to chime in here as an eskate noob. I am in the process of parting together my first build, and I've been doing a ton of reading. I have two focboxes on their way, and I don't want to blow one if I can prevent it, but FOC mode sounds great.

Regarding the warnings, should I be afraid of even trying FOC on my focboxes? I've reads posts of people blowing their DRVs and other issues on them as well, but it seems to happen a lot less than other 4.12 vescs from the number of posts on the subject.

I'd just like to be safe and have a reliable board, but it's difficult to weight those desires with the desire to also have a smooth and quiet board running FOC.
```

---
## \#10 Posted by: TarzanHBK Posted at: 2018-03-19T17:28:20.685Z Reads: 236

```
Shipp them to @JohnnyMeduse - he´s the repair magician ;)
```

---
## \#11 Posted by: TarzanHBK Posted at: 2018-03-19T17:30:21.643Z Reads: 234

```
Focbox, 10s and a motor with max 190kv is a good way to be safe ;)
Something can happen all the time, but that is a good standard recipe to be safe
```

---
## \#12 Posted by: Namasaki Posted at: 2018-03-20T03:27:42.517Z Reads: 228

```
After almost 2 years running BLDC, I was starting to get the itch to try FOC.
After reading this post, the itch is gone.
```

---
## \#13 Posted by: MannyM0E Posted at: 2018-03-20T04:10:39.429Z Reads: 214

```
@ThermalM16 also a good VESC repair. He was good with shipping to, fixed my TB VESC pretty quick. I'm currently using the repaired VESC with no problems.

@Namasaki I know what you mean. I be getting the itch to just to know what the fuss is about with FOC.
```

---
## \#14 Posted by: goldrabe Posted at: 2018-03-20T05:26:47.681Z Reads: 203

```
What iteration of firmware where you running?
I am still tempted to run my Maytech's in foc.
```

---
## \#15 Posted by: pat.speed Posted at: 2018-03-20T05:28:14.969Z Reads: 201

```
No no no no no. Maytech vescs are more unreliable then Tb vescs. Well at least they used to be, maybe tb has gotten worse
```

---
## \#16 Posted by: will_manners Posted at: 2018-03-20T05:30:49.929Z Reads: 199

```
I assumed it was pretty common knowledge that you will run into problems on FOC with almost any of the 4.12 vescs with the acception of Ollin, FOCBOX etc. 

I've been running dual maytech vescs in BLDC and never had any problems.

@JohnnyMeduse is the guy to speak to for DRV replacements.
```

---
## \#17 Posted by: ThermalM16 Posted at: 2018-03-20T05:36:56.774Z Reads: 200

```
@longboardshort depending on where you’re located you can ship to either me or Johnny. I’m located in Florida and he’s in southern Canada I believe. Either way you go, they run about the same price when you factor in you cost to ship it to either of us. I’m not sure if he’s swamped right now or not, but most of my repairs have been completed in a day or two. 

@Namasaki you know you want to try it, just give in :joy:
```

---
## \#18 Posted by: Eboosted Posted at: 2018-03-20T06:14:55.713Z Reads: 196

```
@namasaki why don't you buy a Focbox? It's totally worth it, runing in FOC is like riding a brand new car, no weird sound and satisfying feeling, accelerations from a dead stop at extremely smooth. You won't go back and will focboxes you won't brake anything
```

---
## \#19 Posted by: Namasaki Posted at: 2018-03-20T11:56:52.518Z Reads: 187

```
I already have a lot invested in 4 Ollin Vescs. 
And I don’t mind driving an old car. 
Like my 1999 Toyota 4Runner
```

---
## \#20 Posted by: longboardshort Posted at: 2018-03-20T14:25:34.661Z Reads: 185

```
Sorry if this issue has been brought up a thousand times before.. but what is it than Focboxes have that so vigorously prevents frying of the DRV?

Edit: Also pmed you @ThermalM16
```

---
## \#21 Posted by: gravitycarve Posted at: 2018-03-20T14:37:04.443Z Reads: 181

```
Toyota Master race.

I just bought a 2001 toyota tacoma with 100k

Anyway I can vouch for @JohnnyMeduse he fixed both of mine in a weekend and just had to wait for snail mail.
```

---
## \#22 Posted by: Eboosted Posted at: 2018-03-20T14:45:14.457Z Reads: 173

```
But the ollin VESCs are totally capable of runing FOC, I thought you were runing DIY VESCs. Go ahead and try it
```

---
## \#23 Posted by: Namasaki Posted at: 2018-03-20T15:08:32.971Z Reads: 172

```
No thanks.
```

---
## \#24 Posted by: Tobi Posted at: 2018-03-20T17:31:21.164Z Reads: 171

```
 Dont use that old bldc tool ... 

Steps to go ;

1) download new vesc tool from official website
2) connect vesc with the new tool
3) firmware upgrade the vesc
4) reboot vesc connect again
5) follow foc wizard, then input wizard
6) sucess

no problem so far since 3 monthes i switched from bldc to foc

My hardware vesc 4.12 (germany) 6374 200 kv motor (germany)
```

---
## \#25 Posted by: ThermalM16 Posted at: 2018-03-20T21:44:17.462Z Reads: 160

```
FOC can overheat FETs which can in turn kill the DRV. This isn't always the case, but it seems to be the majority of the time. The FOCBOX uses direct FETs which offer much better cooling options, like pressing them against a large heat sink.
```

---
## \#26 Posted by: longboardshort Posted at: 2018-03-22T19:21:07.222Z Reads: 158

```
Just got a focbox in the mail, and im excited to use it.. but a little apprehensive.  It says not to exceed 30A or -15A for batt max and min.. is this always the case or just for R2 use?  I used 50A on my VESC I believe.  

Also came to find out that switching to 5.5mm bullet connectors does void the warantee... thought I read it didn't somewhere before but I'm glad I asked support before doing anything.
```

---
## \#27 Posted by: jerry373 Posted at: 2018-03-24T23:27:11.608Z Reads: 147

```
Do you know exactly why the new VESC tool is better than the BLDC tool for hw 4.12+FOC?

My configuration is VESC hw 4.12 + SW 2.18, 190kV, 6374, 10S1P LiPo and 15/72 gear ratio (mountainboard with 8" Primo tyres). I get about 20km on a charge in BLDC mode and top speed ~35kmh

Today I tried for the first time to configure FOC and after some weird start-up issues it went OK. the problema started when I tested the board while riding. If I accelerate too fast or brake too hard I get the DRV errors and the VESC resets. The DRV is not dead but I don;t want to risk it and reverted to BLDC which works as before. In between the FOC.BLDC changes I always flash a new FW to be sure I don't mess up the configuration.

To my knowledge the FOCBOX is basically a VESC 4.12
```

---
## \#28 Posted by: Tobi Posted at: 2018-03-25T11:33:34.236Z Reads: 135

```
i dont know it for sure, but its how things work generally ... why would u use win xp, if u can use win 10 ? newer software / firmware always is better than the older one.

vesc 4.12 is also capable of runing foc, i did post my hardware settings, i use it 4 month now without any issuis ... but this will not mean its suitable for ur setup as well ...

u have to try it, nobody can say it for sure, differnent manufactors will make things complicated ... but i would always try newest software / firmware  / update first.
```

---
## \#29 Posted by: jerry373 Posted at: 2018-03-25T12:08:56.645Z Reads: 132

```
Haha..well indeed I agree with you if you know it's better. But I also like the idea of not braking things that already work good enough... I'm going for a ride now..the sun in shining here in NL
```

---
## \#30 Posted by: jerry373 Posted at: 2018-03-25T18:58:28.031Z Reads: 121

```
so today i rode in bldc mode than came home and decided to give @Tobi suggestion a go. I've installed the new VESC tool and plugged in my VESC. It recognized hw 4.10 (I thought I have 4.12)  and it updated the fw to 3.37. Than I configured FOC with no issues. Unfortunately still get the DRV error code when I brake hard... :frowning:

I'm back to bldc and I think I'll stick to that for a while...  I could update the capacitor but I have to read trough the forum if that actually will solve the DRV and FOC. Personally I don't really care...I thought I could make my ride a bit more quieter and get a bit more range but what I now have in bldc mode it's not bad at all :slight_smile:
```

---
## \#31 Posted by: fraannk Posted at: 2018-03-26T10:19:32.676Z Reads: 105

```
While we're at it, I might as well ask here. I'm about to try FOC on my dual FOCBOX'es. It's an 8s setup with 230Kv motors. I'm below the ERPM limit, so that shouldn't be a problem. Anything particular I should take note of? My setup should be compatible, right? :)
```

---
## \#32 Posted by: cypa9904 Posted at: 2018-03-26T10:45:17.325Z Reads: 105

```
Hi. Can sb help me? 
I have a mountainboard 1:5 gearing 10s 2x 192kv motors. Will focbox be a good choise for a board like that? And using FOC mode change the risk of burnout or sth like that? Thanks for answers! :)
```

---
## \#33 Posted by: TarzanHBK Posted at: 2018-03-26T12:11:30.779Z Reads: 100

```
If you have low to medium hills, don´t ride like a maniac and you´re under 100 kg, you should be good.
Make sure to cool them, the more the better!

Foc on 10s is the sweet spot, where the chance of burning out something is the lowest.
If you wanna be 100% sure to not destroy something, just go with BLDC.
```

---
