# 10s bms with 9s battery

### Replies: 21 Views: 906

## \#1 Posted by: Bloop Posted at: 2018-07-21T13:24:05.045Z Reads: 117

```
Hey gus i have a 10s bms from besttech. is ther any chance i could use it for a 9s battery ?? or it wont work??

Thank you
```

---
## \#2 Posted by: Jake2k17 Posted at: 2018-07-21T15:27:06.690Z Reads: 103

```
It should work for charging as long as you connect it right.
```

---
## \#3 Posted by: Bloop Posted at: 2018-07-21T22:26:58.515Z Reads: 91

```
Hey @Jake2k17 thank you. I have anothe really stupid question.. Any idea what will happene if i try to charge a 9s battery with a 42v charger ? should there be any problem if i dont let it charge more than 37V ??? 

I need a solution for tomorrow cause i had some problems with a few elements from my battery and now my 10s has only 9s.. and i would love to finish this and dont really have time to wait for new batteries.
```

---
## \#4 Posted by: Bloop Posted at: 2018-07-21T22:35:03.917Z Reads: 83

```
i mean my bms has overcharge protection at 4.2v .. but is this for the cells or for the whole battery...
```

---
## \#5 Posted by: Jake2k17 Posted at: 2018-07-22T01:16:36.585Z Reads: 77

```
I think this would be ok because that is the recommended charger for liion packs 
I’m assuming your battery is a liion right? Even with lipos it should still be fine
```

---
## \#6 Posted by: Jake2k17 Posted at: 2018-07-22T01:17:08.629Z Reads: 74

```
This is for the cells, each cell is fully charged at 4.2
```

---
## \#7 Posted by: Bloop Posted at: 2018-07-22T04:18:51.623Z Reads: 70

```
Yeah im using li.ion.

9s * 4.2 = 37.9V charging
42V is for the 10s. I dont understand what you mean by 'recommended charger' ?

I know the full cell is 4.2 but if the bms has overcharge protection will check each cell not to go over 4.2 or will check the final Voltage to stop at 42V.

Hmm.. and if i only wire 9s on the 10s bms will it still keep the overcharge protections hmmm....
```

---
## \#8 Posted by: Jake2k17 Posted at: 2018-07-22T04:42:54.490Z Reads: 68

```
Well if you go on mboards or other liion battery sites they charge brick they send is the 42 v. Honestly though you should just add one more cell into your pack and make it 10s and it is 100 times easier
```

---
## \#9 Posted by: Bloop Posted at: 2018-07-22T05:07:06.575Z Reads: 61

```
Yeah im aware is easyer and that was the plan before one of my cells got dmged.

my question was something else...
```

---
## \#10 Posted by: Jake2k17 Posted at: 2018-07-22T05:29:34.293Z Reads: 57

```
Assuming you are in US I just searched up 9s bms and multiple were available. They are a little pricier at $45 but it’s a better option than charging 9s with 10s bms
```

---
## \#11 Posted by: Namasaki Posted at: 2018-07-22T05:35:55.339Z Reads: 54

```
You can NOT use a 10s bms for a 9s battery unless the bms is designed for multiple series configurations.
If it is designed specifically for 10s, then it will only work with 10s.
```

---
## \#12 Posted by: Bloop Posted at: 2018-07-22T06:02:41.649Z Reads: 53

```
Is a bestech bms designed for 16s but has the resistors and components for 10. 

If i only connect the first 9 cells i assume it will work just fine.. the biggest problem is that i dont have a charger for 9s.. only the 10s one. If i try to charge with 42V and only charge to 37V and dont go over( not to overcharge) should it work or will it break and it wont work from the start

![IMG_20180707_111228|666x500](upload://gkPYPJi9IO4rRGv3Y7n9Sjcw13u.jpg)
```

---
## \#13 Posted by: pat.speed Posted at: 2018-07-22T06:07:57.262Z Reads: 51

```
Yes, it will work ok. Just leave the last balance lead disconnected. I use a 13s bms for my 12s lipo as 12s bms’ are hard to find for cheap. 

You CANNOT use that 42v charger though. It will ruin your pack. You MUST use a 37.8v charger
```

---
## \#14 Posted by: Jake2k17 Posted at: 2018-07-22T06:08:50.534Z Reads: 50

```
Jesus then nobody buy any battery packs from mboards lol
```

---
## \#15 Posted by: pat.speed Posted at: 2018-07-22T06:12:27.918Z Reads: 50

```
What do you mean? A 10s pack needs a 42v charger. Any other pack needs it’s spec’d charger
```

---
## \#16 Posted by: Bloop Posted at: 2018-07-22T06:31:44.933Z Reads: 48

```
Jake to get the charging voltage for battery you need to get the max that battery can hold (4.2v) and multiply with the number of series cells you have. 10s - 42v, 9s - 37.9V etc 

Many 10s charger will also reffer to 37V because they are using the normal voltage for a li.ion cell 3.7V but this is not max. You will see that they have in paranthesis 42V 

@pat.speed Thank you for the response. I will try to find another way altho.. i really wanted to test this out today.. before i leave so i was just looking for unconventional methods...
```

---
## \#17 Posted by: b264 Posted at: 2018-07-22T07:21:36.503Z Reads: 47

```
[quote="Bloop, post:3, topic:62452"]
Any idea what will happene if i try to charge a 9s battery with a 42v charger ?
[/quote]

Fire&nbsp;
```

---
## \#18 Posted by: Namasaki Posted at: 2018-07-22T07:33:47.742Z Reads: 45

```
[quote="pat.speed, post:13, topic:62452"]
I use a 13s bms for my 12s lipo as 12s bms’
[/quote]

What bms are you using?
I'm using the Bestch HCX-D223V1 for 10s which is what appears to be pictured above.
If it doesn't see 10 cells, it will go into protection mode and shut down.
```

---
## \#19 Posted by: Namasaki Posted at: 2018-07-22T07:51:15.450Z Reads: 45

```
[quote="Bloop, post:12, topic:62452"]
Is a bestech bms designed for 16s but has the resistors and components for 10.
[/quote]


They use the same basic board for various configurations.
Your bms was configured for 10s.
If you only connect 9 cells, it should shut down in protection mode as soon as you turn it on.
```

---
## \#20 Posted by: Bloop Posted at: 2018-07-22T07:56:29.579Z Reads: 44

```
:-( aww ok thank you
```

---
## \#21 Posted by: pat.speed Posted at: 2018-07-22T10:46:33.954Z Reads: 39

```
Oh that’s strange. I know that “dumb bms” does not know when the last cell is missing. 

I am using a Chinese charge only bms, cost me about $10 on eBay
```

---
