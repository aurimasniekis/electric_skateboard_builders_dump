# New Build HELP! No Lights on VESC and Cannot Read Firmware msg is all I get!

### Replies: 4 Views: 72

## \#1 Posted by: weednwheels Posted at: 2020-02-02T21:48:01.204Z Reads: 17

```
Hi Peeps,
I'm a 50 year old Skater/DH Longboarder that hated the idea of walking uphill more than an Eboard so last year I bought both a Raptor and Halo Board to ride uphill and than Bomb/Freeride the hills.  Not knowing a thing about Eboards I went with in-hub designs so I would have more of a free wheel feel...It didn't work to well as fast freeride 90 ft stand up slides rattled the Sh## out of everything and the performance was only mediocre compared to my Rayne setups with precision trucks and RAD (Rider Approved Designs, my go to for Fast Freeride but not compatible with either Kegel or Abec cores).  BUT something happened, I got Eboard addicted once I embraced the difference!  So I ditched trying to make an eboard that freerides like my quiver and decided to build a Trampa Mountainboard to slay the unlimited trail riding I have living in the Sonoran Dessert (Arizona) and our  300+ days of sunshine....OH LORD WHAT DID I GET MYSELF INTO!!!  I'm a pro skater NOT a DIY type at all (at least the electric side of it).  

**I've been trying for 3 weeks to get the board running and have used the search feature here before just posting this for help, I've really tried guys but alas I 'm stuck, FRUSTRATED and just want to RIDE!**

So here's the deal.  Being a poor broke ass skater I couldn't just order a pre-built Trampa so I decided to use as much as I could from Trampa minus all electronics and DIY the wiring harness (no monster box or the like) VESC, Remote and motors.  I went with Dual Torque Board 6380's and nano remote, Dual Turnigy 8 AH graphene Lipos in Series for 12S and 2 Flipsky  4.12 FESC.  My problem started (and I suspect ends) with my complete EPIC FAIL trying to solder a wiring harness with XT90's using Super Worm 8ga wire.  I've never soldered a day in my life and the 8 GA made it difficult but the real problem was using really thin solder that came with my beginning solder kit, you know the stuff that is really thin and burns off before you can dab it anywhere.  I burned ALL 10 XT90's trying to make a battery side cable to run from the middle of the board (batts) to the rear kick where I mounted a box with the Flipskys in it. After destroying all but one xt90 which I put on the batt side into a Serial xt90 connector, I was able to solder bullet connectors to the power side of the VESC and battery cables.  So it goes Batteries---XT90 to Series XT90 ---to 5.5mm Bullets with the hot side (red) going into a reset able 200 AMP in line fuse (water proof car audio type) out to dual Bullets to connect parallel into VESC and same on Neg (black) without the fuse box in between.     Additionally I have no PC so also installed a Flipsky BT module to configure motors.  

When I turned it on I never got any lights but the BT module and Remote module both were gettting power.  However i could not see the Vesc at all using the Android VESC Tool until after hours (maybe days) of reading here I did rewire the BT module as recommended in another thread (move the VIN pin from the factory setting which had it wired in the 5.5v input) and I could SEE the BT module now.  I was stoked, I'll be riding in an hour.....nope!  All I got was a temp connection via BT then it would drop and say "Cannot read Firmware, check the port on VESC . . . ".  Figured it was my wiring so I bought a amp meter and ran down 3 bad bullet connector (my fault).  Re soldered everything and got all the same as above.  Figured I blew a chip as the comm and remote busses had power but no firmware found.  Returned VESC's (bought on Amazon Prime so easy returns) which meant re soldering all 10 bullets (2 red/ 2 Black on batt side and 6 on motor side) hooked back up and got FLASHING LIGHTS on VESC's!!!! I'll be running down Road Runners in the Desert in an hourt!!! NOPE.  One bullet came loose and bam...no lights again and back to "cannot read firmware" msg!!!!!!!!  UUGGGGGGGGGGHHHH!  After punching a few holes in the walls and making up cuss words so loud my police trained Husky Belgium Malinois refused to come (which pissed me off even more, at myself mind you for such an ugly display of frustration), my wife was hiding too but she'll get over it, I threw her some kibble and gave my boy a steak and we are all good again (well at least he and I are the wife is still not speaking to me but thats ok).

So all week I've been trying to figure if I blew the cards (again) and need to start from scratch (again) with better wiring or am I missing something regarding Firmware msg?  Read a lot here and on Vedders site but regarding setup via BT module alone I just can't get an answer.  I cannot at this time set up via USB without buying a computer and Flashing fimware via ST Link (whatever that is) seems like another frustrating rout IF the VESC are blown anyhow and need replacing?????

Any help guys would be GREAT.  I honestly tried to do my own research before just throwing up this SOS!  Help me before I lose my great relationship with my dog for being the frustrated ASS I have been for 3 weeks, the Wifey will just have to deal and will leave me if she ever reads this anyhow....more ride time for me and my dog if that happens (kidding, she 's great most of the time but a dog is great ALL the time).
Thanks in advance...Ricstrong text
```

---
## \#2 Posted by: Secco Posted at: 2020-02-03T09:03:13.829Z Reads: 10

```
I'm newb and do not use BT connection yet so I'm not put my word on here and wait for more experienced ones to chime in.. but i'm following with interest. I've blown a dual Flipsky 4.2 and 3 single Flipsky 4.12 (out of 4) so I wish i knew more of the reasons behind the failure.
```

---
## \#3 Posted by: weednwheels Posted at: 2020-02-03T20:01:02.977Z Reads: 9

```
Thanks Secco for the response...I am 4 for 4 blown (if that is truly the case) on the Flipsky 4.12 Singles but in know way am willing to say its Flipskys' fault.  My own bad wiring is probably to blame but as we are both noobs here MAYBE not.  I've been stalking this forum for over a year and have to say there is a real community willing to help us noobs so if we are both a little patient someone should come along soon and shed some light on it for us.
```

---
## \#4 Posted by: Skyart15 Posted at: 2020-02-03T20:20:36.575Z Reads: 7

```
You may want to head over to  forum, more people there that will be able to help
```

---
