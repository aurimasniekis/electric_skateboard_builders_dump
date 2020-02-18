# Can I charge through this loop key port?

### Replies: 32 Views: 1320

## \#1 Posted by: AssaultedPotato Posted at: 2018-01-17T06:18:58.201Z Reads: 166

```
![0116182213_HDR|666x500](upload://6GU6xGk3zRyeYi8js5UMj38ACoe.jpg)
```

---
## \#2 Posted by: Colson003 Posted at: 2018-01-17T06:24:23.278Z Reads: 161

```
Took me a minute to comprehend that wiring. No you could only use that for a loop key. Charge port would need to be on the same two leads as the vesc.
```

---
## \#3 Posted by: AssaultedPotato Posted at: 2018-01-17T06:25:32.024Z Reads: 155

```
So I would need to plug in the loop key to charge?
```

---
## \#4 Posted by: Colson003 Posted at: 2018-01-17T06:26:33.604Z Reads: 152

```
Yes. Unless you put the loop key on the positive lead closer to the vesc than the charge port.
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-01-17T06:28:54.261Z Reads: 140

```
As @Cmaselli said. Do NOT connect the loop key to the antispark! If you do you will short your batteries and destroy them
```

---
## \#7 Posted by: Ishayc Posted at: 2018-01-17T06:30:16.055Z Reads: 131

```
If you connect this loop key you will blow up your battery.
a loop key creates a short and it needs to create it on the plus or minus wire not between the plus and minus.
```

---
## \#8 Posted by: AssaultedPotato Posted at: 2018-01-17T06:32:24.449Z Reads: 125

```
Wait I'm confused now. First according to Colson003 this could only be used for a loop key. Now Cmaselli and Ishayc say it can only be for charging?
```

---
## \#9 Posted by: Colson003 Posted at: 2018-01-17T06:33:16.910Z Reads: 125

```
Pretty sure the orientation is messing with everyone. ![IMG_0111|375x500](upload://hlRo4DCjva9FS9LoYQWCOmYkBUN.PNG)

This isn't a common way of using a loop key, I've seen it done before. It's just not common as you'd need the loop key connected to charge the pack.
```

---
## \#10 Posted by: FredrikHems Posted at: 2018-01-17T06:34:21.882Z Reads: 113

```
Can you please provide some better pictures of your wiring? Or a schematics
```

---
## \#11 Posted by: Ishayc Posted at: 2018-01-17T06:36:02.364Z Reads: 113

```
Oh i now see that you have them all in series.
confusing picture.
```

---
## \#12 Posted by: AssaultedPotato Posted at: 2018-01-17T06:36:07.525Z Reads: 106

```
Sorry, the orientation was kind of confusing. @Colson003 has the clearer picture. Can I charge through that loop key port?
```

---
## \#13 Posted by: Cmaselli Posted at: 2018-01-17T06:36:41.772Z Reads: 106

```
Oh shoot, you're right. Sorry, I saw red and black going into the loop key xt90 and I freaked out lol
```

---
## \#14 Posted by: Ishayc Posted at: 2018-01-17T06:38:10.866Z Reads: 105

```
Nope.
You need to take the wires that are connected to the vesc and charge through them.
Put the loop key between the charging port and the vesc.
```

---
## \#15 Posted by: FredrikHems Posted at: 2018-01-17T06:38:24.156Z Reads: 100

```
No you can not charge through it. First problem is that you will need a 12s charger, which i doubt you have. You will also need to wire up the balance wires.
```

---
## \#16 Posted by: AssaultedPotato Posted at: 2018-01-17T06:38:41.471Z Reads: 101

```
It's 8s, and I have an 8s charger.
```

---
## \#17 Posted by: FredrikHems Posted at: 2018-01-17T06:40:00.124Z Reads: 98

```
Oh, I belived it was an 12s setup. But still, you cant charge through that If I remember right
Edit: Please post a schematics including Vesc and balance leads
```

---
## \#18 Posted by: Ishayc Posted at: 2018-01-17T06:45:25.024Z Reads: 97

```
![image|375x500](upload://k0WrD1SSkFkRMuDHA5AAzyqjTuy.jpg)
```

---
## \#19 Posted by: AssaultedPotato Posted at: 2018-01-17T06:51:43.597Z Reads: 92

```
![0116182250_HDR|375x500](upload://wV0Cd2TJfjC0apExoTvjGB4iVnp.jpg)
```

---
## \#20 Posted by: Colson003 Posted at: 2018-01-17T06:52:00.500Z Reads: 90

```
Here's one with the loop key still between the packs. ![IMG_0116|375x500](upload://zPwgN9qONMRh2glniwf9jTsEZDr.jpg)
```

---
## \#21 Posted by: Colson003 Posted at: 2018-01-17T06:53:18.935Z Reads: 86

```
So to be clear, you CANT use the same port for both charge and loop key. 
You CAN have the loop key between packs, but it will also have to be connected when charging.
```

---
## \#22 Posted by: Ishayc Posted at: 2018-01-17T06:55:59.634Z Reads: 75

```
As I drew, the loop key should be before the vesc that you won't charge the batteries and have the vesc on.
And yes, you cant use the same port for both.
```

---
## \#24 Posted by: Colson003 Posted at: 2018-01-17T06:58:04.488Z Reads: 70

```
Yes that is where it should be, but if he wants it between the packs he can do so.
```

---
## \#25 Posted by: AssaultedPotato Posted at: 2018-01-17T06:58:43.462Z Reads: 72

```
Eh I'd rather not have to also plug in the loop key in order to charge
```

---
## \#26 Posted by: Ishayc Posted at: 2018-01-17T06:58:53.815Z Reads: 74

```
Then he must have the vesc on when he charges. 
Not a good idea.
```

---
## \#27 Posted by: AssaultedPotato Posted at: 2018-01-17T07:00:26.021Z Reads: 72

```
With the vesc in parallel with the battery while charging, it would turn on anyway. I think you mean with the loop key plugged in?
```

---
## \#28 Posted by: Colson003 Posted at: 2018-01-17T07:01:03.684Z Reads: 72

```
My battery uses a bms and when I plug it in it turns everything on. I haven't had an issue with the vesc being on while charging.
```

---
## \#29 Posted by: Ishayc Posted at: 2018-01-17T07:01:58.346Z Reads: 67

```
The loop key must be in if you don't change it's place therefore the vesc will be on.

Go with how I drew it and save you the trouble.
```

---
## \#30 Posted by: Ishayc Posted at: 2018-01-17T07:06:02.939Z Reads: 67

```
Then you actually have the option to charge and pull current at the same time from the battery?
Not recommended.
```

---
## \#31 Posted by: Colson003 Posted at: 2018-01-17T07:10:01.057Z Reads: 64

```
I don't know exactly how it's wired up. Its from TB, I'm pretty sure all their packs are like that.
```

---
## \#32 Posted by: scepterr Posted at: 2018-01-17T07:17:18.812Z Reads: 60

```
Just run the charge port Before the loopkey
```

---
## \#33 Posted by: Clonkex Posted at: 2018-01-17T07:17:47.918Z Reads: 63

```
I don't believe it makes a difference. All it will do is take some load off the batteries equivalent to whatever the charge current is. The charger is current-limited, so it won't hurt the charger, and the current won't go into the batteries and back out again, it'll just flow to everything.

Think about laptops or phones or any electronic device with a battery. They quite happily charge while current is being drawn from the battery.
```

---
## \#34 Posted by: Ishayc Posted at: 2018-01-17T07:25:06.558Z Reads: 62

```
@Clonkex -  
All those Electronic devices you are talking about has protection and a more sophisticated circuit that is build to do those stuff. 

A good explanation can be found here - https://arduino.stackexchange.com/questions/39805/can-you-charge-and-use-a-lipo-battery-at-the-same-time

Another issue you will have is the currents.
When you charge and discharge simultaneously, the currents are in a different direction.
If you charge with 2A and the load(VESC) asks for 10A the battery will provide 8A.
```

---
