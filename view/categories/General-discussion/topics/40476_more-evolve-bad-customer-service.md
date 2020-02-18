# More Evolve Bad Customer Service

### Replies: 39 Views: 2255

## \#1 Posted by: darkkevind Posted at: 2017-12-08T22:14:22.457Z Reads: 276

```
Just thought I'd share my recent disappointing experience with Evolve UK's customer service...

Think twice before being sucked in and conned guys...

http://kevindark.co.uk/Blog/Read/11
```

---
## \#2 Posted by: 12meterkuk Posted at: 2017-12-08T22:18:21.035Z Reads: 277

```
Although it sounds bad but this is really the norm for big esk8 companies... I don't think boosted or inboard would send u a separate bms.

The only difference is those companies actually have pretty good warranty and repair services
```

---
## \#3 Posted by: Mikenopolis Posted at: 2017-12-08T22:34:55.048Z Reads: 276

```
How is it that you have seven blown BMS Evolve boards? that seems like a high number of specific failure...I always thought their batteries were the weakest link, now it seems like their BMS a bigger issue.

Evolve's replies doesn't seem that much like a "con" as you put it. More like a privately held service to ensure proper repairs. It is odd that they pulled to Franch site's BMS off the shop though.

Please educate me as to what's so special about Evolve's BMS that requires them to be proprietary or is it just a form factor? If so can their their heat sink area/opening be modified as a workaround?
```

---
## \#4 Posted by: darkkevind Posted at: 2017-12-08T23:15:36.224Z Reads: 253

```
Cheap components basically...

The only thing special about the BMS is that it talks to the evolve ESC through UART to give voltage level, individual cell level etc. to the controller, oh and it won't turn on without it...

If people weren't bothered about those features and it would actually turn on I could use any old 10s 60A BMS.
```

---
## \#5 Posted by: b264 Posted at: 2017-12-08T23:21:23.048Z Reads: 243

```
The BMS unlocks the motor controller.
```

---
## \#6 Posted by: saul Posted at: 2017-12-08T23:25:23.792Z Reads: 233

```
[quote="darkkevind, post:4, topic:40476"]
ESC through UART
[/quote]

lets just trick the esc then....
you'll probably need a working one to sniff out the protocol. 
but really thats more work than its worth because you're still giving people an excuse to buy an overpriced pos.

The only good thing they have is the trucks, the rest is pretty disappointing...
```

---
## \#7 Posted by: Mikenopolis Posted at: 2017-12-08T23:29:42.198Z Reads: 221

```
[quote="b264, post:5, topic:40476"]
BMS unlocks the motor controller
[/quote]
[quote="darkkevind, post:4, topic:40476"]
it won't turn on without it
[/quote]


**That's just evil**
```

---
## \#8 Posted by: darkkevind Posted at: 2017-12-08T23:37:38.298Z Reads: 215

```
Oh and surprise surprise! I've been banned from the Evolve Facebook group!! 🤣😂
```

---
## \#9 Posted by: b264 Posted at: 2017-12-08T23:39:10.249Z Reads: 217

```
http://www.electric-skateboard.builders/t/im-an-outlaw-burn-noticed-a-fugitive-from-a-facebook-group/35452 @longhairedboy
```

---
## \#10 Posted by: SilentException Posted at: 2017-12-09T00:10:49.273Z Reads: 211

```
Honestly, I can see the both sides of this. On one hand, they suck donkey balls but on other, if you manage to make a mistake on wiring, soldering, something that might maker pack ignite or worse it comes down boiling on Evolve boards. But being a builder, I will stand on your side :)
```

---
## \#11 Posted by: darkkevind Posted at: 2017-12-09T00:59:20.739Z Reads: 200

```
But why if it's been modified would it fall on Evolve?

You don't stick a cosworth lump in a Cinquecento then moan at fiat when it didn't stop on stock brakes and ploughs in to something.... :confused:
```

---
## \#12 Posted by: SilentException Posted at: 2017-12-09T01:06:08.107Z Reads: 195

```
I didn't mean it in a way that the customer would complain to Evolve. Just simple, because
Evolve board caught fire
is a better headline than
Electric skateboard cought fire because of modified battery pack :)
```

---
## \#13 Posted by: benjammin Posted at: 2017-12-09T04:18:13.015Z Reads: 183

