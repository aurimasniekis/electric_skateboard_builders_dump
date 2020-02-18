# GT2B install replacing wired remote - PPM to analog current

### Replies: 6 Views: 532

## \#1 Posted by: Canuck Posted at: 2017-12-09T18:49:24.781Z Reads: 86

```
First post, but I've been browsing the forums for several weeks now...

I'm trying to figure out a _cost effective_ mod for an E-Glide AT built board to work with a GT2B instead of the original _wired_ remote. For those not familiar, this board uses a PG Drives "I-Drive" ESC in conjunction with a brushed motor. The pre-installed remote is a simple wired pot, with a signal voltage operating range of 0-4.5V.

Here is the schematic from PG Drives (the speed limiting pot is optional and not installed in this application):

<img src="/uploads/db1493/original/3X/8/a/8a6f3b17874721caa934d8bc2a98d2fd9aaa6411.PNG" width="310" height="171">

So the question is, does anyone have any ideas as to what my options are for a cost effective way to integrate the PPM output of the GT2B RX with the analog voltage signal required for the I-Drive ESC without just replacing the entire ESC (most costly option) with a VESC? I'm guessing there is some reasonably priced and reliable product out there, but my search attempts have failed so far.

Thanks! :sunglasses:
```

---
## \#2 Posted by: JohnA Posted at: 2017-12-09T18:58:20.884Z Reads: 83

```
Basically the PWM output of the receiver is just a modulating voltage between 0 and 5 volts. You should be able to filter out the modulation with a capacitor. Here’s a link I found that went over doing this to an arduino’s PWM output. https://provideyourown.com/2011/analogwrite-convert-pwm-to-voltage/
You could also have the receiver output the PWM to an arduino nano (I’m sure there’s a tutorial out there on how to do this), and then have the arduino nano output via one of its AO pins. This could give you the ability to define throttle curves and even integrate switches so the board knows when you are on the board or have fallen off.
```

---
## \#3 Posted by: Canuck Posted at: 2017-12-11T04:25:11.032Z Reads: 50

```
Thanks for the info! That is definitely helpful. It appears adding a low pass filter consists of both a resistor and capacitor of appropriate value:

<img src="/uploads/db1493/original/3X/0/2/0203c0044373ed1d0a14deb99de55d1aed252148.jpeg" width="358" height="305">

The potential drawbacks mentioned appear to be undesired variability in the voltage signal and delayed responsiveness, which could be bad for e skate, depending how significant. 

One thing comes to mind though, is the RX signal actually PWM or is it PPM? My admittedly low level understanding of the two protocols makes me think that a low pass filter would not work for PPM as opposed to PWM, which makes sense intuitively to me.
```

---
## \#4 Posted by: ThermalM16 Posted at: 2017-12-11T04:34:39.829Z Reads: 42

```
What about using an inductor instead. Those are all I see being used for converting digital to analog in the Macbooks I work on.
```

---
## \#5 Posted by: Canuck Posted at: 2017-12-12T03:38:19.406Z Reads: 29

```
I’m still learning, but it seems that when the RC world refers to PPM it is not actually true PPM but rather a multiplexed PWM. If this is the case with the GT2B, then a low pass filter may work.

I came across [this](https://www.allaboutcircuits.com/technical-articles/low-pass-filter-a-pwm-signal-into-an-analog-voltage/) article which describes a "two-pole" low pass filter which incoporates an inductor:

<img src="/uploads/db1493/original/3X/4/2/423c7fefc9b710a81ce815f401e35cd0742cf3ea.jpeg" width="446" height="188">

The benefit of a two-pole filter is improved voltage stability and response time over a one-pole.
```

---
## \#6 Posted by: Canuck Posted at: 2017-12-12T04:53:58.423Z Reads: 23

```
The more I look at this, the more it seems like a microcontroller like an arduino will be the best solution. I have virtually no experience programming however, so this will be another thing to learn.
```

---
