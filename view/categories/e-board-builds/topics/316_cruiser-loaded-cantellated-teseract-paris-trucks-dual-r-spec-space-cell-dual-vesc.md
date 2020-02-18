# Cruiser &#124; Loaded Cantellated Teseract &#124; Paris Trucks &#124; Dual R-SPEC &#124; SPACE Cell &#124; Dual VESC

### Replies: 20 Views: 3889

## \#1 Posted by: Mitch Posted at: 2015-10-15T09:27:11.515Z Reads: 185

```
Hey guys,

So after reading many discussion on here I've decided to build my first electric skateboard and going all out first go!

I am planning on ordering  2 x enertion r-spec 2.0 brushless motors, space cell battery, 2 x DIY electric skateboard torqeboards 12S 120A car ESC OPTO HV, Wiireceiver with numchuck, 12S UBEC and 2 x motor mounts.

If someone could provide some feedback on this setup and if anyone has overcome the issue of only being able to go to 80% with the space cell before shorting out the ESCs it would be greatly appreciated :)

I will be sure to post my build once its complete.
```

---
## \#2 Posted by: lox897 Posted at: 2015-10-15T09:30:12.860Z Reads: 183

```
I think @cmatson will know about the space cell. Or @onloop.
```

---
## \#3 Posted by: lox897 Posted at: 2015-10-15T09:31:02.954Z Reads: 179

```
Good setup! Do you have hills in a your area and how much do you weigh?
```

---
## \#4 Posted by: Mitch Posted at: 2015-10-15T10:30:04.045Z Reads: 171

```
Thanks for the reply lox897, yer I have some medium to steep grade hills in my area and way around 80kg. Do you think this setup will be able to handle going up hills? does it all depend on the gearing setup...
```

---
## \#5 Posted by: sl33py Posted at: 2015-10-15T13:54:32.263Z Reads: 168

```
yes, it's all in the gearing.  This will be a beast with dual 63mm r-spec.  Depending on your battery of choice 10/12s it will be a bit of a handful.

Unless you are a seriously talented rider, i might suggest easing into it with lower series batteries to start, then you can add more as you get more comfortable.  6-9-12s would be my suggested "learning" curve.
```

---
## \#6 Posted by: longhairedboy Posted at: 2015-10-15T19:56:37.099Z Reads: 165

```
You can achieve the same effect by programming those ESCs to not be maxed out all the time. Dial the throttle output way down until you get used to it then tune it up some more when you're ready.  At least i think you can still do that on those ESCs when using a nunchuk. Anyway it would save you money on batteries.
```

---
## \#7 Posted by: lox897 Posted at: 2015-10-15T21:16:33.821Z Reads: 166

```
@longhairedboy That's a great idea. I would do that.
```

---
## \#8 Posted by: lox897 Posted at: 2015-10-15T21:17:13.590Z Reads: 168

```
I don't know much about gearing and @sl33py is pretty great.
```

---
## \#9 Posted by: cmatson Posted at: 2015-10-16T01:38:04.153Z Reads: 178

```
I currently have a space cell, torqueboard's esc, and single enertion r-spec setup like @lox897 said.

Unfortunately, I haven't been able to solve the 80% problem, even though I live in a completely flat area... 

**settings I am using:**
My acceleration is set to the lowest setting (which surprisingly, is actually pretty quick).
max forward: 80%
no reverse, 80% braking (a lot of braking when you slam on it, but I like being able to stop on a dime just incase...)
motor timing is also at the lowest setting, which makes the overall speed slower, but cuts down on amp draw.

basically, the problem is the space cell's max of 60 amps; it isn't a bad thing, just torqueboard's esc is a beast, and was designed to pull more than the space cell can handle. tons of people use it with lipo's of a higher discharge rate without a problem.

**Solution to the 80%!!!!!!!**
Buy a VESC instead! not bashing torqueboard's esc, it really is awesome and easy to program; just for the space cell, a VESC is way better. Also keep in mind that all my settings are set up for my weight (140ish pounds, 65kg) on 14/36 gearing. I have also tried 13/36, and 16/36, but the middle ground worked best for me. 

When my dad took my board for a spin, he blew the space cell's fuse (standard automotive fuse; cheap, and easy to replace) within 5 seconds of riding it... he weighs about 200ish pounds, 95kg).

good luck man!
```

---
## \#10 Posted by: elkick Posted at: 2015-10-16T12:50:39.662Z Reads: 161

```
You're right, I'm using the space cell with two VESCs and since you can limit battery values to 60A and still put the values for the motors higher (like 2x 80A), it never blows the fuse. Also, I'm able to climb steep hills without any issues, even with hub motors which are quite demanding for power usually.
```

