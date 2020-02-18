# Advice for my VESC 6.6

### Replies: 11 Views: 349

## \#1 Posted by: kchxaz Posted at: 2019-03-26T05:10:20.109Z Reads: 120

```
Hi guys,

So I just received my VESC 6.6 and before I get all excited and start doing stuff to it I thought I would ask those who have gotten one in the past I noticed it is wrapped in a heat shrink, while far from water proof or even resistant maybe I should leave it on to give it "some" protection, if not moisture then at least dust or wayward wires that might do (whatever)...I do know that in order to program it I'll need to gain access to the USB which is under the plastic, so I'll need to carefully cut a hole to gain access to that.

I do notice that the vesc has a 6 wire hall sensor connection where my motors have 5 wires for the sensor - how can this work? Does the 6th wire connect to one of the 5th wires or is it just not needed?

Lastly and most importantly I didn't realize that this didn't come with a remote, what do I need to get to fill this gap? I notice that there is no antenna like with ESC's so what do I need to buy to fill in the remote part besides the actual remote? I see transmitter and receiver spots on the VESC so what do I need and where to get it?

Thanks!
```

---
## \#2 Posted by: jun1208 Posted at: 2019-03-26T05:22:05.059Z Reads: 114

```
Hey Kerry :slight_smile:

Yes you will have to cut a hole on the ports you will be using (eg. USB/Bluetooth/PPM etc.) if you don't want to cut open the transparent heat shrink :+1: 

Regarding the hall sensor, I can't be sure about other brands but my Flipsky 6.6 came with a 5pin to 6pin JST cable in the packaging to use with Flipsky's motor so you just need to plug the cables accordingly.

And yes the remote is separate with the VESC, you can buy the latest VX1 from Flipsky or the mini remote which is the most commonly used esk9 remote in DIY :smiley:
```

---
## \#3 Posted by: wafflejock Posted at: 2019-03-26T05:26:03.529Z Reads: 108

```
Controller input is configured in the "VESC Tool" software get it here https://vesc-project.com/
You can basically use any standard RC controller I have my own trigger based design I use there are a few nice wheel based ones (if you're into 3d printing and want to make your own everything), but also a few mentioned and other that are popular among esk8

The VESC also allows for nunchuk and analog (ADC) input

![Capture|231x485](upload://6EGXPA8GnYoje6CG6RLGFucvGjN.png) 

Basically after going through motor configuration wizard in there I go to app section and setup the endpoints for my remote input and am pretty much good to (might tweak motor amp settings so it isn't too crazy)
```

---
## \#4 Posted by: b264 Posted at: 2019-03-26T05:27:03.506Z Reads: 87

```
Heatshrink won't do anything for waterproofing.  Multiple coats of silicone conformal coating on all the parts that don't get hot is how to waterproof, and one coat of acrylic conformal coating on the parts that do get hot.
```

---
## \#5 Posted by: kchxaz Posted at: 2019-03-26T07:36:15.922Z Reads: 73

```
I got the Flipsky as well, but I think I got the one without the extra wiring and stuff (sold out). So I didn't get the adapter like you did. How does the 6 pin condense down into the five pin? Is there anyway to take a pic? I can't imagine fabricating one to be very difficult. 

Thanks for the comment!
```

---
## \#6 Posted by: kchxaz Posted at: 2019-03-26T07:39:29.630Z Reads: 73

```
Just got a can of aerosol Si conformal coating from amazon:+1:. Good advice to coat it with that stuff. I'm going to have to attach the receiver wires and stuff first of course but good advice. Thanks.
```

---
## \#7 Posted by: kchxaz Posted at: 2019-03-26T07:47:07.932Z Reads: 72

```
I'm pretty sure that I have the mini already, it came with a different ESC but what would I need to attach to the VESC to have it communicate with the remote (an antenna I know for starters)?
```

---
## \#8 Posted by: jun1208 Posted at: 2019-03-26T07:50:09.409Z Reads: 73

```
I can take a pic when I get back home later :slight_smile: this is the [sensor wires](https://flipsky.net/collections/accessories/products/flipsky-esc-sensor-wires) btw :+1:  

Did you get the [single](https://flipsky.net/collections/electronic-products/products/flipsky-fsesc-6-6-based-upon-vesc%C2%AE-6-heat-sink) or the [dual](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink) 6.6?

The remote you have is [this](https://flipsky.net/collections/accessories/products/2-4ghz-radio-transmitter-remote-controller-with-receiver)?
```

---
## \#9 Posted by: lrdesigns Posted at: 2019-03-26T08:12:04.714Z Reads: 63

```
The reason for six wires on the sensor plug is some motors have an extra wire for motor temperature. But most motors do not.
```

---
## \#10 Posted by: kchxaz Posted at: 2019-03-27T00:21:21.295Z Reads: 41

```
Yes, those are the 6 pin wires that came with my FSESC 6.6

This is the [remote](http://www.diyeboard.com/new-version-4-speed-mode-24ghz-remote-controller-rc6-for-eboard-p-666.html) that I have as well as [this](http://www.diyeboard.com/new-version-3-speed-mode-24ghz-mini-remote-controller-rc5-p-575.html) one too.

Thanks for the feedback
```

---
## \#11 Posted by: jun1208 Posted at: 2019-03-27T00:41:22.880Z Reads: 37

```
If you have the wires that I linked previously then just connect 1 end to the hall sensor cable on the motor and 1 end to the hall sensor port on the VESC :slight_smile:

As for the remote, those are remotes for Chinese binary ESC meaning they don't come with a separate receiver, you can't use them on VESC :slight_smile:

You need something like what I linked which comes with a separate receiver unit :+1:
```

---
