# Some help with a battery

### Replies: 22 Views: 347

## \#1 Posted by: TreeFactory Posted at: 2019-02-13T23:08:05.001Z Reads: 96

```
Hello, I'm not as confident as I'd like to be about this. I've searched about and couldn't find a definitive answer so I figured I'd ask here. Does anyone know if the red wire is the first positive wire or the ground wire? My instinct is that it's the first positive but I don't know for sure.![0213191805_HDR|690x388](upload://yUBtCAq7b7Mbj5foKedfgYbXQAt.jpeg)
```

---
## \#2 Posted by: rich Posted at: 2019-02-13T23:21:48.968Z Reads: 90

```
The red wire is the last positive (3rd cell) :wink:

Pins:
1. B-
2. B1+
3. B2+
4. B3+ (red wire)
```

---
## \#3 Posted by: Arzamenable Posted at: 2019-02-13T23:29:18.373Z Reads: 82

```
I concur if it makes you feel any better. Not that Im an expert compared to @rich, but I’ve recently burned up a charger so I understand your hesitancy. 

Consider getting a multimeter 👍  ⚡️⚡️⚡️
```

---
## \#4 Posted by: Lambjr088 Posted at: 2019-02-13T23:31:08.145Z Reads: 82

```
I concur it is the last. But please try and get your hand on a multimeter any would help specially in this sport or hobby
```

---
## \#5 Posted by: TreeFactory Posted at: 2019-02-13T23:31:26.219Z Reads: 81

```
Thank you guys for the help. I'm making a 12s LiPo with a BMS I picked up. From what I can tell there is 13 wires on the BMS and from what I've learned here I am supposed to ignore all the B-'s except for the last one.
```

---
## \#6 Posted by: Arzamenable Posted at: 2019-02-13T23:33:14.382Z Reads: 74

```
Pics or it didn’t happen
```

---
## \#7 Posted by: Arzamenable Posted at: 2019-02-13T23:37:02.086Z Reads: 72

```
I am currently doing similar shenanigans ![image|375x500](upload://k3jGAT097HSJpvKUBBu6BF5DFCp.jpeg) 


What does your BMS look like?
```

---
## \#8 Posted by: TreeFactory Posted at: 2019-02-13T23:39:26.521Z Reads: 71

```
![0213191838_HDR|690x388](upload://yUwZQcWAN4qZZJsdkHGNyoGEfZs.jpeg)
```

---
## \#9 Posted by: Arzamenable Posted at: 2019-02-13T23:43:52.002Z Reads: 69

```
I presume these are the parts still? 
![image|690x249](upload://qMqq4lU9yKCUCsi8nwnsDtJHYvv.jpeg)
```

---
## \#10 Posted by: TreeFactory Posted at: 2019-02-13T23:44:41.075Z Reads: 66

```
minus the 100a anti spark. I've decided to go with a loop key instead
```

---
## \#11 Posted by: TreeFactory Posted at: 2019-02-13T23:53:40.544Z Reads: 63

```
Had to take a hiatus on building cause life gets in the way sometimes but I'm back to trying to get this guy done
```

---
## \#12 Posted by: Arzamenable Posted at: 2019-02-14T00:01:41.304Z Reads: 61

```
Are you hardwiring (soldering and cutting stock leads) this or marking an adaptor?
```

---
## \#13 Posted by: TreeFactory Posted at: 2019-02-14T00:05:41.543Z Reads: 62

```
Making adapters so if a battery dies it will be easier to swap out. That being said I am soldering the stock leads from the BMS(the white wires) to the clips for the adapters instead of crimping and adding more wire in between connections.
```

---
## \#14 Posted by: TreeFactory Posted at: 2019-02-14T00:09:22.910Z Reads: 59

```
I'm also not to sure if the range will work out for me with these only being 6000MaH so I don't wan't to hardwire.
```

---
## \#15 Posted by: mynamesmatt Posted at: 2019-02-14T03:08:09.057Z Reads: 52

```
if you ever have doubts, use your multimeter and test between the connection. if the result is 0 volts between red and red that means its the same. if it's 3.7 ish volts then it's between cell one and 2 for example
```

