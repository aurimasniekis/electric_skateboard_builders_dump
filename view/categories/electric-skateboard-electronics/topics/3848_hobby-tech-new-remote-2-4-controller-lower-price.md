# Hobby tech New Remote 2.4 controller - lower price

### Replies: 28 Views: 3185

## \#1 Posted by: appelton Posted at: 2016-05-26T07:17:44.428Z Reads: 250

```
Guys, I just've noticed that Hobbytech have lowered the price for that small, nice looking remote. It used to be 99$ - now it is 69$ which makes a pretty good deal. 

http://www.aliexpress.com/item/New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32612820590.html?spm=2114.01010208.3.1.sKxHAC&ws_ab_test=searchweb201556_8,searchweb201602_1_10017_10021_507_10022_10020_10009_10008_10018_10019_101,searchweb201603_9&btsid=3e69d47b-cf5c-4b6e-b7e8-75877ac4ed9b
```

---
## \#2 Posted by: Maxid Posted at: 2016-05-26T07:22:47.059Z Reads: 249

```
Says "page can not be found"
```

---
## \#3 Posted by: magnetvox Posted at: 2016-05-26T07:24:46.922Z Reads: 240

```
Link works for me.
```

---
## \#4 Posted by: Maxid Posted at: 2016-05-26T07:25:30.537Z Reads: 229

```
Maybe because I am on mobile?
```

---
## \#5 Posted by: magnetvox Posted at: 2016-05-26T07:26:09.223Z Reads: 201

```
Should still work? Strange.
```

---
## \#6 Posted by: appelton Posted at: 2016-05-26T07:29:23.375Z Reads: 189

```
Hard to say , it works for me. It might be because of the mobile.
```

---
## \#7 Posted by: philipp Posted at: 2016-05-26T09:13:56.999Z Reads: 182

```
It has a "light" channel 2...
Does someone have an idea if this could be missused as a cruise control button?
I really do like the size of it and I'm missing the cruise control on my TB-Mini remote :smile:
```

---
## \#8 Posted by: makevoid Posted at: 2016-05-26T09:40:34.165Z Reads: 177

```
not very practical to reach for cruise control if you don't have a tiny thumb :D
```

---
## \#9 Posted by: Maxid Posted at: 2016-05-26T10:10:14.030Z Reads: 173

```
Are there any reviews of this remote? I can't find any information besides aliexpress
```

---
## \#10 Posted by: philipp Posted at: 2016-05-26T10:12:54.921Z Reads: 175

```
I wouldn't mind removing the switch and putting a clicky button to the front of the case and solder it to the channel 2.
But I dont know how the vesc needs to get the cruise control in order for it to work :\
```

---
## \#11 Posted by: Maxid Posted at: 2016-05-26T10:23:08.209Z Reads: 166

```
My guess is that cruise control happens inside the remote and just sends the initial potentiometer signal in a loop without you holding the actual potentiometer position.
Therefor it should be possible to retrofit any remote with a cruise control by putting a small Arduino in there that reads the potentiometer value once you click a button and then imitates the potentiometer signal.

This is just an idea though!

EDIT: like this maybe: [https://www.arduino.cc/en/Tutorial/DigitalPotentiometer](https://www.arduino.cc/en/Tutorial/DigitalPotentiometer)
```

---
## \#12 Posted by: makevoid Posted at: 2016-05-26T10:58:34.066Z Reads: 157

```
I have one of those, I like the compactness of it but it's not so precise as the trigger ones like the GT2 and the other one hobbytech is selling, so with the vesc incremental acceleration (that requires less precision because varies the acceleration incrementally instead of the instant acceleration) everything is ok, with a normal ESC it's "fine" but not optimal imho
```

---
## \#13 Posted by: philipp Posted at: 2016-05-26T11:16:44.526Z Reads: 148

```
Thanks for the info!
I hoped that the cruise-control logic is integrated in the vesc, because it would allow very simple remote designs...
```

---
## \#14 Posted by: Maxid Posted at: 2016-05-26T12:26:03.218Z Reads: 143

```
I don't have a VESC (yet) so can't tell you if that is the case. If so it would obviously be really cool.
```

---
## \#15 Posted by: lowGuido Posted at: 2016-05-26T12:59:48.555Z Reads: 142

```
does that remote have a receiver?
although for $69 i'd just buy a Kama..
```

---
## \#16 Posted by: lowGuido Posted at: 2016-05-26T13:01:41.524Z Reads: 138

```
what do you mean by [quote="makevoid, post:12, topic:3848"]
the vesc incremental acceleration
[/quote]
```

---
## \#17 Posted by: trbt555 Posted at: 2016-05-26T13:13:34.811Z Reads: 136

