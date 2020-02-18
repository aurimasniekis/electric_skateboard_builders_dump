# What is FOCBOX (vescx) ERPM Limit?

### Replies: 16 Views: 2226

## \#1 Posted by: onepunchboard Posted at: 2017-08-14T18:11:11.601Z Reads: 360

```
Hi,

What is FOCBOX ERPM Limit? I read vesc 4.12 generally use 60,000~80,000.
I know focbox is based on 4.12 but is it still the same ermp? on website it doesn't state anything tho 

I know default is 100,000  and this seems to cause drv fault.
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-08-14T18:13:21.831Z Reads: 350

```
Erpm is 60,000
```

---
## \#3 Posted by: BigBoyToys Posted at: 2017-08-14T18:19:46.750Z Reads: 343

```
Ive seen video of the FOC box at 84,000 erpm on an ebike.
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-08-14T18:21:09.263Z Reads: 340

```
exactly, it doesn't seems to have issue passing 60k it just get inefficient right?
```

---
## \#5 Posted by: BigBoyToys Posted at: 2017-08-14T18:30:38.312Z Reads: 328

```
I think the margin of safety past that speed is reduced so chances of failure are higher. Definatley a good idea to keep it @ 60K or below. My 12S 130KV 28 pole hub boards is pushing that limt on a full charge as well.
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-08-14T18:35:13.352Z Reads: 315

```
I see thanks for advice, I will stick to the 60k
```

---
## \#7 Posted by: trampa Posted at: 2017-08-14T19:03:52.715Z Reads: 309

```
It's a HW 4.12 at heart, so the limit should be the same.

Frank
```

---
## \#8 Posted by: Blasto Posted at: 2017-08-14T19:23:45.336Z Reads: 302

```
The ERPM limit was figured by @chaka through a trial and error process. The Infineon hex fets are big and slow compared to directfets.

**Hexfet**
<img src="/uploads/db1493/original/3X/f/3/f35448a2da7190a389fb8b8979af1be59c79d6c1.png" width="529" height="85">

VS
**Directfet**
<img src="/uploads/db1493/original/3X/0/1/017195c132ac4454975d859032c82f635cfae767.png" width="480" height="82">

Now add some slow fets with bad decoupling, then you have a very noisy circuit with a 60K erpm limit.

I'm sure if @chaka would do his testing with his directfet design his results would be different.
```

---
## \#9 Posted by: onepunchboard Posted at: 2017-08-14T19:45:00.382Z Reads: 288

```
so the old mosfet was main problem.
I guess it would be okay to say there is bit more head room.
I actually seen a video testing 100k on focbox. didn't seem to trigers anything.
thanks for info it was very helpful
```

---
## \#10 Posted by: chaka Posted at: 2017-08-15T12:56:37.140Z Reads: 268

```
The 60k erpm is mostly determined by the driver and the lack of the third current shunt resistor. I have found some MOSFETs that look better on  paper than the direct FETs but there always seems to be a trade off on rise time VS resistance.  One thing that can be done with FETs that have a low gate charge and high resistance is run 12 to spread the thermal dissipation? 

We really do not need to go above 60k erpm in eskate. @trampa If your machine needs to go that high you have a poorly designed build. From what I have seen in eMTB's you are actually running much lower than 60k.
```

---
## \#11 Posted by: trampa Posted at: 2017-08-15T15:48:49.206Z Reads: 237

```
Our customers have all sorts of projects on the boil and some need more ERPM. Good to know that 150K is possible now.

Frank
```

---
## \#12 Posted by: chaka Posted at: 2017-08-15T16:00:36.022Z Reads: 230

```
Yes of course, but it is better to run at a lower erpm for high current applications. The higher switching speed seems to effect the "on" resistance.
```

---
## \#13 Posted by: trampa Posted at: 2017-08-15T16:13:59.511Z Reads: 220

```
That is up to the developer of the equipment. The higher ERPM gives them a bit more freedom to use different motors. We use quite low KV motors.

Frank
```

---
## \#14 Posted by: onepunchboard Posted at: 2017-08-15T16:19:26.763Z Reads: 217

```
that's true, higher rpm gives more economic efficiency. as of most low kv motors in compact size is not easy to make and expensive.
```

---
## \#15 Posted by: chaka Posted at: 2017-08-15T16:44:40.155Z Reads: 213

```
I get that but this is an eskate forum and it is best to speak in terms of what works best  within our constraints.  Your information would be better suited on an RC forum, marketing wise I think you will be able to attract users who could utilize smaller high KV motors.

This type of marketing here generally just causes confusion to new builders.

Chaka
```

---
## \#16 Posted by: trampa Posted at: 2017-08-15T20:04:52.579Z Reads: 199

```
I didn't start that ERPM topic. 
I do also recommend low KV setups for ESK8. :wink:

Frank
```

---