---
## \#11 Posted by: Mitch Posted at: 2015-10-17T01:07:25.085Z Reads: 154

```
Thanks for the help everyone. So just starting looking into the VESC and it seems like a much more efficient setup and a lot more features without the risk of blowing a fuse. Just to clarify if i purchase 2 x VESC will i still require a UBEC and wiireceiver?
```

---
## \#12 Posted by: Mitch Posted at: 2015-10-17T01:15:46.694Z Reads: 156

```
Hey elkick, can you post a couple photos of your setup/
```

---
## \#13 Posted by: cmatson Posted at: 2015-10-17T01:54:29.700Z Reads: 158

```
nope, you won't need the UBEC. You also won't need a wii receiver if you are willing to put in a little extra effort.

It is worth it though, because the external wii receiver sometimes looses connection because it isn't soldered to the board.

here is a thread for the wii receiver: http://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139/21
```

---
## \#15 Posted by: lox897 Posted at: 2015-10-17T02:30:26.570Z Reads: 159

```
Elkick's board looks like this: https://endless-sphere.com/forums/viewtopic.php?f=35&t=73295&p=1107111#p1107111

Scroll down.
```

---
## \#16 Posted by: elkick Posted at: 2015-10-17T09:37:14.734Z Reads: 169

```
@Mitch, some more photos of the hub motors build (V1 and V2): 
<img src="/uploads/db1493/original/1X/0ac4928313b06303e5618de1b97e11381b5d6c8e.jpg" width="690" height="243"> <img src="/uploads/db1493/original/1X/837e53591862ecaca3cbb395a9a304c410b9c988.jpg" width="261" height="500"><img src="/uploads/db1493/original/1X/08e6d887faaa5ed97717fb802060698d57a89c39.jpg" width="448" height="500"><img src="/uploads/db1493/original/1X/540516b1357ad07b367f4941e049712b96b346f6.jpg" width="252" height="500"><img src="/uploads/db1493/original/1X/a242fee45ed913bec012234581c52579e92308be.jpg" width="690" height="333"><img src="/uploads/db1493/original/1X/038bd0aa1f95ff442b8cf176902c455258f7ba41.jpg" width="545" height="500">
```

---
## \#17 Posted by: onloop Posted at: 2015-10-30T23:21:00.122Z Reads: 142

```
@kai In order to make the "E-board Builds" category really easy to search & locate specific builds i am asking that you change your title to something descriptive that better expresses the makeup of your build.

Most of the new build threads tend to end up with a name such as 
**"new- noob - noobie - beginner - first - build - help - newb"** this becomes hard to keep track of.

I would like to see each build thread with a descriptive title, such as;
**Project Name | Deck Name | Trucks | Motor type | Mounting method | Voltage/Battery | ESC**

Example
**The Samurai | Custom Deck | Paris Trucks |  R-SPEC | Custom Mount | 10S | VESC**
```

---
## \#18 Posted by: broshi Posted at: 2015-12-10T14:55:41.444Z Reads: 124

```
I basically want to try this build.

Could you tell me what kind of hills the hub motors can take and the top speed max range?
```

---
## \#19 Posted by: elkick Posted at: 2015-12-10T15:34:54.139Z Reads: 125

```
It's a Rayne Mosquito II, with 83mm flywheels, dual CarvOn hub motors V2, Enertion Space Cell, dual VESC and a Nunchuk remote. Max. speed is 68kph with 83mm and its around 90kph with the 90mm wheels. I've never had difficulties with hills so far, but starting from a standstill wont work if it's more then 10-12%. I am about 72kg so I don't know how it would perform if somebody is around 100kg, but I usually tow my kids also uphill and nothing happens if I approach that hill in slow speed.

It's really difficult to give an advice since people tend to have different requirements. I wouldn't recommend hub motors  for those steep hills around 25%, not because it's not possible, but it's might be no fun longterm if the motors are pushed to their limits in low ERPM all the time. 

But think it would be quite easy to sell that board again if you're not happy with it. :grinning:
```

---
## \#20 Posted by: broshi Posted at: 2015-12-10T17:19:08.199Z Reads: 123

```
JESUS 68km/h  I'm definitely going to get them, that's the nail in the coffin!

I think I basically have the same components as your build. 

should be fun to build and ride, thanks!
```

---
## \#21 Posted by: elkick Posted at: 2015-12-10T17:32:59.042Z Reads: 118

```
Sorry, it's a Rayne Piranha deck of course (don't know why this was misspelled).
```

---