---
## \#16 Posted by: Arzamenable Posted at: 2019-02-14T04:14:45.009Z Reads: 51

```
![image|346x500](upload://lZrEbib8ZUadVRFsHUf3tnQzoM6.jpeg) 

Sorry, I am not an engineer. This configuration doesn’t cut up your leads. Your current is controlled by the ESC (80A in this case).

@Namasaki has several great posts that detail these set ups. 

Don’t take this as gospel, but I am fairly certain its correct.
```

---
## \#17 Posted by: TreeFactory Posted at: 2019-02-14T06:27:42.120Z Reads: 40

```
This is pretty much what I was planning. they're 13 wires coming out of my particular BMS though. That 13th is supposed to be the last B- correct? Or do I have an extra lead for some reason?
```

---
## \#18 Posted by: rich Posted at: 2019-02-14T10:14:33.863Z Reads: 35

```
[quote="TreeFactory, post:17, topic:84142"]
That 13th is supposed to be the last B- correct? Or do I have an extra lead for some reason?
[/quote]

It's the first B- (B0).

Just for understanding, B- (also called B0 on balance wires) is the negative lead of the first cell of your battery. B1+ is the positive of the first cell, B2+ is the positive of second cell and so on.

That's why it's important that your first lipo is battery negative and the last and fourth in series the main battery positive.

I changed the nice diagram of @Arzamenable to your needs

![diagram_00e|346x500](upload://3Bk0FpyQt3CEvugAX5aOBK7HFDx.jpeg) 

On the PCB of your BMS should be printed which cable is which connection.

There are different types of BMS available that's why many are confused and shouldn't just copy diagrams which could be wrong for their setup. If you understand how "your" BMS should be connected then you can draw your own diagram and are ready to go.

In any case you must connect the main battery negative to B- before connecting the balance wires to BMS.

And as mentioned, use a multimeter before plugging the main balance connector. Negative on B0 or main negative, then start with the positive tip on B1+, then B2+ and so on, every step should increase the voltage about 3.8V (or whatever your cell voltage is) until you reach your main voltage at B12+.

[quote="Arzamenable, post:3, topic:84142"]
Not that Im an expert compared to @rich
[/quote]
:joy:
Thanks but would an expert cut a 6s balance extension with scissors while it's still connected to the battery? Damn, that was an instant adrenaline rush from the hissing, popping and sparkling sensation.
```

---
## \#19 Posted by: TreeFactory Posted at: 2019-02-14T15:19:24.295Z Reads: 22

```
This has been wildly helpful. I would have had the battery order backwards. I thought where its marked the number 1 battery would have been in the number 4 spot due to thats where the positive cable goes to the ESC's
```

---
## \#20 Posted by: TreeFactory Posted at: 2019-02-14T15:22:41.264Z Reads: 23

```
Meaning i was about the put that ground lead in the wrong order
```

---
## \#21 Posted by: rich Posted at: 2019-02-14T16:23:57.803Z Reads: 19

```
Glad I could help. 
You have no idea how long it took for me to understand everything :grin:

It's easy to mess up the right order with balance wires
For example here is on the top B0 and on the bottom B6+. If the female connector would be on the left side the order would be mirrored with B6+ on top.

![100950h|690x388](upload://fhB8tzEjaiJROsW2OXFqZBITfXX.jpeg) 

When the female connector is this way (so you can see the pins) then is B6+ on the top and B0 on the bottom. If the cable of the female connector comes from the left side it's mirrored, too.

![101332h|690x388](upload://dudml7umc61DYIbGCyph0xK859M.jpeg) 

Then the print on the PCB is on the bottom side so it's mirrored from the top. Many faults possible.
That's why it's recommended to check all voltages with a multimeter before plugging it to BMS.
```

---
## \#22 Posted by: TreeFactory Posted at: 2019-02-14T19:10:06.721Z Reads: 15

```
I will defiantly be picking one of those up before fully assembling this. Again, thank you guys for the help. I'd have a pile of non working, non matching parts if it wasn't for this site.
```

---
