# Help setting up GT2B (SOLVED)

### Replies: 23 Views: 144

## \#1 Posted by: Sapphirinia Posted at: 2019-02-07T18:59:52.835Z Reads: 42

```
Hey guys, so I replaced my bust vesc with a focbox and it seemed as though the remote was having issues when I was trying to calibrate it in BLDC. Fast forward to now, I got a replacement GT2B and I'm having the same issue. When I hit display to set the pulse width it just stays in the middle. If I play with the trim it'll move to different places but it won't change based on the trigger pull. Can I get some help here?
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-02-07T19:00:52.064Z Reads: 41

```
You sure its set to PPM (and UART if BT module)?
```

---
## \#3 Posted by: Sapphirinia Posted at: 2019-02-07T19:04:01.481Z Reads: 37

```
![IMG_20190207_140234396|375x500](upload://kZo6Pq81EWJlbU6GDeEgFzPibu8.jpeg)
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-02-07T19:05:13.708Z Reads: 32

```
Not sure, might have something to do with how you have no control method set :thinking:

E; if you were to choose one, you want control no reverse with brake
```

---
## \#5 Posted by: Mich21050 Posted at: 2019-02-07T19:06:51.319Z Reads: 29

```
Did you run the input wizard also does your gt2b receiver blink?
```

---
## \#6 Posted by: Sapphirinia Posted at: 2019-02-07T19:06:54.190Z Reads: 31

```
I was following some instructions on enertion site. That's what it said to do to set up the remote ![Screenshot_20190207-140558|250x500](upload://6jtI7kBICeR1xSgKMAfCHDUpOYU.png)
```

---
## \#7 Posted by: Sapphirinia Posted at: 2019-02-07T19:08:13.996Z Reads: 25

```
Receiver is solid. I don't think there's a wizard on this one.
```

---
## \#9 Posted by: Sapphirinia Posted at: 2019-02-07T19:11:52.515Z Reads: 27

```
Ok so if I move the steering wheel on the remote it moves it
```

---
## \#10 Posted by: Mich21050 Posted at: 2019-02-07T19:12:32.500Z Reads: 25

```
Then you plugged it in on the wrong channel. Plug your focbox into ch2 on your receiver.. :slight_smile:
```

---
## \#11 Posted by: Sapphirinia Posted at: 2019-02-07T19:13:31.316Z Reads: 20

```
There we go... And I probably didn't need to buy another remote
```

---
## \#12 Posted by: Mich21050 Posted at: 2019-02-07T19:13:51.777Z Reads: 19

```
@mmaner I think this is solved.. :slight_smile:
```

---
## \#13 Posted by: Sapphirinia Posted at: 2019-02-07T19:15:10.321Z Reads: 19

```
I randomly turned the little wheel out of boredom and noticed lol
```

---
## \#14 Posted by: Mich21050 Posted at: 2019-02-07T19:16:08.577Z Reads: 20

```
Next time when you are facing any issue just post some pics so it's easier for people to help you.. :slight_smile:
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-02-07T19:18:47.324Z Reads: 20

```
Use the new vesc tool... its much simplier

nothing to do with is topic**
```

---
## \#16 Posted by: Sapphirinia Posted at: 2019-02-07T19:19:27.574Z Reads: 20

```
I didn't know if it worked with focbox. It's my 1st one
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-02-07T19:20:09.063Z Reads: 19

```
enertion has it posted.
https://www.enertionboards.com/FOCBOX-foc-motor-speed-controller.html
```

---
## \#18 Posted by: dareno Posted at: 2019-02-07T19:20:54.977Z Reads: 19

```
hit the solution button on this then @Sapphirinia on @Mich21050 post.  If it makes you feel better I have done far worse.    
Vesc tool works fine with focboxes but you may have to update firmware
```

---
## \#19 Posted by: Sapphirinia Posted at: 2019-02-07T19:21:17.150Z Reads: 20

```
That's the one I downloaded
```

---
## \#20 Posted by: Mich21050 Posted at: 2019-02-07T19:21:38.541Z Reads: 19

```
Or just use @Ackmaniac firmware/tool :slight_smile:
```

---
## \#21 Posted by: AlanZhou Posted at: 2019-02-07T19:21:41.035Z Reads: 18

```
really lol?

https://vesc-project.com/vesc_tool

^updated verson, works with focboxes because its a regular 4.12 (upgraded)
```

---
## \#22 Posted by: Sapphirinia Posted at: 2019-02-07T19:22:12.386Z Reads: 15

```
Yea lol. It's the regular bldc
```

---
## \#23 Posted by: Mich21050 Posted at: 2019-02-07T19:22:36.633Z Reads: 14

```
How's typing with one hand? :joy:
Sorry...
@AlanZhou heal fast
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-02-07T19:22:48.340Z Reads: 14

```
frickin suck. Other hand is semi usable
![IMG_20190207_142256|375x500](upload://vzdVDKdQUg8K1YEW49d0yAng5yh.jpeg)
```

---
