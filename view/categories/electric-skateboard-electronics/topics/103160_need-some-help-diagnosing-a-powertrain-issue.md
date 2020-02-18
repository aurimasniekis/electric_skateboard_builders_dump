# Need some help diagnosing a powertrain issue

### Replies: 6 Views: 113

## \#1 Posted by: doejersey Posted at: 2019-10-21T00:52:46.699Z Reads: 34

```
Howdy,

Ive been working on a DIY board for a while. I had some very specific goals for the build hence the wonkiness of my set up. I thought I was being clever but I guess not. First off I'm running 2 10s1p batteries from ElectricSkateboardParts.com (Thanks friend) this way both batteries can be carried onto a plane without incident. In theory this meant I have a 10s2p setup with 40A discharge continuous. Which should be fine for a flight safe commuter board for traveling.

I'm running a torque boards 6374/190KV motor, (single motor setup) with I believe 14/36 teeth. (I might be a little bit off on this one but I can't exactly remember). 

I was previously using a Flipsky ESC V4.12 but when I attempted to adjust the settings on the device I could never get the settings to save. It would either magnetically lock the motor when I would throttle up, or I'd get an error and it would fail to save. 

So, frustrated I got an ownboard ESC figuring that it would be preset with everything and I could just plug and play, even if it wouldn't be the most optimal setup. So I finally get it from China, and I hook everything up. Everything looks fine, remote binds, esc powers up, etc but when I throttle up the motor spins super slow and with so little force that you can pretty much just stop it with your paws. 

So I'm an idiot and somewhere along the line I messed up. But could some one please help me figure out where? I'm getting super frustrated and may just get a prebuilt for flying at this rate. Thanks ahead of time!

![IMG_20191020_203129|690x325](upload://pPUnr7F58Ql5IpEGtBuUf4CDnSx.jpeg)
```

---
## \#2 Posted by: Paulycnotes Posted at: 2019-10-21T02:27:40.903Z Reads: 29

```
Hey bro you are using a own board ESC which is completely different and made for Hub Motors which is why your motors are running slow based on the murders you're currently using I take it you're not using hubs and I actually had that same ESC and ran into that same problem but if you look closely it says 70 KV on the own board ESC which would be a high KV for Hub motor but not for pulley.
```

---
## \#3 Posted by: doejersey Posted at: 2019-10-21T21:09:13.922Z Reads: 22

```
Really. I'll double check that when I get home. I figured it would be fine since own board offered a pulley set up now. But yea maybe I was wrong or ordered the hub motor one. 

Either way appreciate the reply. You wouldn't believe how frustrated I am considering the multi week shipping timelines on Chinese distributors. Do you have a suggestion on ESC? Like I said in OP I was using the Vesc v4.12 but I ran into a lot of issues with the software.
```

---
## \#4 Posted by: Schulerbible Posted at: 2019-10-21T21:44:13.391Z Reads: 18

```
What issues did you have with the software?
```

---
## \#5 Posted by: doejersey Posted at: 2019-10-21T22:36:26.186Z Reads: 17

```
I posted a bit above. But I would get issues with the software not detecting the Vesc. Then I would have issues where once I got some baseline settings saved to the Vesc the motor was just magnetically locked and would never spin no matter what I did. The Vesc Software itself seemed functional (I didn't get any crashes or anything). There just wasn't a ton of help online when I googled around.
```

---
## \#6 Posted by: Schulerbible Posted at: 2019-10-22T06:58:02.121Z Reads: 14

```
Do you know someone who could help with the Flipsky or potentially diagnose if it's broken. If the unit has an issue I bet you will get a replacement esc. Other than that, the Hobbyking Vesc works just fine and has a decent price.
```

---
