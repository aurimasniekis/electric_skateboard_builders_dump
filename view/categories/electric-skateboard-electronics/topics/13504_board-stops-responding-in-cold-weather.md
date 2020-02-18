# Board stops responding in cold weather

### Replies: 29 Views: 2819

## \#1 Posted by: Mrmoonlight Posted at: 2016-11-23T00:11:55.959Z Reads: 196

```
I've been trying to figure out where the source of the problem is, but now that the weather has cooled down a bit, my board has stopped responding. Remote looks connected and my lcd is still showing plenty of charge, but no response from my board until it warms up again. This happens pretty quick too. About 2 minutes into my ride and the temp is around 35F. Board rides just fine if it's 10 degrees warmer. 
 
Any suggestions on what components are most susceptible to cold? or has anyone else experienced anything similar?

Setup:
Space Cell 3
Ollin VESC
Bench Wheel Remote + Receiver
Carvon single V2 Hub
```

---
## \#2 Posted by: Namasaki Posted at: 2016-11-23T02:22:38.931Z Reads: 179

```
Are you putting your remote hand in your coat pocket while riding?
My ego remote use to disconnect if I put my hand in my pocket to keep warm.
Bluetooth remotes are touchy. 
You might try a different remote.
```

---
## \#3 Posted by: Mrmoonlight Posted at: 2016-11-23T03:21:20.523Z Reads: 170

```
I'm keeping the remote out and even threw it in the freezer for a few to see if the cold was causing the remote to cut out, but no dice. When I get back into the house, it takes a few minutes before the board will work again. Powering everything off and on makes no difference. Once it warms up a bit, it's like it never happened.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-11-23T03:44:49.619Z Reads: 160

```
Strange, never heard of this problem before.
Talk to @RunPlayBack 
He runs a setup very similar to yours and he rides in cold weather as well.
Although, he uses a different remote and receiver.
Maybe your receiver is getting too cold and malfunctioning.
```

---
## \#5 Posted by: Stevemk14ebr Posted at: 2016-11-23T04:07:16.445Z Reads: 152

```
That is odd, maybe it's a battery thing I know lipos don't like cold
```

---
## \#6 Posted by: Mrmoonlight Posted at: 2016-11-23T06:28:23.214Z Reads: 141

```
It's the SpaceCell 3 so the battery is LiNiCoMnP. Shouldn't have an issue with a little cold. 

@Namasaki 'm gonna start swapping parts and see what happens. Change my remote back to the Steez and see if there's any difference.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-11-23T12:29:04.047Z Reads: 132

```
Frankly, I can't even imagine going out and riding in 35F weather!
```

---
## \#8 Posted by: Smithster Posted at: 2016-11-23T14:06:43.792Z Reads: 127

```
Just did the conversion 

1 degree Centrigrade

Ohhh That's chilly :snowflake:
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-11-23T14:19:13.841Z Reads: 122

```
Sounds like a loose connection cable somewhere. In warm weather the connection is flexible and works; if it gets too cold a cable is too stiff to flex and loses connection.
Check everything and make sure to use some hotglue to get everything in. Perhaps the connector cable from receiver and vesc somewhere.
```

---
## \#10 Posted by: Mrmoonlight Posted at: 2017-01-06T18:59:39.503Z Reads: 104

```
UPDATE:
So I've been trying to figure this one out, but I need freezing temps so it's been taking awhile. Checked all my connections and swapped parts and I've pretty much narrowed it down to my VESC. The issue was happening every time I rode in sub freezing weather and after I swapped VESC's the problem disappeared. 

Anyone know of any VESC settings that affect how it performs in cold weather?
```

---
## \#11 Posted by: lox897 Posted at: 2017-01-06T21:39:32.959Z Reads: 96

```
Pretty sure there's temp limits for the FETS
```

---
## \#12 Posted by: mmaner Posted at: 2017-01-07T00:10:25.032Z Reads: 95

```
It's 24 degrees Fahrenheit in North Alabama today, been riding a little but had no issues with my MEB VESC or DIY VESC. I'd check the phase wire connections at the VESC to  to make sure they are not contracting with the cold.
```

---
## \#13 Posted by: Mrmoonlight Posted at: 2017-01-07T03:29:33.864Z Reads: 82

```
Checked and double checked all my VESC connections. Phase wires are solid. It's one of Chaka's VESC's so quality is top notch. Swapped it for my DIY VESC and everything works just fine below freezing.
```

---
## \#14 Posted by: mmaner Posted at: 2017-01-07T04:06:50.578Z Reads: 80

```
Sounds like a VESC issue, by process of elimination.  I don't know though, I would have guessed RX.
```

---
## \#15 Posted by: chaka Posted at: 2017-01-07T04:12:46.705Z Reads: 78

```
You can send it in and we can switch it out for a fresh unit. 

Thanks for taking the time to trouble shoot this yourself before contacting us.

