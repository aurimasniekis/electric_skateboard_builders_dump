# Do FocBoxes suffer from DRV failure?

### Replies: 9 Views: 462

## \#1 Posted by: kuphjr Posted at: 2017-09-17T23:24:15.509Z Reads: 117

```
I just blew my 3rd VESC in a row due to DRV failure.  I am pretty upset and I don't want to buy another piece of garbage that is just going to fail after 15-20 miles again.

I am thinking of just buying FOCBOXs, but I need to know if they will have the same issue.  If they do, I am just going to sell my board because I cannot afford to keep replacing these crappy electronics.

I bought all my VESCs from DIY Electric Skateboards if anyone is wondering.
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-09-17T23:27:12.814Z Reads: 118

```
Can a focbox have a DRV failure, yes! However, they seem to hold up pretty well in FOC as long as your settings are correct.
```

---
## \#3 Posted by: kuphjr Posted at: 2017-09-17T23:28:59.112Z Reads: 116

```
Okay, I was also just reading another thread that says there is some kind of thermal shutoff on the FOCBOX that can help prevent these DRV issues.  Can anyone confirm if this is true?
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-09-17T23:31:45.049Z Reads: 114

```
Get the Ollin ESC from @chaka.  Handles FOC like a pro and if you manage to burn it up, you’ve got a 2 year warranty
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-09-17T23:41:25.716Z Reads: 109

```
[quote="kuphjr, post:3, topic:33369, full:true"]
Okay, I was also just reading another thread that says there is some kind of thermal shutoff on the FOCBOX that can help prevent these DRV issues.  Can anyone confirm if this is true?
[/quote]

The directfet on the FocBox are faster to react than the DRV, unlike the regular 4,12 where the mosfet where slower than the DRV, so on the FocBox the mosfet are just doing their job properly.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-09-17T23:45:53.556Z Reads: 105

```
I just gave all my FOCBOX a very hard time. I mean a really very very hard time. With multiple different motors. Changed firmware. Software errors during development of new features so that the motors acted like they will blow up each moment. Wrong parameters and shitloads of km (the one in my big 12S8P more than 2000km). 
But they never broke.

Of course everything can brake but i didn't find a way yet to do so.

My 4.12 VESC's did FOC for 12 km and then they failed and send me flying at 45 km/h.
```

---
## \#7 Posted by: flywithgriff Posted at: 2017-09-18T00:07:59.895Z Reads: 97

```
@scepterr has found a way to kill them
```

---
## \#8 Posted by: onepunchboard Posted at: 2017-09-18T00:13:27.412Z Reads: 93

```
some people say they hear a tick which cutt off power to vesc immidiately. which I didnt manage to push that far. But Im pushing 3300w for my single motor, which is quite a killer for esc and motor but still works. im also using foc 65k erpm again should kill original vesc. I also had some motor short. some even pushed up to 80+k on the road but never heard died.

for normal use I dont think it will fry
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-18T00:24:01.550Z Reads: 90

```
It's easy when you get a defective one 😋
```

---
