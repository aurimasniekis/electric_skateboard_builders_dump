# Best VESC settings for li-ion 30Q 12s4p and dual 6374 190kv motors?

### Replies: 20 Views: 1663

## \#1 Posted by: stimm Posted at: 2018-03-30T15:47:52.262Z Reads: 313

```
Hey everyone,

I am about to set up my dual focbox vescs (via cambus).   I have a 12s4p 60amp SuPower ([BMS](http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html)), and dual 6374 190kv motors.  

I want to make sure I set these correctly:

Motor Max, 
Motor min (regen), 
Batt max, 
Batt min (regen), 
Absolute max 

Also if you have suggestions for:

Minimum input voltage
Maximum input voltage
Battery cutoff start
Battery cutoff end

I want to be able to have good braking for going down hills.   I will also use BLDC but might try FOC mode in the future.  

Thanks for any help, I have searched up and down the forums and people seem to be varying their opinions for these settings.  (I have my own opinions but I don't want to influence the decisions.) :wink:

 Thanks everyone!
```

---
## \#2 Posted by: intensivegecko Posted at: 2018-03-30T16:40:30.185Z Reads: 297

```
What cells are you using?
```

---
## \#3 Posted by: Colson003 Posted at: 2018-03-30T16:42:53.867Z Reads: 297

```
Is this your first board? Do you have a Bluetooth module to easily change theses settings? 

Here’s what I’d start out with:
Motor max: 60
Motor min: -60
Battery max: 30
Battery min: -8
Absolute max: leave it alone, I think its 130

Minimum input voltage leave it at 8
Maximum input voltage leave it at 57
Battery cutoff start: 36 (3 volts per cell)
Battery cutoff end: 33.6 (2.8 volts per cell)
```

---
## \#4 Posted by: intensivegecko Posted at: 2018-03-30T16:45:30.005Z Reads: 290

```
So motor max, min, batt max, min, and what else need to be split along two vesc?
What does absolute max do?
```

---
## \#5 Posted by: Colson003 Posted at: 2018-03-30T16:48:05.139Z Reads: 281

```
I gave those settings per VESC. Only battery max and min need to be split. 
Absolute max I believe is just a cutoff point, if you exceed it you’ll get some error like: abs_over_current. All I know is that it should be left alone at 130
```

---
## \#6 Posted by: intensivegecko Posted at: 2018-03-30T16:50:31.245Z Reads: 277

```
Oh I swapped motor and battery in my head. I see that now.
```

---
## \#7 Posted by: stimm Posted at: 2018-03-30T16:53:23.272Z Reads: 270

```
30Q Samsung.
```

---
## \#8 Posted by: stimm Posted at: 2018-03-30T16:56:07.428Z Reads: 264

```
This is my first board, but I am a pool skater and I am used to the speed and have good board control.  I wonder if I should put the battery cut off a bit higher, around 41V or 40V.   I think that might be safer? I had it at 20% when I built the battery and it was around 41V (3.41V per battery).
```

---
## \#9 Posted by: Colson003 Posted at: 2018-03-30T16:58:55.068Z Reads: 257

```
You can set the battery cutoffs as high as you’d like, you’ll lose range while gaining some longevity of the pack.
```

---
## \#10 Posted by: thiswasandy Posted at: 2018-09-13T06:18:36.209Z Reads: 194

```
What settings did you end up going with?
```

---
## \#11 Posted by: Jasonkimberson Posted at: 2018-09-13T18:47:42.213Z Reads: 194

```
I didn’t post this, but this is what I am running on my 12s4p with 6374 170kv motors

It would be interesting if people gave suggestions for me as well

![image|690x361](upload://uOlGlSojdIcfiiH3pnUMEIqwRmk.jpeg)
```

---
## \#12 Posted by: Sebike Posted at: 2018-09-13T19:16:18.702Z Reads: 188

```
edit: sorry. I thought it was 10s

recommend cutoff start arounf 3,2v / s and end around 3,0 / s

Motor max 70
Batt max 30 per vesc if dual, depending on BMS discharge?
Motor min -40
Batt min -10
```

---
## \#13 Posted by: Jasonkimberson Posted at: 2018-09-14T04:30:53.278Z Reads: 172

```
I have a bestech charge only running Samsung 30q in a 12s4p
```

---
## \#14 Posted by: thiswasandy Posted at: 2018-09-18T18:53:41.899Z Reads: 165

```
How’s this working for you?

Wheel size and gear ratio?
```

---
## \#15 Posted by: Jasonkimberson Posted at: 2018-09-18T19:12:26.488Z Reads: 160

```
Well, went on a 24 mile ride and everything was good until one of the motors got jacked.  ![image|666x500](upload://x3bENonGNsEoj5PNturdUlDzr7I.jpeg) 

I went with cheap motors dickyho was selling.  I have since ordered some janux 6374s.  Waiting for those to come in.

I am running 15/36 gear ratio, and my old motors were 170kv, the new ones are going to be 190kv
```

---
## \#16 Posted by: thiswasandy Posted at: 2018-10-12T21:09:11.804Z Reads: 134

```
Hey man checking in since you changed out your cans.

I’m also running a 12s4p with dual 190kv motors.

Any changes to your settings?
```

---
## \#17 Posted by: Jasonkimberson Posted at: 2018-10-12T21:25:50.491Z Reads: 126

```
Yes, made a few adjustments, changed the 40a to 50a.  If you want to run hard you can change that to 60a and it will be insane.  I’ll get some screen shots later
```

---
## \#18 Posted by: Jasonkimberson Posted at: 2018-10-13T08:25:38.535Z Reads: 116

```
![image|690x413](upload://AdwNkjljg7B7iTwNi1Sabv9qMop.jpeg) ![image|690x400](upload://m42qoPz13p4hSEuQnDamoOMXlOz.jpeg)
```

---
## \#19 Posted by: matthieuleblanc Posted at: 2020-01-14T15:38:10.842Z Reads: 26

```
Hi Jason

i would like to have advices about my Vesc setting  with VTC6 sony li-ion battery 
it's a 12s4p 12AH bms charge only

i have an orrsom board from Trampa with two 6364 154Kv motors 
i would to know the setting for :slight_smile:
MOTOR CURRENT MAX : ?
MOTOR CURRENT MAX BRAKE : ?
BATTERY CURRENT MAX : ?
BATTERY CURRENT MAX REGEN : ?
 and also about :
Minimum input voltage
Maximum input voltage
Battery cutoff start
Battery cutoff end

Thanks a lot for for advices i realy don't want to burn it all :sweat_smile:
```

---
## \#20 Posted by: Jasonkimberson Posted at: 2020-01-20T19:37:54.971Z Reads: 19

```
Sorry for the late reply.  Been off the forums.  You can see my last settings on this post for a similar build

https://www.electric-skateboard.builders/t/boosted-xl-boosted-board-deck-evolve-tb-trucks-janux-motor-mounts-the-eboosted-enclosures-dual-focbox-janux-6374-190kv-motors-12s4p-samsung-30qs-with-bestech-bms-enertion-nano-x-2-4ghz-remote-metr-at-bluetooth/67046/44
```

---
