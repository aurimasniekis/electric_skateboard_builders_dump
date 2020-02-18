# Help Needed! BMS wiring

### Replies: 4 Views: 366

## \#1 Posted by: Trdolan03 Posted at: 2018-04-23T03:10:19.437Z Reads: 100

```
Hello,
I have a battery pack made out of 20 1s 5ah cells from hobbyking. I have 2 questions. I am discharging them individually on my iMax B6 equivalent charger and the voltage is sagging .1V on a 1a draw. They are rated at 20C. Is this normal? Will there be this significant voltage sag when riding/accelerating?
My second question is about BMS wiring. I created 2 packs of 10 batteries in series and then wired those packs in parallel. If I have just 1 BMS, how would I wire this? We can use this BMS for wiring purposes: http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html
Link to batteries: 
https://hobbyking.com/en_us/turnigy-5000mah-1s-20c-lipoly-single-cell.html?___store=en_us
```

---
## \#2 Posted by: Namasaki Posted at: 2018-04-26T14:12:49.517Z Reads: 73

```
Any 5ah 20C Lipo will have substantial voltage sag. 
Putting them in parallel will help some but still 20C is low even for a 10ah Battery.
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-04-26T14:58:26.675Z Reads: 70

```
5ah 20C means they are rated for 100a discharging
```

---
## \#4 Posted by: Namasaki Posted at: 2018-04-26T15:08:20.978Z Reads: 60

```
That is not a true equation. 

In reality it’s more like this:
AH x C / 3
5 x 20 / 3= 33a continuous current

Any amount of load will cause some voltage sag and the closer your load is to the true max the greater the sag will be
```

---
