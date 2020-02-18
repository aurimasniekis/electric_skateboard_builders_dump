# DIY 18650 Battery Related Questions

### Replies: 28 Views: 1161

## \#1 Posted by: Jojo5 Posted at: 2018-05-07T03:21:01.713Z Reads: 154

```
Hello all, 
I've just recently gotten back into electric skateboard related stuff after finishing my board last summer. After a bunch of research and reviewing what I have I decided to try my hand at building a 10s4p 18650 Li-ion pack out of Samsung 30Q cells from [liionwholesale](https://liionwholesale.com/). 
Here is a picture of my progress as of now
![IMG_20180506_165613|375x500](upload://ad1v0EQtNoxRJsHl4F3cc7DcrYq.jpg)
I've been using "pure nickel strips" from [Vruzend](https://vruzend.com/product/100-pure-nickel-strip-for-battery-building/). They are .15mm x 7mm and supposedly carry 7 Amps. 
For spot welding I've been using the spot welder that [Aulakiria](https://m.blog.naver.com/aulakiria/220992039512) makes and it has been working great so far.

My main question concerns Current (Amperage) capacity of the nickel strips and where I need to double up. As of now my estimated average current draw will be approximately 60A (Samsung 30Qs discharge 15A multiplied by 4 in parallel) which suggests that I need to layer my nickel strips somewhere. 
Do I need to have multiple layers of nickel strip across only the series connections? Only the parallel connections? Or both?
Thanks for reading :+1:
```

---
## \#2 Posted by: ToucanSam Posted at: 2018-05-07T05:01:41.677Z Reads: 139

```
Series connections have to survive higher wattage than the parallel connections. I built a 12s6p battery with Samsung 30Q cells. 30Q cells have been tested to reliably output around 20A which is why I went with them over the 25R5 cells. So I would use enough Nickel to withstand 80A.
```

---
## \#3 Posted by: Okami Posted at: 2018-05-07T05:23:39.483Z Reads: 134

```
I would say 5 strips minimum, if u can. Though in real life with little hills maybe u wont need more than 30A, I think.

Yes go for beefing up serial connections.

2nd option - **Unpopular way how to beef up**: solder thicker cable on top, if space permits (using acid and decent power soldering iron)
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-05-07T05:38:59.300Z Reads: 121

```
Or get thicker nickel strips
```

---
## \#5 Posted by: Jojo5 Posted at: 2018-05-07T05:42:03.410Z Reads: 116

```
If I were to use enough nickel for 80A it would turn out to be something like 11 layers correct? (80A current / 7A nickel capacity = 11.4 layers)
Is there an alternative method to stacking so much?
```

---
## \#6 Posted by: Jojo5 Posted at: 2018-05-07T05:44:32.832Z Reads: 112

```
Do you have a source?
```

---
## \#7 Posted by: Trdolan03 Posted at: 2018-05-07T05:44:42.894Z Reads: 111

```
There is motor amps and battery amps. You need to layer if for about 30 amps and just limit your vesc to 30 battery amps. You can still run your motor at 80 though.
```

---
## \#8 Posted by: Trdolan03 Posted at: 2018-05-07T05:47:51.659Z Reads: 114

```
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F123040528620
You can get .2mm here which would make it a few layers thinner.
Edit: or you could use wider strips. 7mm is pretty small compared to the 18mm diameter of the cells. Bump it it to .2mm x15 and you have almost 20 amps per strip to work with.
```

---
## \#9 Posted by: Jojo5 Posted at: 2018-05-07T05:54:53.903Z Reads: 112

```
Thanks for your input I think I'm starting to get it. Basically I just need to layer 5 or 6 nickel strips across each serial connection with the nickel that I have in order to get 30-35 battery Amps. Or I could get some thicker nickel and use 3-4 layers to achieve the same effect. 
If I find that the spot welds aren't holding between the layers of nickel can I use a bit of solder to hold it together?
```

---
## \#10 Posted by: ToucanSam Posted at: 2018-05-07T06:08:19.837Z Reads: 106

```
I used higher amperage strips of nickel, each of my strips was rated for 10A to 15A, so yes I just spot welded a bunch of them to each series connection. I also have service series connections though, every other series connection I made, instead of using nickel I soldered on 8AWG wire with 6mm bullet connectors. This was originally because I was going to use 6 separate battery enclosures spaced out under the board but I didn't end up with enough space so long story short... Soldering on some nice wire will also work just fine, just make sure your wire can withstand the draw from the motors. In my case I will be heat sinking my VESC's and allowing them to push 60A per motor to max out my battery's capability. So I had to get series connection wire capable of withstanding 120A, since the wires are all only a few inches, 8awg was my gauge of choice to be safe.
```

---
## \#11 Posted by: Trdolan03 Posted at: 2018-05-07T06:09:47.083Z Reads: 100

```
@ToucanSam  The battery draw is much lower than the motor draw. Your batteries will not need to push 120a
```

---
## \#12 Posted by: ToucanSam Posted at: 2018-05-07T06:11:04.282Z Reads: 96

```
Yes you can use solder to hold them, make sure you scratch up the nickel where you're going to solder though, sometimes solder will slide right off those slippery smooth strips. Also be careful not to glob on the solder, too much in one place will create electrical resistance.
```

---
## \#13 Posted by: Trdolan03 Posted at: 2018-05-07T06:11:50.569Z Reads: 93

```
If you plan on soldering the nickel strips you may want to consider pre tin
```

---
## \#14 Posted by: Okami Posted at: 2018-05-07T06:14:32.446Z Reads: 90

```
I recently got a hold of acid made for soldering onto cells.. dont know what I would have done without it. 

