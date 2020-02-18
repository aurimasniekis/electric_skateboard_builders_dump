# Li Ion pack won&rsquo;t charge after a short

### Replies: 9 Views: 228

## \#1 Posted by: eparks11 Posted at: 2019-09-02T20:37:43.368Z Reads: 57

```
I'm wondering if someone can help me. My charge port got damaged, and when it did the center positive prong touched the negative and shorted out (creating quite a spark). I cut the damaged port off of my charge lead, and soldered a new one to my 10s2p lion pack. I just took my board out for a test ride and everything worked fine.

However, when I went to charge the pack, the red/green indicator on my charger is no longer turning red (red indicates it's charging). So I assume my pack isn't charging. I double checked all my connections, and they look solid, so I'm not quite sure what to test next.

Can someone give me advice on troubleshooting this?
```

---
## \#2 Posted by: clistpdx Posted at: 2019-09-02T20:56:17.435Z Reads: 56

```
Is your charger showing any color? Blinking green?
```

---
## \#3 Posted by: eparks11 Posted at: 2019-09-02T20:59:13.045Z Reads: 51

```
Just solid green.
```

---
## \#4 Posted by: eparks11 Posted at: 2019-09-02T21:03:51.298Z Reads: 53

```
Also, I checked the voltage on the pack. It’s at 37.1v.
```

---
## \#5 Posted by: Tinp123 Posted at: 2019-09-02T21:44:14.294Z Reads: 45

```
Happened to me on my old meepo battery. Bms went down. Probably your case too. I guess you have meepo/wowgo/ownboard 10s2p battery?

If you feel brave enough, you can remove heat shrink from battery and bypass bms. It is not safest option to ride without any sorf of bms, but it will work until you get new bms or new battery. Also, if you are going to open your battery and ride it with bms bypassed, don't forget to check every series groups voltage with multimeter after every few charges.
```

---
## \#6 Posted by: eparks11 Posted at: 2019-09-02T22:44:31.982Z Reads: 41

```
Was afraid of that. My 10s2p is from MBoards.co. I’ll reach out to him and see if he’ll sale me a replacement BMS. Was thinking about upgrading to a 10s3p anyway, guess now would be a reason to do it.
```

---
## \#7 Posted by: eparks11 Posted at: 2019-09-19T22:08:31.334Z Reads: 21

```
Well, the new BMS arrived, and I got it connected. The battery is registering 37v on the XT60 connector, but the battery still won't charge. I'm not really sure what to troubleshoot next. If anyone has any advice, I'd much appreciate it.

![IMG_6214|666x500](upload://CY0hvGQvhzwGP3eP5bIT1zp7kL.jpeg)
```

---
## \#8 Posted by: Santino Posted at: 2019-09-20T01:50:54.806Z Reads: 14

```
Did you check if the charger have a fuse? Maybe it is that...
```

---
## \#9 Posted by: eparks11 Posted at: 2019-09-20T03:15:41.310Z Reads: 12

```
Thanks for the response, but I have two chargers, tried both, and it doesn't charge with either of them, so I think I can probably rule that out.

At this point I'm thinking about just buying a Wowgo/Meepo/Backfire board. Plug the battery in from it, see if it works. If my board works after that, then great, I'll know it's just a damaged battery. I'll then attempt to remove the cells from this battery, and rebuild the battery all together using a kit. 

As a bonus, I'll have a functioning board to ride while my DIY board is in the shop..which it apparently will be most of the time :unamused:
```

---
