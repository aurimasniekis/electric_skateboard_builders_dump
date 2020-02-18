# Questions before purchasing VESC

### Replies: 11 Views: 2399

## \#1 Posted by: lilracerboi Posted at: 2016-02-20T03:15:25.502Z Reads: 183

```
So I am about to buy a VESC, but I have some uncertainties. I am of course going to buy no doubt, but does the VESC have a power switch like car ESCs do? I have the Hobbywing EZ-Run in my board and I have the switch mounted where I can flip it from the outside.

Are there any other things I should buy along with the VESC? Cables? Should I invest in an anti-spark system? I want to buy everything I need all at once so I don't have to wait for them in case I order later.

Last thing, how can I protect the VESC in my board? Could I use a bunch of foam or something?
```

---
## \#2 Posted by: lox897 Posted at: 2016-02-20T04:35:03.128Z Reads: 181

```
The VESC does not come with an on/off switch. You could make your own antispark key (search google, sl33py on endless sphere did a guide) or you could buy the switch from 

You don't need cables but you may need some connectors. (4mm Bullet for motor and XT60/XT90/HXT4mm for battery.

To protect the VESC: The ones from enertion and ollinboards come with heat shrink. Some other guys who have put protection can give some advice I'm sure.
```

---
## \#3 Posted by: evoheyax Posted at: 2016-02-20T04:35:08.164Z Reads: 174

```
The VESC does not have any power switch. You have many options for that. Some on here use cheap circut breakers from ebay to do the job, and the more professional looking solution is ollies power switch, but that is around quite pricey (around $70 USD). The bueaty though of this power switch is that it has an anti spark system.

And if you want to take all precuations, an anti spark switch is not a bad idea. My take of the vesc is that they are very easy to brake. Wrong settings, not using a regulated power supply to config the settings, ESD, short circuiting by not heat shrinking at least the capacitor board, if not the main board also, overheating, too high of a max current setting, are all issues I have seen others have.

About protection, heat shrinking is what I think a lot of people do, maybe with some Velcro or hot glue. If you want to do a through job, I bought this acoustic dampening pad off amazon that absorbs pretty much all road vibrations, protecting you electronics from damage due to vibrations. Foam could also work, but a little airflow may be best. You do want it to stay cool.

Overall, the VESC is the best of the best in terms of features, but be ready to do a lot of research, configuring, and overall, getting your hands dirty (figuratively, not literally), cause this is not like setting up an rc speed controller where is plug and play. You will need some time and patience to get the vesc working. However, you won't regret buying one once you do.
```

---
## \#4 Posted by: lilracerboi Posted at: 2016-02-20T05:42:52.058Z Reads: 151

```
Thanks for the advice! I'm currently using deans plugs for my setup. Would that be an issue? Should I switch connectors?

Regarding the switch, would this be the switch you (@evoheyax) mentioned? product/on-off-high-voltage-anti-spark-power-switch-2-14s/ 
I might actually get that since I don't know or am afraid to make my own circuit. I want to protect my VESC as much as possible.

I know what I'm going to get into when I get the VESC and I really can't wait to tinker with it. I know the BLDC Tool is identical on all OS's, but are there any differences between Windows and Linux? Any compatibility issues on Windows?
```

---
## \#5 Posted by: treenutter Posted at: 2016-02-20T06:11:30.790Z Reads: 141

```
@lilracerboi I like using Linux to configure VESC because I can run Vedder's commands and directly upload new firmware. Also easily update to the latest BLDC Tool. If you're using Windows or Mac you've got to wait for a port of the Linux version. It's not s problem. The Windows and MAc ports work very well.
```

---
## \#6 Posted by: evoheyax Posted at: 2016-02-20T06:15:13.669Z Reads: 136

```
I just update a v4.10 esc from enertion in the October batch from 1.14 to 2.15, which is the latest mac version of BLDC. Seems fine.

And yes, that's the power switch. Very good quality. I'm very pleased with mine.
```

---
## \#7 Posted by: lilracerboi Posted at: 2016-02-20T06:48:36.161Z Reads: 136

```
I'm going to be using my laptop for the BLDC Tool and I might just dual boot Linux on it just to experience Linux more. Haven't used it extensively so this'll be a good chance to do so.

Also looks like I'll be getting that power switch, though I will now need to get a bigger enclosure.
```

---
## \#8 Posted by: lox897 Posted at: 2016-02-20T09:46:15.422Z Reads: 131

```
Deans plugs should work fine. They may be a bit harder to solder.
```

---
## \#9 Posted by: elkick Posted at: 2016-02-20T14:40:23.783Z Reads: 125

```
Antispark with fuse:
<img src="/uploads/db1493/original/2X/5/5057600cb0d77813fb63a9e93b464e10c7eeecc6.jpeg" width="375" height="500">
```

---
## \#10 Posted by: paragon Posted at: 2016-02-21T06:38:28.514Z Reads: 106

```
More info please. :)
```

---
## \#11 Posted by: elkick Posted at: 2016-02-21T07:36:08.822Z Reads: 99

```
It's just Vedders anti spark PCB with an added fuse holder. The fuse sticks in there absolutely tight and won't move, it can be replaced but you have to pull it out with some force. No problems with vibrations at all.
```

---