Leaving solder on spot now takes just 1-2s of heating.. works like a charm both for cells and nickel strip. From experience it was rather hard with regular califony to get decent amount of solder, where needed
```

---
## \#15 Posted by: Trdolan03 Posted at: 2018-05-07T06:15:35.933Z Reads: 88

```
[quote="Okami, post:14, topic:54628"]
acid made for soldering onto cells
[/quote]

Link to it?
```

---
## \#16 Posted by: ToucanSam Posted at: 2018-05-07T06:17:39.050Z Reads: 90

```
That part was never explained to me, I was told if I tell my VESC to allow 60A per motor and I have a battery capable of 120A, things like steep hills and accelerating faster will benefit because I have the amperage the motors need. Where as if I were using a 60A battery and 30A per motor I would not have as good performance. So like acceleration from stop for instance, brushless motors use higher amperage for more torque so if they have access to higher amperage they will have more torque. Is that not the case?
```

---
## \#17 Posted by: Okami Posted at: 2018-05-07T06:18:04.723Z Reads: 91

```
Well I can try to recommend getting one from aliexpress. The one I got was crafted locally. 

I heard it is used in jewelry and u can basically make it at home. I think zinc plates left in salt water was used in making it. After it has reacted, u just need to use a tiny drop of this 'solution' / acid for soldering.

Maybe theres a tutorial on instructables to try out.

Soldering is easy as solder gets attracted quite aggresively this way. Though sometimes solder blobs may fly around which is not that cool and should be looked after

---

On a side note. I also heard about a process where copper gets plated with nickel. That would make whole process easier but i forgot whenever it is later possible to also spot weld it or not
```

---
## \#18 Posted by: Trdolan03 Posted at: 2018-05-07T06:22:12.427Z Reads: 87

```
That could be true for small motors and low amperages 5-15 motor amps. However, I have tested a dual drive mountainboard accelerating up a steep hill and it only drew battery 30 amps.
```

---
## \#19 Posted by: Trdolan03 Posted at: 2018-05-07T06:28:56.980Z Reads: 85

```
It has to do with the PWM control method the vesc uses to control the motor.
```

---
## \#20 Posted by: ToucanSam Posted at: 2018-05-07T06:36:26.552Z Reads: 83

```
I see, well that's interesting I'll look in to it! Either way I'll have baller range ;D I also have talked to a lot of people that say the exact opposite, and from what I know about motors I won't lie I expect a very large performance difference between when I allow 30A and 60A. When I finish my build I will post of the build process and my findings!
```

---
## \#21 Posted by: Trdolan03 Posted at: 2018-05-07T06:45:38.623Z Reads: 76

```
I would love to be wrong! Report back with your findings
```

---
## \#22 Posted by: Ackmaniac Posted at: 2018-05-07T07:14:08.258Z Reads: 76

```
Make 4 layers for your series connection by putting 2x 2layers like this
![image|273x233](upload://gB7yKDYrp6vInE937v6ZGeCqSOF.jpg)
No way you are drawing 120A constant. Even 60A constant is far off.
And the bursts are also no problem.

And do not even think about the idea to solder something to the battery. Why did you buy a spot welder.
```

---
## \#23 Posted by: xilw3r Posted at: 2018-05-07T07:21:06.486Z Reads: 76

```
I would like to add to Ackmaniac, try welding strips one over another on two dummy cells and see how many you can get welded reliably, because the more you weld on the harder it gets to do it correctly. You might want a beefier Lipo for that action. 3 should be easy to do on one another without issues. Hey, having more thermal mass wont make things worse :)

Edit: there is something wrong with the replying thing, two posts in a row now that I made suddenly had a quote of another post which I definitely did not make. Anyone else getting this?
```

---
## \#24 Posted by: Trdolan03 Posted at: 2018-05-07T07:25:16.145Z Reads: 75

```
[quote="xilw3r, post:23, topic:54628"]
Edit: there is something wrong with the replying thing, two posts in a row now that I made suddenly had a quote of another post which I definitely did not make. Anyone else getting this?
[/quote]
Nothing wrong here.
```

---
## \#25 Posted by: Okami Posted at: 2018-05-07T08:18:52.946Z Reads: 71

```
Should have inspected his layout a bit more. U are right, that config should work nicely
```

---
## \#26 Posted by: Jojo5 Posted at: 2018-05-07T14:14:58.063Z Reads: 66

```
I saw in a YouTube video by [EbikeSchool](https://youtu.be/wdZ_Ca_sAZE) that when stacking nickel I should use a "pyramid style" of layering. Something like this: ![IMG_20180506_181321__01|375x500](upload://6gUvJsJnuK1gk8RWsPJEFZm7cW4.jpg)
Would this be more reliable or would I be okay just stacking two layers to the closest cells in each series connection as shown in your diagram?
```

---
## \#27 Posted by: Ackmaniac Posted at: 2018-05-07T14:18:40.378Z Reads: 64

```
2 layers at the closest have the same effect. The orange lines in your picture carry 20A and the red lines 40A.
BUt it also doesn't hurt if you add one strip in the length of the orange lines and one for the red lines.
```

---
## \#28 Posted by: Jojo5 Posted at: 2018-05-08T00:26:14.974Z Reads: 51

```
![IMG_20180507_155415|375x500](upload://zGIttYCLSz506WgIoGvzOLDpTn.jpg)
Double layered nickel on the series connections. Hopefully it holds up.
Edit: image didn't upload
```

---
