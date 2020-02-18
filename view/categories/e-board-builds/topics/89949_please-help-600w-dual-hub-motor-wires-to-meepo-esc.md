# Please help. 600w dual hub motor wires to meepo ESC

### Replies: 19 Views: 663

## \#1 Posted by: Kmanna Posted at: 2019-04-09T17:32:08.087Z Reads: 123

```
Hi, guys im really new at this. Just got my first board from meepo like 2 months a go and fell in love with esk8ing. And i wanted to build something with a kick tail and smaller. Ive decided to go with this deck.

![1554830720857962624645774041527|375x500](upload://9YXlie0yeYfFWVu3RwArIIr4Pwh.jpeg) 

And i have a meepo ESC laying around so i decided to just use that. 

![15548308179482683973616014896655|666x500](upload://2PhIlzjJY05EhJdVTVdH12wBfNR.jpeg) 

And ordered some 600w 90mm wheel dual hub motors from china since im guessing thats what meepo uses anyways. For the price tag they have. 

![15548308846886405833705322295050|375x500](upload://jZRJFCukbSQRFmQgLpOh152O3PB.jpeg) 

And thinking of just getting meepo sanyo battery 10s 2p w case to finish. But the problem is how can i connect the motors to the ESC? What is the adapter/converter or work are needed to hook those up together? Please help. Thanks in advance. 

![15548310570933983006469507778572|375x500](upload://kTgsTKLtJxf2vMX7GxgUf9QHM6M.jpeg)
```

---
## \#2 Posted by: Miniproto Posted at: 2019-04-09T17:48:42.474Z Reads: 111

```
Im building right now with these Motors..  you can solder or buy new connectors to the ESC.
But I would keep the Gold Connectors and change the connectors on the Motor side.

As for the Sensors..red is 5V, black is GND, Yellow W,Blue U White is V..
But i believe you had Green instead of white.. i must look again if no one can answer.
```

---
## \#3 Posted by: bartroosen12 Posted at: 2019-04-09T18:05:38.672Z Reads: 112

```
I guess they use these MR30 connectors:
https://nl.aliexpress.com/item/1-paar-10-paar-Vergaren-MT30-MT60-MR30-Plug-Connector-Motor-connector-Man-Vrouw-Bullet-Connectors/32910177226.html?spm=a2g0s.8937460.0.0.418e2e0eBVdHHL

For the sensors I guess it's this type of connectors but I'm not sure:
https://nl.aliexpress.com/item/10-Sets-JST-XH2-54-XH-2-54mm-Draad-Kabel-Connector-2-3-4-5-6/32952337808.html?spm=a2g0z.search0104.3.76.1a221b56wrcg90&amp;transAbTest=ae803_4&amp;ws_ab_test=searchweb0_0%2Csearchweb201602_8_10065_10068_319_317_10696_10084_453_10083_454_10618_10304_10307_10820_10821_537_10302_536_10843_10059_10884_10887_321_322_10103%2Csearchweb201603_6%2CppcSwitch_0&amp;algo_pvid=ecaa1ac7-1fa0-483e-a590-e6c3734dcde0&amp;algo_expid=ecaa1ac7-1fa0-483e-a590-e6c3734dcde0-11
```

---
## \#4 Posted by: Kmanna Posted at: 2019-04-10T15:18:15.093Z Reads: 91

```
Ok, can you be more specific here for me? Which connectors do i need to get and do you have any video of doing the work? I'm sorry im very new at this. about 2 months old.. Thanks in advance.
```

---
## \#5 Posted by: Kmanna Posted at: 2019-04-10T15:18:41.463Z Reads: 89

```
So all i need to do is cut the wires and reconnect them with those type of connectors?
```

---
## \#6 Posted by: bartroosen12 Posted at: 2019-04-10T18:46:43.925Z Reads: 86

```
You need 2x MR30 connector:
The 3 motor wires are easy,
Both connect them to match the same collors (yellow,green,blue)

And 2x JST 5pin connector:
Then the sensors wires, you need to search for a datasheet for the color patern because mostly they use the same color combinations.
```

---
## \#7 Posted by: dtaoo Posted at: 2019-04-10T19:15:58.540Z Reads: 83

