# Two selfmade VESCs

### Replies: 16 Views: 946

## \#1 Posted by: nordlicht Posted at: 2018-02-16T13:10:38.818Z Reads: 265

```
Hi,
I am repairing an electric longboard in terms of my work at the university (can you believe my luck?) because the old controllerboard broke. The old controller was from those balance-boards, the HUB motors aswell. TBH it's quite a cool concept to recycle the old motors, but the controller was shit anyway.
My uni also started to build VESCs on their own for several electric vehicles, so I wired the VESCs up and connected a test motor.

I started the BLDC tool and connected the VESCs, both seemed to work and had a connection. Software version 2.18. When I wanted to auto-config the motor parameters, the motor spun immediatly when I plugged the motor cables in **controller A**. When I plugged the motor cables into the **controller B** it didnt do that. Than I just read the config from **controller B** and wrote it to **controller A**, but with controller A the motor still starts spinning immediatly.
To clarify: **Controller A** spun up **without trigger pulled**, when I pulled it, the rotational speed changed.
Controller B didnt spin up at all.
That happened WITH cloned settings.

Has anyone a clue where to start looking?
Thanks in advance!
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2018-02-16T13:13:57.783Z Reads: 259

```
Bad throttle settings?
```

---
## \#3 Posted by: longhairedboy Posted at: 2018-02-16T13:15:24.438Z Reads: 256

```
just to clarify, you ran motor detection on VESC A with Motor A and it worked, but when you ran detection on VESC B with Motor A it wouldn't spin up at all?
```

---
## \#4 Posted by: nordlicht Posted at: 2018-02-16T13:21:53.571Z Reads: 243

```
Thats correct. I used to same motor.
I think I wasn't clear, gonna correct that in the OP:
**I DID NOT PULL THE TRIGGER TO DRIVE**. The controller A spun up even tho the trigger wasnt pulled. When I pulled it, the rotational speed changed.
The controller B didnt spin up at all
```

---
## \#5 Posted by: longhairedboy Posted at: 2018-02-16T13:39:45.423Z Reads: 228

```
yes. That's a PPM signal issue. That's my guess, anyway. Even if you don't have the trigger pulled, if its set wrong, it can think its supposed to be spinning.
```

---
## \#6 Posted by: nordlicht Posted at: 2018-02-16T14:17:21.577Z Reads: 213

```
I had an oscilloscop hooked on my PPM signal since I programmed it myself with an arduino via Bluetooth and that was my first guess aswell.
The positive pulse length was always 1.50ms with a rate of 50Hz.
The pulse length of the original PPM was for "position-zero" 1.48ms, but due to limited options in the arduino I was fine with that. I really dont think that the 0.02ms are an issue, but I can check it out next monday.
So far I would like to gather some idea =)

Edit: Whats ment witrh "bad throttle settings"?
```

---
## \#7 Posted by: longhairedboy Posted at: 2018-02-16T14:46:17.000Z Reads: 170

```
[quote="nordlicht, post:6, topic:46578"]
Edit: Whats ment witrh “bad throttle settings”?
[/quote]

its another way of saying "PPM Issue"
```

---
## \#8 Posted by: krloz Posted at: 2018-02-16T15:18:08.295Z Reads: 152

```
Even if you feed the same ppm signal to both vescs. If one is configured to have its centre, no gas, position at say 1.5 and the other one at 1.3. One will be static and the other one would be spinning
```

---
## \#9 Posted by: nordlicht Posted at: 2018-03-14T16:52:27.401Z Reads: 119

```
Sorry guys, the project was put on ice for a while, thats why I didnt respond.

So what you write about the throttle settings makes perfect sense! But I am supposed to check on a different VESC now, and I cant seem to read the PPM signal. I programmed an arduino to just go from 0% to 100% and than hold for 5s at 50%. Some basic programm to check if the VESCS handle the PPM same.

But one VESC doesn't show under **App Configuration -> PPM** just a static input of 50%, like no cables are connected, even tho I ticked he **Display** tickbox. The other one behaves like it should

Does that mean PPM doesnt work on the VESC or did I maybe miss some options?
Input voltage is 17V, Cutoff start is 10V, max is 57V, so that shouldn be an issue.

Cheers, thanks for your time,
Nordlicht
```

---
## \#10 Posted by: b264 Posted at: 2018-03-14T17:04:03.208Z Reads: 105

```
Make sure the PPM cable isn't turned the wrong way.
```

---
## \#11 Posted by: nordlicht Posted at: 2018-03-14T18:38:14.308Z Reads: 94

```
Thanks, made sure of that. Any other ideas?
```

---
## \#12 Posted by: b264 Posted at: 2018-03-14T20:37:45.094Z Reads: 78

```
Make sure real time data is enabled and the application is set correctly
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2018-03-14T22:18:45.192Z Reads: 64

```
Did you check if pin 57 of U1 (MCU) and R5 were properly solder, and if it was 2.2k
```

---
## \#14 Posted by: nordlicht Posted at: 2018-03-15T13:48:29.238Z Reads: 50

```
> Make sure real time data is enabled

Do you refer to the "activate sampling" tickbox in the "realtime data" tab? Or how do I activate realtime data?

Ok. I just spoke to a person who is close to those manufacturing these boards and they said, that most of them come without PPM input. Why so ever, I have no clue.
I guess I have to use the ADC now. Is there a way to use ADC also for breaking? If not, how can I use the motor for breaking while using the ADC?
```

---
## \#15 Posted by: b264 Posted at: 2018-03-15T16:27:41.730Z Reads: 40

```
[quote="nordlicht, post:14, topic:46578"]
Do you refer to the “activate sampling” tickbox in the “realtime data” tab?
[/quote]

Yes

[quote="nordlicht, post:14, topic:46578"]
most of them come without PPM input.
[/quote]

Just select an Application to use in the settings, use "PPM and UART" or just "PPM" if you won't be using a bluetooth module.

Remember every screen click "Read configuration" first and then "Write configuration" before you leave the screen
```

---
## \#16 Posted by: nordlicht Posted at: 2018-03-15T21:26:22.028Z Reads: 29

```
I checked the resistor, it had the value if should. The soldering also looked fine on the chip, but since I found the specific leg (is that the right term you use in english? not sure) of the ARM uC it was easy to check if the signal was there. It wasnt. But the RC- element was fine, the signal was smoothened (not sure about the term again here - sorry), so I "simply" (it wasnt simple at all :grimacing:) soldered the end from the RC element to the according leg of the ARM and it worked like a charm. Looks terrible tho.

If anyone should have a problem like that ever: I used varnished copperwire (as thin as a hair), its a pain to solder it, but anything thicker would be even harder.

Thanks a lot for your help!
```

---
