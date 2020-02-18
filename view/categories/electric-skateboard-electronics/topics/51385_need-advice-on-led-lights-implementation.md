# Need Advice on Led lights implementation

### Replies: 14 Views: 1619

## \#1 Posted by: Rotko Posted at: 2018-04-06T09:20:34.960Z Reads: 271

```
Hi guys,

I need an advice regarding the implementation of led lights (front and retro) in my setting:

10S3P 30Q
2x Focbox
Software: Ackmaniac Esc tool (works flawlessly, donation done)
Mini Remote (Ch1: throttle, Ch2: cruise control)

Cruise control for me is mandatory so, sadly, I must give up controlling the lights per ch2.
I think there are basically 2 solutions left in my case: 
1)	Connect the 10s3p battery to the leds, forsee a mechanical switch on the enclosure (no possibility to send the brakes signal from the remote throttle to the tail lights, in order to have stronger break lights when I brake)
2)	Forsee some independent rechargeable led lights (no possibility to send the brakes signal from the remote throttle to the tail lights, in order to have stronger break lights when I brake)

Am I right? Is there any other possibilities?
What are the pros and cons of these two solutions?
In case 1) is there some wise thread you can point me to? I need to understand how to do that without blowing up.

Thank you in advance for your help
```

---
## \#2 Posted by: Acido Posted at: 2018-04-06T10:10:58.268Z Reads: 253

```
led light do not work on 36v i think...
you would need a step down converter
some guy here made the 2. solution you posted here with an arduino... there's a thread about it
```

---
## \#3 Posted by: Rotko Posted at: 2018-04-06T10:21:40.804Z Reads: 239

```
Thank you Acido, I'll start looking for the step down converter
```

---
## \#4 Posted by: b264 Posted at: 2018-04-06T19:29:02.974Z Reads: 233

```
[quote="Acido, post:2, topic:51385"]
led light do not work on 36v i think
[/quote]

An LED works fine on 36V or 500V as long as it has the proper current-limiting resistor.  An LED driving circuit probably doesn't, though.  If you use 2 LEDs mounted opposite polarity to one another you could even run them on 240V AC if you used a large resistor.

It's the drive circuit that has the limitations... not the diodes themselves
```

---
## \#5 Posted by: wafflejock Posted at: 2018-04-06T19:36:56.452Z Reads: 222

```
Agree with Acido on 2 you can use an arduino to "analogRead" the signal and use the value to decide whether or not to turn on the LEDs.  You'd need to step down the voltage from the battery for the arduino (believe linear regulator on the arduino can deal with around 16V max coming in but a bit lower is probably safer), beyond that though pretty sure the LEDs can be powered directly off the digital pins on the arduino (5V but somewhat low current so depends on what LEDs or arrangement you go with there)

Always find this useful when messing with LEDs: http://led.linear1.org/led.wiz

Also did my own 'riser lights' here:
https://cad.onshape.com/documents/7be8e5eec66596f68a989626/w/2c722dcc2ec89f5c71643bec/e/488c17c6f310d5c7be62da8a

Put a 350mAh battery in there, USB charger and switch (I didn't do the tapping into the throttle signal stuff).

https://photos.app.goo.gl/u6A9XjzjCiAhHp9n1
```

---
## \#6 Posted by: Mich21050 Posted at: 2018-04-06T19:41:58.411Z Reads: 198

```
I'm not sure but you could also use those ppm brake lights from eskating here is the link :smile:
 https://eskating.eu/product/6w-waterproof-led-light-kit-with-rear-brakes-control/
```

---
## \#7 Posted by: CHAINMAILLEKID Posted at: 2018-04-06T19:53:39.448Z Reads: 198

```
You can get LEDs for a lot of different voltages, but I think the 36V ones tend to be pretty high wattages.

I think the step down converter you'd want to get lower would be a buck regulator.
```

---
## \#8 Posted by: Rotko Posted at: 2018-04-07T12:14:34.337Z Reads: 172

```
thanks a lot for the big amount of info. I will consider it.
@Mich21050
I considered the idea of using what you suggest, in fact I have @fottaz 6W Waterproof Led light kit with REAR BRAKES CONTROL.

The wiring works like this:
![IMG_20180407_111839|673x500](upload://8NUeOK7DryZPx21aj3Wf2F6bbX0.jpg)

So considered my case I can't connect to Vesc because I need, following Ackmaniac's indication, Master slave connection for throttle, while slave connection for cruise control . Can't connect to receiver because I use the two channel (mini remote has only two ch) for same throttle and cruise control.
```

---
## \#9 Posted by: Deckoz Posted at: 2018-04-07T15:57:45.443Z Reads: 153

```
If you want bright LEDs. Use a meanwell Ldd-100h driver and some Cree, osram, or Phillips 3-8w LEDs...
```

---
## \#10 Posted by: StarLoad Posted at: 2018-04-08T02:32:44.433Z Reads: 150

```
https://www.electric-skateboard.builders/t/making-simple-wireless-switch-and-brake-light/49805?u=lunarkim

@LunarKim 
I saw what you want here.
```

---
## \#11 Posted by: fottaz Posted at: 2018-04-08T19:02:15.303Z Reads: 130

```
Hey rotko, it should not be a problem for you (and for everybody using also all receiver channels) because "to receiver" of the led kit goes in the 1st channel that you normally use for throttle, then "From Vesc" the ppm signal of the controller that  your normally plug into the receiver. It doesn't changes nothing for you if I've understand good what you meant.
```

---
## \#12 Posted by: Rotko Posted at: 2018-04-09T09:07:34.629Z Reads: 120

```
Hi @Fottaz,

Maybe I get what you say.
With this setting:

![FACKBOX|690x293](upload://aVvfhgy0Fm9phfjRqWdrts4isXq.jpg)
![receiver|640x480](upload://uZNdims1U2OKWpPjnuM5Qtrhzob.jpg)

I would be able to use your led lights (+ Higher red tail lights while braking)  and, at the same time, Ackmaniac's cruise control?

 Fell free to correct / confirm.
Thank you
```

---
## \#13 Posted by: fottaz Posted at: 2018-04-09T18:52:30.141Z Reads: 113

```
@Rotko Yes Sir, you will be able to use throttle signal and the lights at same time, you should see the brake module as a Y splitter, of course it keeps the signal between receiver and vesc, and it takes signal needed for the brakes light effect!
```

---
## \#14 Posted by: fottaz Posted at: 2018-04-09T19:17:00.988Z Reads: 112

```
Hope it's more clear like this, it doesn't change any previous connection.
![image|690x444](upload://xKwaV6QtIhnk0A5h9PqT1xtC2o1.png)
```

---
