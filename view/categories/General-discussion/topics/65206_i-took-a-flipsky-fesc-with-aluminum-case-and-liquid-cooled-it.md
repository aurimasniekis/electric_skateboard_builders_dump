# I took a Flipsky FESC with aluminum case and liquid cooled it

### Replies: 21 Views: 703

## \#1 Posted by: chuttney1 Posted at: 2018-08-17T20:30:12.357Z Reads: 287

```
https://youtu.be/MCtxwAEVzBY

After researching the use of mineral oil for cooling PC components published here on Youtube. I apply that knowledge to this project and it works as expected. I just wanna give thanks to Flispky for making an enclosure because I know this was possible even if the intended purpose of the product is not marketed as. 

I still ran into issues with the push button switch and corners of the XT90 connector leaking and some of the holes need to be sealed. It was originally designed to be waterproof. It was not designed to hold liquid contents but I think I debunked if this controller can be considered waterproof if I can dunk this in water for an extended period of time.
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-08-17T20:34:52.124Z Reads: 279

```
Do you have a Bluetooth module to test the temp difference between with and without?
```

---
## \#3 Posted by: skatardude10 Posted at: 2018-08-17T20:48:17.598Z Reads: 259

```
Neat, keep it up, but at the same time (hopefully constructive criticism time) I don't really see the point. Wouldn't the oil need to be circulated to conduct heat more effectively? 

If you could get the oil circulating, I almost feel like it would be cool to liquid cool a vesc with aluminum chassis (maybe loaded inside with thermal pads instead of oil for ease) and a liquid cooling pump and two radiators mounted to the rear of your board for natural airflow while riding. It would look super cool too, almost like the back to the Future car, but a skateboard... LoL.
```

---
## \#4 Posted by: hyperIon1 Posted at: 2018-08-17T20:52:28.588Z Reads: 230

```
Very interesting stuff. Really makes you think.
```

---
## \#5 Posted by: chuttney1 Posted at: 2018-08-17T20:55:35.786Z Reads: 223

```
I got first version of @rpasichnyk Bluetooth module, but I don't know the pinout for V6.6 since I'm using it on VESC V4.7. I actually prefer not to keep it inside because the case can act like a faraday cage.
```

---
## \#6 Posted by: chuttney1 Posted at: 2018-08-17T21:00:25.312Z Reads: 210

```
[quote="skatardude10, post:3, topic:65206"]
I don’t really see the point. Wouldn’t the oil need to be circulated to conduct heat more effectively?
[/quote]

I have no intention of running oil cooling lines as I believe having the case exposed to the air provides enough cooling. Plus moving side to side does get the oil moving.
```

---
## \#7 Posted by: Brdchris Posted at: 2018-08-17T21:08:56.623Z Reads: 200

```
What happens when this heats up? With no where for the pressure to relieve itself I imagine this is going to leak out any seals.
```

---
## \#8 Posted by: Vanarian Posted at: 2018-08-17T23:16:36.333Z Reads: 164

```
I had the same fucking idea one year ago and was faced with the same question : does movements of the board suffice to circualte the mineral oil inside ? Was even considering pulling an electric cooler with the mineral oil in order to provide "negative" temps. 

Thank you for bringing this to life ! I'll follow this, it's also a nice way to prevent moisture on components.
```

---
## \#9 Posted by: brenternet Posted at: 2018-08-17T23:20:26.299Z Reads: 161

```
Most sealed coolers will pump the oil to a radiator to dissipate the heat, I suppose the case is doing that job but volume of oil would eventually be overcome with heat.

It's a great proof of concept!
```

---
## \#10 Posted by: Jmding Posted at: 2018-08-17T23:39:03.832Z Reads: 154

```
Maybe if you find that circulation is inadequate, you could put in a couple buoyant plastic balls that will "float" around as you accelerate / turn, to help agitate and circulate the fluid?

