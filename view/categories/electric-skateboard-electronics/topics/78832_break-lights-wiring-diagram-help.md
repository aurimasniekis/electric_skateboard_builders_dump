# Break lights wiring diagram help

### Replies: 8 Views: 458

## \#1 Posted by: ggalisky Posted at: 2018-12-24T02:46:37.895Z Reads: 120

```
Hello all, 

I am trying to build a head light and tail light system for my up coming build. The picture below is my wiring diagram. I am using the two 5v 1a power ouputs on my focboxs to power the strips. I will be using 10 inches of this led:https://www.adafruit.com/product/1138?length=1 . 10 inches of this led tape at max power consumption is around 900mA, so I was thinking of wiring the 5v 1A power ouputs on my focboxs in parellel to stay safe and not over load either focbox. The AT Tiny 85 will be programed to read the PWM values from the reciever and detect if I am breaking. The 3 position switch is to switch between day time mode, night time mode, and rainbow mode. The other switch is to turn the whole system on or off. 

My main question is about whether wiring the 5v 1A outputs on the FOCBOXs in parallel will cause and issues. If it does cause issues could I use a diode on the 5V 1A output on one of the focboxs to fix this issue. 
![Capture000|690x376](upload://lo202XUph98Ahv06ldfZ3Id0OwT.jpeg) 
Thanks!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-12-24T10:32:25.085Z Reads: 92

```
not sure if it's an issue BUT, you'd be better off using a separate power supply using a step down converter. you'll choke the vescx far less and won't have to worry
```

---
## \#3 Posted by: Sedmii Posted at: 2018-12-24T11:43:58.576Z Reads: 89

```
Even if this converters support parallel connection, it is generally a bad idea to do this. Slight variations in voltage would cause high current flow trough one of the converters, beside this there are more reasons this is not advisable. 
I think you may have wrong calculations about current draw. How many leds do you have on your strip lenght. If this is true, maybe your FOCBOX wont be overloaded.
But if you really need over 1A current do as @mynamesmatt said. Separate step down is a better idea because you dont want to risk your FOCBOX over something this trivial.
```

---
## \#4 Posted by: ggalisky Posted at: 2018-12-25T04:19:46.938Z Reads: 68

```
What would be a good option to power them? I have a 3s 1p pack and a 10s 4p pack that I have on the board currently. What would I use to step down the voltage? What would you all recommend? Thank you for taking the time to reply!
```

---
## \#5 Posted by: ggalisky Posted at: 2018-12-25T08:04:06.143Z Reads: 63

```
https://www.ebay.com/itm/Turnigy-HV-High-Voltage-SBEC-BEC-High-Input-5A-5v-6v-Switch-Regulator-8-42V-in/302310059628?hash=item4663156e6c:g:JisAAOSwONBZEMhl

This would probably work
```

---
## \#6 Posted by: StefanMe Posted at: 2018-12-25T12:19:58.456Z Reads: 48

```
Definitely use an step down or something. Otherwise u only will get problems.. specially freeze your ATTINY.

U use an LM2576HV to do this job.
https://www.youtube.com/watch?v=tp5KQ5WFtwQ
https://www.electric-skateboard.builders/t/haya-integrated-deck/68132/909?u=stefanme
```

---
## \#7 Posted by: ggalisky Posted at: 2018-12-25T16:08:31.122Z Reads: 43

```
What remote did you use to allow for switching like that? I currently have the nano X and it only has acceleration, breaking, and a button in the side that does do anything. Do you mind sharing alittle bit about how you setup your break lights?
```

---
## \#8 Posted by: StefanMe Posted at: 2018-12-25T16:13:16.889Z Reads: 44

```
https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084/54?u=stefanme

I created my own remote... including a PCB with outputs and step-down ect.
```

---