```
Customer service has been solid here in the states. 

Kinda understand where they're coming from. If I designed something that could potentially burst into flames, causing serious injury, I'd probably do my best to discourage costomers from doing their own modifications as well.
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-12-09T04:50:15.883Z Reads: 180

```
stateside they'll work with your customer prior to modding for a fee. Not through you. I did it oncem, they caught on to what i was doing, and then sort of cut me off. 

what you have to do is make sure nothing is wrong prior to modding it. Get the customer to get evolve to fix anything before you go in there, and be dead precise in what you do in there. 

so far so good. I've had a couple minor problems but i resolved them.
```

---
## \#15 Posted by: koralle Posted at: 2017-12-09T04:57:35.363Z Reads: 175

```
Esk8 companies should be held to higher standards than your average lame tech giant. That being said,  I don't know any company besides fairphone that really sells a range of original replacement parts at a reasonable price in order for customers to repair their out of warranty products. This is just something that doesn't make sense for them from an economic standpoint apparently.
```

---
## \#16 Posted by: Fiori Posted at: 2017-12-09T06:00:15.813Z Reads: 170

```
I think it's terrible that evolve threatened litigation...Iv'e known Evolve was a shitty company since the first contact I had with them. They will refuse to admit defects at all costs. Their 'repair experts' are a joke. 

But, we are  a DIY community. We need to ALL get together and work on creating some type of arduino unit to trick the evolve ESC so we can just skip dealing with evolve all together.
```

---
## \#17 Posted by: Rutherford Posted at: 2017-12-09T13:18:33.697Z Reads: 162

```
What microcontroller do they use? Since UART is enabled it would likely be possible to grab the firmware and examine it to find the handshake with the BMS. Then one could modify the firmware to not require the handshake and reload it to the board. Could make a tool that does it automatically once it's known, but you will lose the protection of checking that the BMS is there.
```

---
## \#18 Posted by: darkkevind Posted at: 2017-12-09T13:35:27.593Z Reads: 158

```
I honestly don't know :confused:

I've got someone I'm in contact with attempting to decode everything at the moment... Hopefully they'll come up with something, but your idea of amending the firmware sounds promising! :thumbsup:
```

---
## \#19 Posted by: Rutherford Posted at: 2017-12-09T20:26:18.050Z Reads: 152

```
Good luck with it, hopefully there is a simple solution. It's possible that the BMS and ESC are paired by evolve so it won't even run with a different official one, has anybody swapped one of these before?
```

---
## \#20 Posted by: Exiledd_Top Posted at: 2017-12-09T22:08:22.063Z Reads: 152

```
But if that's the case there's bin several threads about people replacing the lipos In the evolve and going 18650 cells in there soooo that would be confusing to that statement
```

---
## \#21 Posted by: myreala Posted at: 2017-12-09T22:23:20.533Z Reads: 144

```
They can be swapped so they are not paired just the UART communication is missing. As long as we can fake that it could also work out.
```

---
## \#22 Posted by: pat.speed Posted at: 2017-12-09T22:30:02.031Z Reads: 138

```
I thought evolve ran liions in their boards? Something like prismatic cells. 

Sorry for off topic
```

---
## \#23 Posted by: darkkevind Posted at: 2017-12-09T23:29:29.254Z Reads: 137

```
Yeah they're prismatic pouches...
```

---
## \#24 Posted by: Rutherford Posted at: 2017-12-10T00:10:45.679Z Reads: 134

```
That's good, it's not as problematic as it could be then. Looks like either spoofing the UART or modifying the firmware should work fine. Just needs someone with a working BMS to investigate :slight_smile:
```

---
## \#25 Posted by: saul Posted at: 2017-12-10T10:06:40.229Z Reads: 128

```
it looks like evolve uk tech team is one person, maybe you should just go in there directly. i see alot of spare parts :sunglasses:

https://youtu.be/Faf1KKEZhVc?t=3m42s
```

---
## \#26 Posted by: b264 Posted at: 2017-12-10T11:06:59.722Z Reads: 126

```
[quote="Rutherford, post:17, topic:40476"]
Since UART is enabled it would likely be possible to grab the firmware and examine it to find the handshake with the BMS. Then one could modify the firmware to not require the handshake and reload it to the board. Could make a tool that does it automatically once it's known, but you will lose the protection of checking that the BMS is there.
[/quote]

