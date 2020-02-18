# Need help in wiring everything together

### Replies: 27 Views: 524

## \#1 Posted by: danepoostain Posted at: 2019-03-26T23:50:24.074Z Reads: 116

```
I am in the end stages of putting everything together to complete my first build. I need a little reassurance on how to wire everything together. This is what I am working with...

12S5P Battery,
FocBox Unity, 
2.4 GHz Controller,
BMS, 
Dual 6374 - 190KV Motors 


I am still in need of a Charging Port and Charger. Open to any recommendations?!

Here are some pics to help show what I am working with... ![IMG_3252|375x500](upload://AeofmAhZtucWrJ5fZ4M1W5HhRcj.jpeg) ![IMG_3254|375x500](upload://559VoFj3clLax9Uy3K78cU5GlXQ.jpeg) ![IMG_3256|375x500](upload://sPrr7fPLPk5HWlcNrgnVoSzjl85.jpeg) ![IMG_3255|375x500](upload://wkZ1HMBwdgJyLnysxRdxYEK5xeD.jpeg) 

A couple of the issues that have come up...
-Not sure how to connect my the motors hall sensors? It seems like the spot they get plugged into the FOCBOX are not the right size. 

-From the Battery I have a XT90 and the FOCBOX has XT60. Can I solder a XT60 Female onto the XT90 to make them connect or is this a no no? 

- Two things that I am really stuck on is how to wire the BMS on this setup? And How to wire in the charge port (still need to order one, any recommendations? Also need to order the actual charger.)

Any help is much appreciated!
```

---
## \#2 Posted by: ryansinatra Posted at: 2019-03-26T23:56:08.447Z Reads: 108

```
Well, first you need some balance leads, but I don't see any. 

I would take the xt90 off the battery and just solder on the xt60 to match the unity so you don't void the unity warranty
```

---
## \#3 Posted by: danepoostain Posted at: 2019-03-27T00:14:04.788Z Reads: 108

```
Good point on the xt60. Should be simple enough to do. 
Can you elaborate in the balance leads? Would that be the smaller wires (+,-) coming from the battery? 

I had @eboosted make the battery for me. He marked on the bms which end goes where (big dot, small dot). Would any of these include the balance leads? See Pics.. ![IMG_3258|375x500](upload://jo0meVBnE4QE7zg5HsrHeZOfOor.jpeg) ![IMG_3259|375x500](upload://rSwVNecDlwpqqHgHVqNkg2L5Zy3.jpeg)
```

---
## \#4 Posted by: Scream Posted at: 2019-03-27T00:25:09.954Z Reads: 100

```
I agree with Ryan, change the battery connector to an xt60 - then you could just connect the Unity straight to the battery, bypassing the BMS (for simplicity).

You are definitely going to want to run your charging circuit through the BMS though. It looks like there's a balance lead loom attached to your battery. Don't plug this into the BMS just yet, but can you tell if it is a match for the white plug on the BMS? I'm guessing whoever made your battery supplied the BMS, so it probably is a match.

Before you plug it in though, you need to connect B- on the BMS to the negative terminal of the battery, and CH- to the negative on your charge port of choice. I just used a DC power plug - but I recommend going with a plastic body one to reduce the chance of accidental shorts.

For the positive lead to the charge port, this connects straight to the positive terminal of the battery - but I recommend adding a 10A fuse in line. I use the glass cylinder ones.

You can use a thinner gauge wire for charging, I think I used 18AWG, but you could go thinner.

EDIT: cool, the balance leads should be straightforward
```

---
## \#5 Posted by: Scream Posted at: 2019-03-27T00:27:20.202Z Reads: 93

```
I suppose if you don't want to unwrap the battery, and you're already taking off the xt90 plug, you could splice the charging circuit onto the battery power leads.
```

---
## \#6 Posted by: Eboosted Posted at: 2019-03-27T00:54:43.562Z Reads: 88

```
I'll gladly help you out man.

1. Change your XT60 from you Unity to the XT90 port I sent you:

![image|375x500](upload://okMW77O6KhUCS1tRpFdfpM0AlqA.jpeg) 

2. These are the instructions to wire the BMS

B- on the BMS
![image|509x500](upload://olTlbfQzdZIxrq5AShbYALU7Uf2.jpeg) 

goes to battery negative
![image|610x500](upload://i5UI8mZ98w6pc8JxEVtvm1bQHKf.jpeg) 

CH- on the BMS
![image|589x500](upload://uKcq41ELRKGTupE8zAsmja4ABek.jpeg) 

goes to negative of charge port
![image|500x500](upload://yNQmdVBb4ae7stFKJR4hKrhbZ8C.jpeg) 

Positive of charge port goes to, positive of battery pack:
![image|643x500](upload://4qrJKNMWTGUk6kpGHL4G2APQdU0.jpeg)

3. Connect the BMS jst plug to the BMS
```

---
## \#7 Posted by: danepoostain Posted at: 2019-03-27T01:01:14.158Z Reads: 83

```
I made this before I saw your reply @Eboosted. Thanks for the help! Does this look right? Ignore my paint app skills :slightly_smiling_face:![Wiring|375x500](upload://3kmApwWYr7C4jjvciYOqUCqH1Ga.jpeg)
```

---
## \#8 Posted by: Eboosted Posted at: 2019-03-27T01:13:59.977Z Reads: 78

```
That's corect man! you are in the right path
```

---
## \#9 Posted by: danepoostain Posted at: 2019-03-27T01:31:35.371Z Reads: 75