```
You guys need to distinguish *throttle preset* from *cruise control*.

**Throttle preset** is typically a functionality of the controller. The Enertion/Backfire controller offers throttle preset, which means the controller will just keep sending the same pulsewidth it was sending at the point you pressed the C-button. It is not aware of your current speed and does not adjust accordingly. When you hit a hill, you'll slow down unless you release the C-button, speed up and repress the C-button.

**Cruise control** is a closed loop speed control and cannot be implemented in the controller because the controller doesn't know what your speed is. 
The VESC has built-in cruise control logic when using the Nyko-Kama nunchuck.
When you press the C-button, the VESC takes your current *speed* as the setpoint and autonomously adjusts motor current in order to maintain that speed. When you hit a hill, the VESC will increase current to keep you from slowing down.
Using the Nyko Kama, when you keep the C-button pressed and accelerate, the VESC will automatically take your new, faster speed as the new setpoint.
```

---
## \#18 Posted by: Maxid Posted at: 2016-05-26T13:15:13.972Z Reads: 129

```
question remains: can the second channel on this remote be misused as a cruise control (especially with the VESC)?
```

---
## \#19 Posted by: trbt555 Posted at: 2016-05-26T13:20:12.227Z Reads: 133

```
Probably not in any practical way without serious tinkering in the VESC code, which is written for the Nunchuck which uses I²C protocol to communicate with the VESC.
The interface with a standard RC controller is a dumb PWM signal.
```

---
## \#20 Posted by: philipp Posted at: 2016-05-26T14:04:19.271Z Reads: 125

```
Dumb... but obviously reliable.
Is there already a reliable wiiceiver (or similar)?
Still waiting for updates on this site : product/wireless-wii-wiiceiver/

Edit:Spelling
```

---
## \#21 Posted by: makevoid Posted at: 2016-05-26T14:12:02.394Z Reads: 122

```
yes, it has a receiver and a loop key in the package to do the binding

I am no vesc expert but with "Current" configuration, when I accelerate I get progressive acceleration instead of constant acceleration, the one that I get with a normal ESC

I'm not sure about the % but
If I push the throttle forward to +25% (75%) and keep it like that with a standard ESC I go to fixed speed X and it stays the same (on an ideal flat road, no air resistance lol)

If it do it on the vesc it will continue to accelerate slowly until it reaches almost max speed I think, this until i lower the throttle to +20% (or something similar), at this point it will stop accelerating and keep the same speed.

http://www.electric-skateboard.builders/t/vesc-faq-duty-cycle-vs-current-control-ppm-settings/1218

Oh, by reading this post I understood that this happens because I've set "Current" control (no reverse with brake), I didn't tried the others yet but I'm very happy with this because I can use controllers like this compact one that are less precise than a trigger-style one but, thanks to current control they are more than ok because this mode requires less precision. It needs to vary the current "acceleration" value, not the overall power 0-100. Hope this makes sense :)
```

---
## \#22 Posted by: trbt555 Posted at: 2016-05-26T14:19:45.623Z Reads: 113

```
For what it's worth, I've never had one single hiccup with my Nyko Kama in the past 6 months and I've been riding very often.
```

---
## \#23 Posted by: philipp Posted at: 2016-05-26T14:33:58.742Z Reads: 109

```
I'd love to use  a NC as remote but decided not to because of a few negative feedbacks about  its reliability.
Hearing that your works fine really makes me want to get one.
What "Nunchuck-Receiver 2 VESC"-Module do you use? The Wiiceiver that isn't available atm.?
```

---
## \#24 Posted by: Maxid Posted at: 2016-05-26T14:51:06.214Z Reads: 111

```
Nyko kama works without an additional receiver with the VESc
```

---
## \#25 Posted by: philipp Posted at: 2016-05-26T15:29:18.425Z Reads: 114

```
Hmmm.. Okay, the many posts and videos with people that use a custom pcb after the receiver irritated me.

I'll a order a Nyko Kama and try it out following this tutorial:
http://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139

Adding a channel to activate cruise control on the vesc with 2.4 remotes would still be awesome though.
```

---
## \#26 Posted by: trbt555 Posted at: 2016-05-26T17:33:35.334Z Reads: 102

```
Tip:
After you open up the Nyko Kama receiver, don't use or lengthen the wires that it comes with, desolder them and replace them with longer ones, long enough to put the receiver as far as possible from the VESC.
Put the receiver back into it's little case to protect it and hot-glue the whole thing shut (after testing).
On the VESC side, hot-glue the jst-connector in place.
```

---
## \#27 Posted by: philipp Posted at: 2016-05-26T17:57:22.087Z Reads: 97

```
Thanks for these helpful tips! :slight_smile:
```

---
## \#28 Posted by: lowGuido Posted at: 2016-05-26T19:00:04.975Z Reads: 95

```
[quote="philipp, post:23, topic:3848"]
but decided not to because of a few negative feedbacks about  its reliability.
[/quote]

I have used Nyko Kama on many builds with and without wiiceiver.  never had an issue with a properly soldered connection.

I don't really understand where all this "negative feedback" comes from. I can only assume a lot of people aren't doing it properly.
```

---