It's not an "unlock handshake" it's constantly transmitting the current battery level, which gets sent on to the remote.  The problem comes in with their feature of automatically switching to ECO mode at 5% battery..... if this UART connection is not made, it's sending 0% battery life to be displayed on the remote, which causes the remote to automatically switch the ESC into ECO mode.  It's entirely possible the offending lines of code are actually in the remote, but fixing it here would still mean you had a broken board battery gauge.  So really it's the sending of current voltage via UART from BMS to ESC that needs to be emulated

So you can put ANY bms on it you want, and it will work --- IN ECO MODE the whole time, which is 25% max power
```

---
## \#27 Posted by: skywalk3r Posted at: 2017-12-10T12:59:42.737Z Reads: 117

```
Replace Evolves ESC with a couple VESCs and just get your own remote. Problem solved :wink:
```

---
## \#28 Posted by: darkkevind Posted at: 2017-12-10T13:08:16.388Z Reads: 117

```
That _is_ the best solution....
```

---
## \#29 Posted by: Rutherford Posted at: 2017-12-10T14:37:32.463Z Reads: 113

```
Seems like it wasn't an intentional effort to prevent fitting a different BMS then. I would either make something to send voltage data to the ESC as normal or change the firmware so that the eco mode settings are the same as the normal settings in this case. Hopefully somebody sorts some solution
```

---
## \#30 Posted by: Rutherford Posted at: 2017-12-10T14:42:21.444Z Reads: 114

```
I suspect I could make a receiver for the original remote, but I don't have one to hand so can't say for sure. I assume they are 2.4GHz? I personally thought the travel on the throttle is too short on those remotes to be comfortable when I tried one, so maybe a replacement is an advantage.
```

---
## \#31 Posted by: TONY888 Posted at: 2017-12-10T15:36:42.728Z Reads: 110

```
Yes，the BMS are paired with ESC！Don't swap them！I tried to swap my boosted v1 controller to another boosted v1 battery，didn't work！then I swaped back，it won't work anymore，boosted firmware are highly encrypted. IDK why evolve has to copycat that too since their software&controller are not that good to be copied，maybe they should put more attention to developing their software instead of encrypt it.
```

---
## \#32 Posted by: darkkevind Posted at: 2017-12-10T17:13:04.750Z Reads: 104

```
I really don't think the BMS is paired with anything or encrypted to the ESC etc. I've made up 18650 packs before, using spare BMS' and installed in to a BGT and all worked perfectly.

It literally is just a handshake between the ESC and BMS. It might even be the case that you could connect one or more of the wires together to fool it...:/
```

---
## \#33 Posted by: b264 Posted at: 2017-12-10T20:28:24.265Z Reads: 101

```
The ESC is not paired to the BMS, because I've changed it.  To re-pair the remote to any Evole GT ESC in range, hold the left remote button down...
```

---
## \#34 Posted by: Fiori Posted at: 2017-12-12T07:41:07.606Z Reads: 95

```
@mwkeefer Had posted on another topic about a module he had working to trick the esc. Any input?
```

---
## \#35 Posted by: Vanarian Posted at: 2017-12-12T13:49:32.794Z Reads: 89

```
Duh, the force ECO mode upon 5% left battery is dumb as shit.

Riders need safety features foolproof and honest after sale services, not babysitting. 

BTW Evolve can't take direct actions against any individual modifying a board apart from breaking warranty and Evolve's liability. 

Once sold the customer buys all the ownership rights on it without reserve, apart from patent protections (which doesn't concern us here) nothing can be done. 

A clause forcing customer to keep coming back to the manufacturer with different consequences than warranty breaking or Evolve's refusal to further take in charge the product for repair is anyway illegal and will easily be canceled if it goes in a court.

That's basic property rights, how come they even think about threatening you. 

How about they eat shit?
```

---
## \#36 Posted by: darkkevind Posted at: 2017-12-12T13:53:14.666Z Reads: 85

```
I know, exactly what I said. You buy the board it's yours to do with what you wish. You wanna strap a rocket to it, no one can stop you....
```

---
## \#37 Posted by: egzplicit Posted at: 2017-12-12T18:06:34.673Z Reads: 82

```
[quote="darkkevind, post:36, topic:40476"]
You wanna strap a rocket to it,
[/quote]

How much kv is that? Will my vesc fry?
```

---
## \#38 Posted by: darkkevind Posted at: 2017-12-12T22:03:39.957Z Reads: 79

```
I believe 20000kv! ;)
```

---
## \#39 Posted by: Vanarian Posted at: 2017-12-16T18:10:12.275Z Reads: 71

```
Over 9000 !!
```

---
