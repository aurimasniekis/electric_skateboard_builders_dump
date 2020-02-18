# Blu-Ya &#124; Haya Deck &#124; Dual FSESC 6.6 &#124; DieBieMS &#124; 12S4P Samsung 30Q &#124; Metr Pro &#124; Photon Remote

### Replies: 10 Views: 492

## \#1 Posted by: MiniChopper4Me Posted at: 2019-06-02T23:10:30.162Z Reads: 159

```
I'm sick and tired of being a buyer of parts and desperate to join the completed build club.  However, I'm physically unable to overlook the most meaningless of details, and so I'm surprised I've made it this far.  While the title says it all, I'll summarize the components for those interested:
1) Haya deck (#8, for anyone who gives a shit)
2) 2x Flipsky ESC 6.6, with heatsinks
3) DieBieMS, batch 3, goddamn this thing has alot of connectors.
4) Metr Pro, although I don't know that a basic model exists.
5) Photon Remote, although I have a Hoyt St. puck waiting to take its place when (if) it gives me problems.
6) 48 Samsung 30Qs, arranged in the "I'm bored of this position but its better than not getting laid" classic 12S4P arrangement.
7) 2x 6354 sensored motors from BKB (thanks again @JLabs !)
8) Janux Motor mounts for Caliber, silver (@marcmt88, you're the shit!)
9) Caliber trucks, 10" 50degree trucks, raw finish
10) Caguama Blue 85mm, 77a durometer wheels
11) Plastic 3D printed parts, provided by the Angel of ESK8, none other than @mmaner himself
12) Time, lots of it, and tools, alot of which I'll probably never need again unless god forbid one of my retarded nephews decides to crash my shit and force me to fix it (even if I crash it, they'll catch the blame I tell you)

On to pictures, f text AND pushing:
![image|375x500](upload://tI6NzUoUm7bO1vNN2fACoVAN29X.jpeg) ![image|375x500](upload://5BSQoTsQ7mjrO8puW4aUpilog4Z.jpeg) ![image|375x500](upload://cxyTF1nuUhCO8gQhgtg5Hj5VIFF.jpeg) ![image|375x500](upload://ihegLNpXPf5i45pHT0EFv4ZtXBg.jpeg) ![image|375x500](upload://1PTIhGclKzEAXp4XXjanoMYQyj2.jpeg) ![image|375x500](upload://iOFVCRhmlkdJnov6XBjZGk304V0.jpeg) ![image|375x500](upload://4D3tzJGUxuxOf85QEzH2mwFSJg9.jpeg) ![image|666x500](upload://7hzRWGxEhZ26mum27MfdyPvLTkO.jpeg) ![image|375x500](upload://7uPgJe4bO84nQYf1xx0RckAXwFb.jpeg)
```

---
## \#2 Posted by: MiniChopper4Me Posted at: 2019-06-02T23:23:25.984Z Reads: 145

```
I said to @mmaner once, "there's no way you can build an esk8 in one night." He responded with "its possible, you just need to have gotten all the necessary parts from China already."

With all of the duct-tape builds I've seen in the little time I've been trolling the forums, I have no doubt you can finish a build in one night, but you really have to learn to let the details slide.  Unfortunately, I can't.  The 90 degree turns with the wires alone were probably 30-60 minutes each, and holy shit are they annoying to make.

I'm staring down the second half of the battery pack  that still needs its balance leads attached and heatshrink wrapping to make it purty, but a glass of rye whiskey really made me think, or better said stop thinking.

So the project goes on.  Maybe another weekend, maybe 2.  I love how it looks , even though I posted the pictures all out of order :smiley:
```

---
## \#3 Posted by: MiniChopper4Me Posted at: 2019-06-02T23:47:12.216Z Reads: 131

```
Pictures fixed, but what's left to do:
1) Finish battery balance leads
2) Wrap up the second half of the battery
3) Make a custom CAN-BUS cable for both ESCs and the DieBieMS
4) Sand down one of the belt tensioners, it rubs like a sumbitch
5) Update and program the shit out of 5 components
6) Add a coat of varnish and seal the bejeezus out of the entire assembly with epoxy
7) Ride this mofo on the 4th of July
```

---
## \#4 Posted by: Flasher Posted at: 2019-06-03T00:41:56.644Z Reads: 119

```
Nice build. One question: you're not the first I see adding a cable over the nickel tab....what's it for?![received_2809321399139657|375x500](upload://9T3yyXjftXBlHD8VZpzRoA86Yvd.jpeg)
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-06-03T02:07:45.827Z Reads: 110

```
For parallel connections It is not needed...

But it's for current reinforcement, as just the nickel itself might not be able to handle the current
```

---
## \#6 Posted by: Flasher Posted at: 2019-06-03T02:31:31.070Z Reads: 107

```
 @AlanZhou  So I shouldn't worry about my build? About to solder a 12s8p with crisscross tabs![Screenshot_20190602-222943~2|690x456](upload://lGYgQ9Pv2P8EJkjBdSYUL8Sf6eY.png)