```
Do you have any recommendations on chargers? and the physical charging port?
```

---
## \#10 Posted by: J_Dizzle Posted at: 2019-03-27T02:32:33.020Z Reads: 73

```
https:///collections/battery-chargers/products/12s-4a-battery-charger
https:///collections/battery-chargers/products/12s-2a-battery-charger
These are your best bets, Build Kit Boards has one but they are out of stock.

Edit:
Here is reliable charging jack: 
https://buildkitboards.com/collections/batteries/products/2-1-2-5mm-charging-jack
```

---
## \#11 Posted by: danepoostain Posted at: 2019-04-04T20:19:19.993Z Reads: 60

```
Thanks for all the help guys! I ran into one more issue. The charge port has 3 prongs. I know the odd looking one at the top is for the negative from the BMS, but what do I do with the other 2? Which one is the positive of the 2 remaining? @Eboosted   ![IMG_3272|375x500](upload://e7ANFFGjCLFHRn9h8vZMucHPVEG.jpeg)
```

---
## \#12 Posted by: Scream Posted at: 2019-04-04T20:25:42.368Z Reads: 60

```
You got a multimeter?

Test continuity/resistance across those two tabs, might find they are connected to the same thing.

Otherwise test continuity from each tab to the centre pin on the charge port. The one that’s connected is your positive.
```

---
## \#13 Posted by: Scream Posted at: 2019-04-04T20:27:09.340Z Reads: 61

```
Also... you sure that top one is the negative bro? Looks like that might connect to the centre pin - i.e. positive.
```

---
## \#14 Posted by: mmaner Posted at: 2019-04-04T20:27:12.427Z Reads: 66

```
![image|690x362](upload://9AR5SGMTdUyI0FY2CzhuNFC2JxK.jpeg)
```

---
## \#15 Posted by: danepoostain Posted at: 2019-04-11T23:27:55.677Z Reads: 60

```
@Eboosted Trying to setup my FOCBOX Unity...
I have a 12S5P battery pack. 

what is the max battery discharge current? 

what should I be setting the max regen braking current to?

I have the 6374 190KV motors from torque boards. 

What is my max motor current and max brake current?
```

---
## \#16 Posted by: Eboosted Posted at: 2019-04-11T23:35:25.971Z Reads: 60

```
Maximum battery discharge on the Samsung 30Q and 12s5p is 75A specified and 100A if you want to push the batteries to the max. I'd personally use 100A and have used that on all my boards.

Max regen shouldn't be more than 15A
```

---
## \#17 Posted by: danepoostain Posted at: 2019-04-11T23:38:22.338Z Reads: 55

```
Thank you @Eboosted 

I looked up the motors from torque boards. They say max amps is 80. 

Still not sure about max braking amps?
```

---
## \#18 Posted by: Eboosted Posted at: 2019-04-12T00:21:12.026Z Reads: 53

```
80A is a lot of current, you will only have 50A for each motor on the 12s5p configuration
```

---
## \#19 Posted by: danepoostain Posted at: 2019-04-16T16:33:12.067Z Reads: 47

```
@Eboosted I'm having trouble getting the board to charge. Is there a way I can trouble shoot this? I would guess that it has to do with the way I have the charge port wired..not sure.
```

---
## \#20 Posted by: Eboosted Posted at: 2019-04-16T16:36:46.078Z Reads: 45

```
Can you should me pictures of your wiring?
```

---
## \#21 Posted by: danepoostain Posted at: 2019-04-16T17:48:36.060Z Reads: 44

```
@Eboosted ts a bit of a mess and once i can figure out this charging issue i will clean it up

Here is the overall pic...![IMG_3290|375x500](upload://bQQ4jq1cNDjeTxpXilir9S4vJDR.jpeg) 

Here is my positive to the positive lead...![IMG_3292|375x500](upload://24pW5qJVLeaGU5odUlq840Txj7e.jpeg) 

Here is my negative from charge port to bms..![IMG_3291|375x500](upload://lMJEiUcSBUJ2a77LPzvcVA4YNja.jpeg) 

Here is my negative lead to bms...![IMG_3294|375x500](upload://yAFmo1HKMuU6vJLEzI5k8TKVULP.jpeg)
```

---
## \#22 Posted by: Eboosted Posted at: 2019-04-16T17:57:12.343Z Reads: 44

```
I can't see where you connected the negative of the charge port, it should go to CH- on the BMS, can you take off the green insulator?
```

---
## \#23 Posted by: danepoostain Posted at: 2019-04-16T18:02:33.740Z Reads: 42

```
![IMG_3295|375x500](upload://1axx4h9UEKI8GLJQ730SBzWj3nf.jpeg)
```

---
## \#24 Posted by: Eboosted Posted at: 2019-04-16T22:35:39.483Z Reads: 40

```
The connections seems to be good.

What happens when you charge the battery?
```

---
## \#25 Posted by: danepoostain Posted at: 2019-04-16T22:37:52.026Z Reads: 40

```
it just doesnt charge. Not sure what the issue might be.
```

---
## \#26 Posted by: Eboosted Posted at: 2019-04-16T22:39:04.808Z Reads: 40

```
Are you sure the red arrow is negative?

![image|476x500](upload://11vG08gbSWLR0OoIztPhIqRjFwN.jpeg) 

The center is usually positive and the external part is negative, use a multimeter to find out
```

---
## \#27 Posted by: danepoostain Posted at: 2019-04-16T23:08:15.861Z Reads: 39

```
ok i will try that. jthanks man youve been a huge help
```

---