Send me an email: jclark@ollinboardcompany.com
```

---
## \#16 Posted by: Mrmoonlight Posted at: 2017-01-07T04:38:53.608Z Reads: 75

```
Thanks!
I still want to test it a little more to be absolutely sure. I've been going over every piece and I realized I'm still using the same patch cables to my remote receiver whenever I used your VESC. For the DIY VESC, I used a different set. Gonna swap those and see if that could be the source.
```

---
## \#17 Posted by: lox897 Posted at: 2017-01-07T22:58:11.332Z Reads: 72

```
Could it be an issue with the temp sensor?
```

---
## \#18 Posted by: Mrmoonlight Posted at: 2017-01-12T15:38:22.626Z Reads: 66

```
Swapped the cable to my remote receiver and it seems like that was the issue! Not sure why, but once I swapped the patch cables, the issue went away. I've been skating in 25 degree weather with no problems. Everything else is the same.
```

---
## \#19 Posted by: chaka Posted at: 2017-01-12T16:08:04.463Z Reads: 65

```
This is good to hear! What type of connectors where you having trouble with?
```

---
## \#20 Posted by: Mrmoonlight Posted at: 2017-01-12T18:17:49.573Z Reads: 58

```
It was the 3 pin patch cable that came with the VESC that connects to the remote receiver. I swapped that out and my board hasn't cut out since.
```

---
## \#21 Posted by: chaka Posted at: 2017-01-12T23:03:57.987Z Reads: 52

```
Thanks for the feedback. We switched to soldering the 3 pin wires on our new version of the vesc. Soldered connections are always better when possible.
```

---
## \#22 Posted by: PXSS Posted at: 2017-01-12T23:11:10.393Z Reads: 50

```
I disagree. Most high end electronics and connectors use crimped contacts for a reason. Of course if you dont you a high quality crimper and stripper, your connections are going to be subpar and susceptible to vibrations and stresses
```

---
## \#23 Posted by: chaka Posted at: 2017-01-12T23:19:35.509Z Reads: 53

```
Non soldered connections always produce more resistance than their soldered counterparts. This is fairly common knowledge.

Another bit of "not so common knowledge" is connectors are usually only good for one connection. Once you pull the connector and reconnect you have lost some compression at the point of contact. Not all connectors behave in this manner. But most small connectors, jst ect.... , are comprimised after several connection cycles.
```

---
## \#24 Posted by: PXSS Posted at: 2017-01-12T23:51:26.063Z Reads: 49

```
Sorry but no. 

"While most people assume a "crimp" is just a contact crushed onto a wire, giving electrical conductivity by means of pressure, real crimping involves "elastic" and "plastic" deformation and flow of metals resulting in "micro cold welds" due to "contact asperity welding" of the metal surfaces. During the deformation process the wire and connector are mechanically cleaned, usually making pre-cleaning of wire and terminal unnecessary. When done right, this crimped connection can be much stronger and longer lasting than a soldered connection, and have electrical resistance of the equivalent length of wire. A properly done crimp is also gas-tight as well, not allowing oxidation to degrade it over time."

This all assumes that you are using the right housing, contact, wire size and crimper tool. The tools requred to do these kind of crimps run in the thousands of dollars for handheld crimpers that work with a specific die made for a specific contact. Big industrial crimping machines run in the tens of thousands of dollars. 

I know because the place I work at owns several handheld crimpers to make such connectons and I bet you my crimped JST-XH/SH/ZH/PA connector lasts longer and has lower resistance than any of your soldered ones. 

As far as your second point goes. Connectors usually have a connection cycle rating based on a properly done crimp.
```

---
## \#25 Posted by: chaka Posted at: 2017-01-13T00:35:19.953Z Reads: 48

```
Well our crimper only cost around 500 dollars so you have me beat.

We are now soldering directly to the pcb so I have a hard time believing a jst connector is better at this point of contact.
```

---
## \#26 Posted by: PXSS Posted at: 2017-01-13T01:58:16.521Z Reads: 45

```
You're soldering the wire directly to the PCB? Yes, as long as your pad or through hole is larger than the contact area of the JST header, the resistance at that point is lower!

There are pros and cons to that too though. It's a permanent connection, you can strain the solder joint unless you add strain relief, if the wire gets damaged you need to desolder it and resolder a new one on, etc. In the case of the OP, if the wire was soldered on to the VESC then he would have not been able to troubleshoot the cable without desoldering and possibly voiding his warranty or shipping it back to you!
```

---
## \#27 Posted by: chaka Posted at: 2017-01-13T02:17:14.855Z Reads: 44

```
Pretty hard to void our warranty... Either way we are happy @Mrmoonlight was able to find the issue and   resolve it. :v:
```

---
## \#28 Posted by: Mrmoonlight Posted at: 2017-01-13T06:10:16.070Z Reads: 34

```
So far, I haven't had any issues with the performance of my soldered connections. Plus it sounds like dropping a ton of cash on a crimper would be a bit of overkill. 

Overall, I'm just happy my board works!
```

---
## \#29 Posted by: PXSS Posted at: 2017-01-13T06:41:14.499Z Reads: 32

```
I'm not saying soldered connections are bad! They're great for hobby stuff, I did it for years! But a properly crimped connector is better.
```

---
