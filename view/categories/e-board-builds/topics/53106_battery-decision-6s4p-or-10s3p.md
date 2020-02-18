# Battery Decision (6s4p or 10s3p)

### Replies: 13 Views: 747

## \#1 Posted by: Sean Posted at: 2018-04-22T08:51:33.454Z Reads: 138

```
Hello guys,

I have a hard time on deciding which battery pack to choose, my build won't be targeted towards speed, it will 'just' be a daily commuter to get from home to tram and from there on to my university.
Both packs would work with the FOCBox without problems right? And both would be around the sam weight?
What do you guys think? 
Keep in mind I am going for the Jet Spud Deck and the Turnigy SK3 6364 190kv
And I am not that heavy :wink: 

Thanks in Advance
```

---
## \#2 Posted by: Jebe Posted at: 2018-04-22T08:53:45.039Z Reads: 134

```
10s 3p- will use less current and be easier on the pack - do you have an existing board ? easier to go with the same voltage use the same charger.
```

---
## \#3 Posted by: Sean Posted at: 2018-04-22T08:57:58.631Z Reads: 135

```
I have been using LiPo's from Hobbyking (6s), however I would like to use a dedicated battery pack with bms and a charger
```

---
## \#4 Posted by: rey8801 Posted at: 2018-04-22T09:07:53.201Z Reads: 129

```
I recently built a jet spud eskate. I used 10s3p battery pack and I get at least 30km range of it with a average speed of 20-25khm and some hills. I say at least because I never went lower than 40% left battery and that was after 2 days of riding of around 18-20km total. I also don't charge the battery to 100% but stop at 41.2 (more conservative) and discharge up to 30. With 30Q It still rode powerful at 40% left. I know that know the @Lumaci is not selling anymore, but few days ago you could grab a really good deal. Please, post pics when you start build it, I am in love with spud builds.
```

---
## \#5 Posted by: Sean Posted at: 2018-04-22T09:11:34.614Z Reads: 116

```
Thanks for the fleshed out answer! Did you have any problems fitting the battery pack under the deck? Is it heavy?
I'll be able to set all those limitations in the FOC setup right? I have only been using Car ESC's and I would love to use a FOCBox, I heard a lot of good thins about it.
```

---
## \#6 Posted by: rey8801 Posted at: 2018-04-22T09:20:35.189Z Reads: 106

```
You heard right. Moreover if you want run it in FOC it's a must have. Also VESC 6 or ESCape if you have the money for. In BLDC you can also think at 4.12 hardware vesc as I did. It's up to you. The battery is not small for the deck size. I couldn't fit it underneath with a pre-made enclosure mainly because I wanted to put to much stuff (BMS with heatsink for discharging, both loop keys and antispark switch). If you use a small bms charging only and either antispark switch or loop key you will save a lot of space. Better if you do your connections with XT60 and not XT90. I used XT90 only for the battery side and I had to remade all the other with XT60 to gain room. With this set up you can for instance buy the unik enclosure that looks fantastic for the price to me, just attached all the electronics to the deck (regardless the enclosure we should do all in that way). 
Ps: if you decide to run it single drive than you will have way more space...

Check my build of you need some parts I used.
```

---
## \#7 Posted by: Sean Posted at: 2018-04-22T09:37:16.753Z Reads: 97

```
Thanks man :)
```

---
## \#8 Posted by: Lumaci Posted at: 2018-04-22T14:39:35.779Z Reads: 84

```
Yeah the unik enclosure is really nice and fits well on smaller boards, also use velcro for a great fitment and clean look costs nothing but might save you some money down the road since a broken vesc aint fun to replace.

![30825248_1625267594236428_1246129754_o|375x500](upload://6vqpmy0r7ctFxIhAaRDP5hHrKai.jpg)
```

---
## \#9 Posted by: rey8801 Posted at: 2018-04-22T15:25:39.078Z Reads: 77

```
I told him about the big deal you had few days ago. I was still thinking about it :grin:
Anyhow I see that your unik deck doesn't have the hole underneath the enclosure as I have seen it in other of their decks.
```

---
## \#10 Posted by: Lumaci Posted at: 2018-04-22T15:32:38.375Z Reads: 73

```
Like this? :-) Its their old version, recently switched it out for the new version.

Looks and feels so much better, the old one i had was broken fixed it up and gave it to a guy in need of a new deck.

![image|666x500](upload://dphSzhjufQkdTOdQgRK2HzIyIJn.jpg)
```

---
## \#11 Posted by: rey8801 Posted at: 2018-04-22T15:39:40.812Z Reads: 70

```
I didn't know about the two version. Thanks for the update!
```

---
## \#12 Posted by: deucesdown Posted at: 2018-04-22T15:42:16.239Z Reads: 70

```
6s vs 10s, if you don't care about top speed, there are some advantages to 6s. You should take a look at a bunch of @lowGuido's posts.

- can skip BMS and use a hobby charger. Bring balance and charge leads out to a VGA connector. Hobby charger will give you a lot more insight to pack health (but won't protect the pack while in transit)
- lower voltage means you can use DC circuit breaker switches instead of the failure prone vedder antispark switch
- easier/cheaper to build 6s with lipo
```

---
## \#13 Posted by: DeathCookies Posted at: 2018-04-23T09:25:52.242Z Reads: 53

```
[quote="deucesdown, post:12, topic:53106"]
can skip BMS and use a hobby charger. Bring balance and charge leads out to a VGA connector.
[/quote]
you can easily use a dvi connector for 12S

[quote="deucesdown, post:12, topic:53106"]
lower voltage means you can use DC circuit breaker switches instead of the failure prone vedder antispark switch
[/quote]
At that time we did not know many Information about the vedder Switch and how it works. Nowadays we know that we have to attach a button and leave it in the off Position when attaching a battery pack

[quote="deucesdown, post:12, topic:53106"]
easier/cheaper to build 6s with lipo
[/quote]
Thats true but it will not be easier to Charge. Here everyone has to decide if you build it user friendly or cheap which results in a bit more work every day for charging the pack
```

---
