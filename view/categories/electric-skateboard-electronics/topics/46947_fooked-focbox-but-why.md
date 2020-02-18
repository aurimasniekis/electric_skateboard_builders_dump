# Fooked FocBox &hellip; . but why?

### Replies: 20 Views: 1364

## \#1 Posted by: ducktaperules Posted at: 2018-02-20T13:33:41.049Z Reads: 260

```
So i have been running dual setup on my board for a while now no problems until this morning. Feel one motor cut out on the way to work. I stop at side of road to check things out. Seems to be working intermittently. decide its best to disconnect power and motor cables and carry on to work with just one motor.

At lunch i remove focbox . . . . quite sure i can smell something odd. take case off and im greeted with this :

![IMG_20180220_130634|666x500](upload://eIebQeMdcSZ8YqgfGl2rZ4VpOde.jpg)

looks like something somewhere has shorted. It seems like the caps that go to the first wire are damaged as well as the trace on the left side of them.

There was also some loose pieces of ferrite in the case. my best guess is that some pieces broke off the inductor ant touched something they shouldn't have have.



**Is it possible that broken ferrite could have caused this damage?**

**If caused by the ferrite, would it be covered under warranty?**

**If not has anyone else had a similar failure?**

**Is there any way to fix the damage?**
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-02-20T13:46:10.975Z Reads: 249

```
Hi There 

Please email to support of Enertion board with the complete details and image evidence of your problem. 
Support email is support@enertionboards.com, don't forget to provide your order ID.
```

---
## \#3 Posted by: ducktaperules Posted at: 2018-02-20T14:19:39.945Z Reads: 239

```
I purchased the focbox through street-wing.com so i dont have a direct order number but i have sent an email anyway.
```

---
## \#4 Posted by: SOICDIP Posted at: 2018-02-20T14:33:11.935Z Reads: 231

```
C102 has burned up, so I'm assuming one of the three capacitors have shorted out.

They can short  out themselves without anything physically touching them.
```

---
## \#5 Posted by: CarlCollins Posted at: 2018-02-20T14:33:28.621Z Reads: 225

```
Thank you so much! we will check what we can do for you
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-02-20T14:42:40.173Z Reads: 218

```
Ceramic capacitors can crack and then they basically are short. There are videos about it on EEVblog channel
 
https://youtu.be/Q2rvAoO-MIA

https://youtu.be/QgKY5QWehME
```

---
## \#7 Posted by: ducktaperules Posted at: 2018-02-20T14:58:40.582Z Reads: 209

```
if the fault is these capacitors (im assuming they are for suppressing motor noise) then would it run with the capacitors removed?
```

---
## \#8 Posted by: SOICDIP Posted at: 2018-02-20T15:12:12.971Z Reads: 200

```
[quote="ducktaperules, post:7, topic:46947, full:true"]
if the fault is these capacitors (im assuming they are for suppressing motor noise) then would it run with the capacitors removed?
[/quote]

They suppress voltage spikes, so it's not recommended.
```

---
## \#9 Posted by: Slak Posted at: 2018-02-20T15:16:07.574Z Reads: 200

```
I quote Jinra here : "They "close the gap" for the battery to provide the VESC additional 
power on demand. Your battery cables may not seem long, but they are for
 the VESC."

Source : http://www.electric-skateboard.builders/t/vesc-faq-how-many-capacitors-what-uf/6125/8?u=slak
```

---
## \#10 Posted by: Jc06505n Posted at: 2018-02-20T15:16:36.901Z Reads: 189

```
How does one prevent this?
```

---
## \#11 Posted by: SOICDIP Posted at: 2018-02-20T15:25:52.697Z Reads: 186

```
[quote="Jc06505n, post:10, topic:46947, full:true"]
How does one prevent this?
[/quote]

If the short is a result of cracking as Kug3lis pointed out, there's practically nothing we can do as customers. 
If it's a wrong valued part (low voltage etc) we can replace it ourselves, but I believe the three are 4.7uF 100V rated.
```

---
## \#12 Posted by: ducktaperules Posted at: 2018-02-20T16:08:03.313Z Reads: 174

```
Correct. on the schematics C102 C103 are 4.7uf 100V. 

looking at the schematic its tho i notice that they only have 2 caps per phase, the actual pcb seems to have an additional 4 caps that are not on the schematic. 2 phases have an extra cap in parallel and one phase has 2 extra caps in parallel.

seeing as all theses cap go to vbat on the other side would i be able to replace the caps and if the trace is damaged just run a wire from the other side to somewhere that is vbat? maybe the same side of the caps on another phase?

edit: 
e.g. like this ![8fd07bfc3d0223296fd088ecf561d91ec171223e|375x500](upload://kxZr1itlmJuXHb5GwjT3HtWcEoT.jpg)
```

---
## \#13 Posted by: SOICDIP Posted at: 2018-02-20T17:02:36.436Z Reads: 169

```
[quote="ducktaperules, post:12, topic:46947"]
would i be able to replace the caps and if the trace is damaged just run a wire from the other side to somewhere that is vbat?
[/quote]

Yeah, that should work. 

Double check the schematic before you plug the power on though.
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-02-20T17:48:15.133Z Reads: 155

```
I guess the problem was vibrations, the solution is to use rubber bushing to isolate it from the deck so vibrations would not go to the PCB. As vibrations can even break solder joints and etc. It causes most of the problem I guess in VESC problems with mystical damages.
```

---
## \#15 Posted by: Blitz Posted at: 2018-02-20T18:46:37.129Z Reads: 142

```
Hey Carl, What If this happened to a vesc-X from a group buy, would Enertions warranty cover non user error?
```

---
## \#16 Posted by: CarlCollins Posted at: 2018-02-20T20:10:45.062Z Reads: 127

```
If that customer bought the warranty as well then Enertion will cover it under warranty. 
If you are having this issue, please contact the original owner and ask him to contact Enertion support via email.
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-02-26T09:06:38.428Z Reads: 89

```
Replacement has been sent to the @ducktaperules 
I hope this will work smooth now. 
It's okay now to close this thread.
```

---
## \#18 Posted by: ducktaperules Posted at: 2018-02-26T10:06:48.751Z Reads: 73

```
@CarlCollins at Enertion and @DavidBanner at street-wing.com sorted this out for me. A nice shiny new FoxBox turned up here just 3 days after contacting Enertion support.

When you buy high quality products from a reliable known brands you also end up getting great customer service. These guys care about the community and helped me get back on the road as soon as possible.

Thanks :slight_smile:
```

---
## \#19 Posted by: CarlCollins Posted at: 2018-02-26T10:10:04.332Z Reads: 71

```
It's our pleasure
```

---
## \#20 Posted by: Skitzor Posted at: 2018-02-26T10:12:32.186Z Reads: 72

```
[quote="ducktaperules, post:1, topic:46947"]
decide its best to disconnect power and motor cables and carry on to work with just one motor.
[/quote]

A tip: Only do this if you confirm CAN cable and belt are also disconnected.

Happy it's solved !
```

---