```

---
## \#7 Posted by: MiniChopper4Me Posted at: 2019-06-03T03:57:25.902Z Reads: 102

```
Depends on what your expectations for power output are.  I don't know what cells you're using but in the case of 30Qs, the max constant output would be 8*15A=120A,  I would worry that that much current would melt those tabs in series.  This is the purpose of the stranded cable in series.

Some people opt to use a whole sheet instead of tabs.  Adds ampacity that way.  Or just use a few 12AWG stranded jumpers instead like everyone else.
```

---
## \#8 Posted by: Tinp123 Posted at: 2019-06-03T07:26:53.281Z Reads: 100

```
In case there is no additional wire, amps from two bottom batteries would go through nickel, and in one place on nickel there would flow 40 amps, which is a little bit too much for this thin, narrow nickel. instead of wire, one or two more layers of nickel could be used. 12awg wire in this case is overkill. 

![0ce007fcb32891820fb40784714ada72a3741dc4|375x500](upload://faL2LA4lAEVW5WFtLmNc2QJCGXO.jpeg) 

@Flasher if you have nickel in series connection between each cell like on your photo, you don't have to worry, that is enough. you will probably never draw 120 amps, and even if you do, it would be divided on 8 strips in series connection, for very short period of time. you will have to take care when connecting main positive and negative wires, because all amps will flow through that spot on nickel, where wire is soldered. you could solve that with few layers of nickel, braided copper wire, or just soldering main positive and negative wires over all lenght of nickel strip that connect batteries in parallel.
```

---
## \#9 Posted by: MiniChopper4Me Posted at: 2019-06-10T18:58:49.723Z Reads: 72

```
Waiting on my second Flipsky 6.6 to get back from Canada (thanks again, @JohnnyMeduse) so I can put everything back together and get this puppy rollin'!

Unfortunately I found out too late that I got a defective one in my Black Friday purchase from October 18 (check your equips before the warranty expires fellas!), although dealing with Johnny beats dealing with Flipsky any day of the week.

I also sent the Photon back for repairs to @Wajdi, hopefully I can still use it on this build, although I have a Hoyt St. puck just itchin' to take its place.

The DieBieMS, Metr Pro, and first Flipsky 6.6 are all updated and working together beautifully!
```

---
## \#10 Posted by: MiniChopper4Me Posted at: 2019-08-16T01:38:39.356Z Reads: 50

```
Let's see:
1. Flipsky 6.6 came back from @JohnnyMeduse and is working perfectly now.  Thankfully I didn't have to redo the 90degree power plug for it.  Whee! Thanks JF!
2. The Photon was a bust.  Even though I got it to work, it was doing crazy stuff when you would touch the antenna on the remote.  I gave up and went with the Hoyt St. puck.
4. After riding around on it for a few test rides and such, I opened it back up to double check everything is sitting tight and such.  The battery rattled around with vibrations from striking the wood bottom so I decided to cover the inside compartment with 1mm thick neoprene foam.  I also added another sheet of fishpaper to sit between the top cover and the battery, since I found spots where the foam had been rubbed away, and the last thing I want is a short. I packed all the components in with foam to keep them from being able to move around, fishpaper and krylon taped the hell out of everything, and sealed the board back up.  My plan is to do some more riding on it and then, if everything holds up and looks a-ok, I'll seal up all the cavities in/out of the board with flex seal.  Takes a few applications/days, but it will definitely keep water out of the board.
5. Finally, I had to realign the mounts/belts etc because I never did that, and the result was all kinds of misalignment issues.  I took apart the entire Janux mount today, cleaned everything up, and made sure it was all square, evenly spaced, and loctited at the end.  One last modification I decided to go with was to replace @marcmt88 idlers with some hardware I ordered.  I didn't like the noise the tensioners make, and they are always grinding away with the shoulder screw and the mount itself.  I went with some other shoulder screws in stainless (my mounts and trucks are raw finish), 8mm x 16mm shoulder diameter/length, used 2 608 bearings on each in combination with a couple of speedrings between them, and an M6 washer at the base to put the bearings in proper alignment with my belts.  Its absolutely perfect and silent.

With the 2 VESCs and DieBieMS connected via CANBUS (custom cable complete), and the Metr Pro connected to the UART of VESC2, and the Puck receiver connected to VESC1 on PPM, everything works perfectly.  Metr Pro shows all the battery info correctly when I click on the battery %, and I can adjust settings on the fly.  Push to start is also enabled and working.

To do:
My last remaining micro-complaint is that the charge jacks I bought don't seem to interface well with my charger,  While both were supposed to be 5.5mm x 2.1mm, I suspect the input jack is actually 5.5mm x 2.5mm.  I bought some adapters off eBay, and it it turns out to be the case, I may just order the correct jacks (again) and replace the culprit.
```

---
