# VESC not connecting to computer, and other issues

### Replies: 9 Views: 802

## \#1 Posted by: zamexil Posted at: 2017-05-02T03:39:29.014Z Reads: 87

```
So I am working on building my own e-board mostly from scratch for a school project, and I have made it to my final step, which is getting the electronics to work. For my vesc, I bought the option from torqueboards. I was setting it up and eventually after a little bit of struggle, was able to connect it to the BLDC tool. On the torqueboards website they have a video guide on how to set up the vesc, and I was following this to set mine up. I got the the step where the vesc detects the motor, however when I clicked the motor detect button on the BLDC tool, the motor just twitched and everything diconnected. I cycled power to the vesc and tried to reconnect however, when the vesc turned on again, the three red lights that are supposed to flash when it is first powered on did not flash, and I was never able to connect it. I tried all of the usb cables I have in my house, and my computer wouldn't recognize that anything was being plugged in with any of these cables. I did some research and found that people have had vescs from torqueboards short out due to untrimmed pins piercing the power cables. I checked mine and it appeared that this may have happened, however when I sent a picture of it to the people at torqueboards, they said that they didn't think this was the issue. I tried to reconnect again today and my computer still doesn't recognize that anything is being plugged in with any usb cables that I plug in. Whenever I power on the vesc the solid blue light still turns on and the wireless controller receiver turns on and is able to connect to the controller. I guess my questions from all of this are: 1) is my vesc shorted out, and 2) if it's not, does anyone know of a fix for this? Thanks for any help!
```

---
## \#2 Posted by: Blasto Posted at: 2017-05-02T03:46:29.306Z Reads: 83

```
[quote="zamexil, post:1, topic:22188"]
I got the the step where the vesc detects the motor, however when I clicked the motor detect button on the BLDC tool, the motor just twitched and everything diconnected.
[/quote]

What power source are you using? My guess here is your using a small power supply with a lack of current
```

---
## \#3 Posted by: zamexil Posted at: 2017-05-02T03:50:43.310Z Reads: 80

```
I bought the 12s battery pack from their website, and it was fully charged when I used it
```

---
## \#4 Posted by: Blasto Posted at: 2017-05-02T03:55:33.449Z Reads: 76

```
Do you have pictures of your setup? 

Does your vesc power up anymore?
```

---
## \#5 Posted by: zamexil Posted at: 2017-05-02T04:04:39.796Z Reads: 74

```
here is a picture of the setup I took the first time I set everything up: http://imgur.com/a/5YUdu
And whenever I apply power to the vesc, the blue light on the back turns on, but the 3 red flashes that are supposed to happen don't. Also, before setting up the vesc, I was able to set up the wireless remote and the receiver for that, which is connected to the vesc, also turns on
```

---
## \#6 Posted by: Blasto Posted at: 2017-05-02T04:36:05.616Z Reads: 73

```
The blue led is on the 3.3V rail... that seams fine, meaning the 5V is ok also (does your receiver power up?)


Does sound like your mcu is dead... possibly by jump starting it with 50V (screwered pins), if that's the case we're talking about replacing half the components on the vesc.... inless it was an io pon and not the power pin that did the scewering
```

---
## \#7 Posted by: zamexil Posted at: 2017-05-02T04:39:53.276Z Reads: 74

```
ya the receiver powers up. 
So basically your saying that the board is pretty much dead?
```

---
## \#8 Posted by: Blasto Posted at: 2017-05-02T04:54:57.779Z Reads: 70

```
[quote="zamexil, post:7, topic:22188"]
So basically your saying that the board is pretty much dead?
[/quote]

Well if you had the normal power up before with the 3 red flashes and nothing now.... 

unfortunately yes (in my opinion). Just replacing the mcu could fix the problem, but i don't know what else could have gotten damaged
```

---
## \#9 Posted by: zamexil Posted at: 2017-05-02T05:00:45.438Z Reads: 69

```
ok, thanks a lot for the help. I'll probably email torqueboards and see what I can get in terms of a replacement
```

---