Are you planning on increasing the max current draw to "over clock" your esc?
```

---
## \#11 Posted by: Hummie Posted at: 2018-08-18T01:19:48.288Z Reads: 135

```
super cool.  buuuut looking for possible problems do you think maybe this would be transferring heat from hot spots to bits on the board that wouldnt do so well with the heat.  maybe the oil moves its way right over to some more delicate temp sensitve stuff, no?
```

---
## \#12 Posted by: Trdolan03 Posted at: 2018-08-18T02:18:12.026Z Reads: 115

```
I am just wondering how to back up the benefit of this with numbers
```

---
## \#13 Posted by: chuttney1 Posted at: 2018-08-18T02:23:41.730Z Reads: 115

```
[quote="Hummie, post:11, topic:65206, full:true"]
 do you think maybe this would be transferring heat from hot spots to bits on the board that wouldnt do so well with the heat. maybe the oil moves its way right over to some more delicate temp sensitve stuff, no?
[/quote]

The consumer grade SMD components have a max of 125°C and military/medical/mission critical stuff have max of 150°C or higher depending on specs. There really isn't any component on this board that's super sensitive for the CANBus chip, STM32F405RTG6, AD8414, and DRV8301.
```

---
## \#14 Posted by: chuttney1 Posted at: 2018-08-18T02:35:26.628Z Reads: 125

```
[quote="Trdolan03, post:12, topic:65206, full:true"]
I am just wondering how to back up the benefit of this with numbers
[/quote]

You don't calculate. You just do it...

Actual answer is there is only a slight benefit, but for the average user the thermal silicone pads are more than enough for your needs. I get to cool the DRV8301 chip on both sides which is what I wanted to do on my VESC derivative. Texas Instruments' recommendation on drilling 0.3mm into the PCB for ground pad is effective for cooling. The oil just helps transfer heat to a larger surface area via thermal conductivity. 

Realistically, I'm only expecting temps to max around 60°C to 65°C on full load with the 85°C thermal throttling in the settings.
```

---
## \#15 Posted by: uigiroux Posted at: 2018-08-18T02:36:08.393Z Reads: 121

```
This reminds me of some special type of ferro fluid I read about that is apperantly used in bike hub motors.  I know it's a totally different concept, but was curious if anyone has tried this in an Esk8 as it would work exactly the same just a smaller version?

https://lunacycle.com/luna-ferrofluid-statorade-hub-motor-coolant-10ml/#ProductReviews
```

---
## \#16 Posted by: trancejunkiexxl Posted at: 2018-08-18T02:47:40.951Z Reads: 114

```
I might try a peltier.. Still thinking about it. Not efficient
```

---
## \#17 Posted by: Hummie Posted at: 2018-08-18T03:08:08.385Z Reads: 110

```
that stuff needs to be in a sealed motor which are maybe never used for boards.  

 i wouldnt call it a totally different concept though and its pretty similar in its approach to transferring heat with a liquid just this is ferofluid and magnetic.  i think just using mineral oil was also used in motors with good results but not as good.
```

---
## \#18 Posted by: uigiroux Posted at: 2018-08-18T06:04:25.769Z Reads: 94

```
Lol oh yeah I totally spaced on the whole sealed motor aspect haha...  I thought the fluid did more than cooling though with its magnetism somehow effecting the performance of the motor, like how the gap between the stator and the magnets works.  Meaning the smaller the gap the better...  Regardless, off topic so I'll stop there haha :smile:
```

---
## \#19 Posted by: Nordle Posted at: 2018-08-18T06:33:28.225Z Reads: 87

```
and once the oil gets hot?
```

---
## \#20 Posted by: Hummie Posted at: 2018-08-18T06:37:27.475Z Reads: 88

```
the oil gets hot but it fills the voids between the hot bits and the aluminum case and is better able to transfer the heat than a gas to that case.
```

---
## \#21 Posted by: Nordle Posted at: 2018-08-18T06:41:50.301Z Reads: 82

```
sure didn't think about that, stupid me...
```

---