```
If anything meepo sells the adapters. https://www.meepoboard.com/accessories/mr30-to-bullet-connector-adaptor/

Would suggest making the adapters yourself, will be cheaper.
```

---
## \#8 Posted by: Kmanna Posted at: 2019-04-11T02:07:25.001Z Reads: 77

```
im sorry what do you mean by sensor the wire? and i cut off the motor side connectors and rewire it to MR30 connector?
```

---
## \#9 Posted by: Kmanna Posted at: 2019-04-11T02:11:26.896Z Reads: 78

```
I recently got in to electric skateboard so i dont really know well about electricity. This might be the best way to go since I need to order the battery case anyways. So, this is almost simple as plug and play right? connect the bullet wires to bullet and connect the MR30 to the esc? What about the 5pin connector?
```

---
## \#10 Posted by: Miniproto Posted at: 2019-04-11T16:10:52.769Z Reads: 71

```
I will make a video at the weekend.. Stay tuned. 😉
```

---
## \#11 Posted by: Kmanna Posted at: 2019-04-12T01:44:00.511Z Reads: 70

```
WILL BE STAYING TUNED!! lol 
Dont forget to post em here and help a brother out.. haha
```

---
## \#12 Posted by: Miniproto Posted at: 2019-04-13T13:40:28.574Z Reads: 63

```
There you go.. I hope it helps. 

https://youtu.be/2SxSvTeWmGc
```

---
## \#13 Posted by: Kmanna Posted at: 2019-04-13T16:44:00.983Z Reads: 60

```
So, in my case i need to buy bullet to MR30 connector to connect to motors to the ESC right? But what about the hall sensors? They look like this. 

![15551736508034323126533987837551|375x500](upload://zZDM8pg8gzY7oWXQj0Bf2H98e8k.jpeg) 

So, this and this goes together right? With the right adapter? 

![1555173722924496094498686037992|666x500](upload://pGMuUsNgGdyJXr1tp3V3Pv6R4OA.jpeg) 

And i have to find a 5 pin adapter for this to go to here? 

![1555173790844698107432083885771|666x500](upload://TRzoRDtvN4sh0TMfcdnGRwUk3f.jpeg) 

Anyone know the data sheet or which ones which on this MEEPO ESC?
```

---
## \#14 Posted by: Miniproto Posted at: 2019-04-14T06:35:06.026Z Reads: 57

```
Normally the white Connectors were with the Hub Motors but they were so small perhaps you threw them away accidentally? Because that's what i almost did. 

If not there are JST adapters for sale either in Amazon or AliExpress 
https://s.click.aliexpress.com/e/l8ryuic

As for the 3 phase Connectors you need to solder or fit with a adapter. 
Connection of the colors are in the Video.
```

---
## \#15 Posted by: Kmanna Posted at: 2019-04-22T01:21:26.258Z Reads: 52

```
Thank you so much i will try to follow along and post em plz follow up thank you

by the way did you finish building your board with those 600w dual hubs? plz post pic or vid of how it rides
```

---
## \#16 Posted by: Miniproto Posted at: 2019-04-22T04:48:13.368Z Reads: 49

```
Hi im working on the Carbon Kevlar Fiber Tray which i had to make a Mold first , takes a lot of time to finish it. In 1-2 weeks i will post pictures...
```

---
## \#17 Posted by: Miniproto Posted at: 2019-05-05T12:16:54.449Z Reads: 38

```
The build is nearly finished but the Carbon is mehh.. It was my first time, and gained experience but i will not throw away the part that I made. 
![IMG_20190505_131955|374x500](upload://79GJA9VKdk0qKM8tZbTPanBlPpy.jpeg)
```

---
## \#18 Posted by: Miniproto Posted at: 2019-05-21T18:20:24.413Z Reads: 32

```
I dont know if youre still following but i did a test ride for 10km and it feels great. Speed was about 25-30km/h with 10s im sure a lighter rider will reach 20mph+.
```

---
## \#19 Posted by: Kmanna Posted at: 2019-05-21T18:38:31.166Z Reads: 30

```
I did a lil test ride with mine too. The meepo esc and 10s 2p it was riding alright but making loud noise. I think because i didnt connect the hall sensors but i was getting wheel bites so im getting thicker riser and harder bushings
```

---
