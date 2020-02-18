# DIY Remote for VESC

### Replies: 11 Views: 1515

## \#1 Posted by: ThomasLefort Posted at: 2017-04-28T09:12:29.495Z Reads: 216

```
Hello everybody,

I'm a student in engineering and like many of the members of this forum, I made my electric skateboard entirely : 

<img src="/uploads/db1493/original/3X/0/8/080aaa81d8f00d86d74949f7a55a1d9a79daa5e3.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/4/047d9a9cf9604a6f47db4f479d46e7b5ad3e7004.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/b/1/b1d364fdb453473fe6ae6dd2994f2d4822fbe4ab.jpg" width="666" height="500">

But I wanted a really easy to use, reliable and functional remote. So I worked on an DIY remote, and after many version, I finally did this : 

<img src="/uploads/db1493/original/3X/a/9/a9ecdcea3cb2331bd1d3b94945bbf936bf9f22c3.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/6/5/655d5e496a455f37eaf2ee9a1275457eadc0ad03.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/6/4/64cb2f55234973207a2e9772b2711cffdc7be3bd.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/9/e9436a2eb20afaf3487be0eb8b0011e7b83989c7.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/6/0/60e1d9881f6c08a030bea63adece78a7bd56e7f5.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/6/762994d26eb1b9d6f64c90444541ff20481ac6be.jpg" width="375" height="500">
The code is based on the library written by RollingGecko : https://github.com/RollingGecko/VescUartControl
I modified lots of thing but their is part of the code, like the interface and the battery percentage calculation that I entirely keep like this because he made an incredible work.

The body is 3D-printed. I have a 300$ cheap 3D printer. The external quality of the print isn't good but I don't work lore on that because I just want it to be functional. I designed the PCBs and send to OSHPark to manufacture it.

At this state, it cost me around 100$ because of the different version. The last version cost 60$ but in this price I still have PCB that I don't use for the moment.

It shows different information like the speed (approximation), the battery voltage, the battery percentage (calculated with the battery voltage), the distance (approximation), the max speed, the current in the motor, and the overall distance (it keep all the distances in memory).

It is super fun to use and very reliable. I never had disconnection even if my controller is on a waterproof box beside the board. It was a lot of work but It worked !

If you have quick questions, I can help you, but I don't have enough time to make an entire tutorial and to clean my code to be useable by everybody. I made this post to give ideas if some people want to make something similar.

PS : I apologize if their is things that you don't understand. I'm bad at writing in English. 

Good ride !
```

---
## \#2 Posted by: jaysoncena Posted at: 2017-04-28T09:26:46.097Z Reads: 188

```
Cool setup!

What transceiver did you use? What data is communicated on it?
```

---
## \#3 Posted by: ThomasLefort Posted at: 2017-04-28T09:53:42.427Z Reads: 186

```
I use a 2.4 GHz module. The basic NRF24L01. And I described all the data that it shows but I basically transfer all the data that we can get from the VESC from the UART port. The data structure that we can get looks like this : 

typedef struct {
    float v_in;
    float temp_mos1;
    float temp_mos2;
    float temp_mos3;
    float temp_mos4;
    float temp_mos5;
    float temp_mos6;
    float temp_pcb;
    float current_motor;
    float current_in;
    float rpm;
    float duty_now;
    float amp_hours;
    float amp_hours_charged;
    float watt_hours;
    float watt_hours_charged;
    int tachometer;
    int tachometer_abs;
    mc_fault_code fault_code;
} mc_values;

I also put some temperature sensors on the board to check the battery temperature but it is used only for safety so I don't show them. And you can add many different sensors because the transmitter and the receiver are based on Arduino Nano. It is some code to change.

Some ideas I had :  

*  Put an SD card to record data from different rides
*  Put a GPS to record rides and show them on computer then. And it give more precise values for speed and distances, if you get the connection.
* I have a screen on my board as you can see on pictures. At the begin I put it because I didn't put one on the remote. But now I use it to show the battery percentage so I can check it without the remote.
* Create a DIY BMS to make the charge easier and to monitor the battery more precisely
```

---
## \#4 Posted by: Okami Posted at: 2017-04-28T11:43:52.007Z Reads: 144

```
Can you describe in a bit more detail how you apply acceleration / brake on the remote?

I see you have 2 triggers there.. so does 1 work for acceleraton and the 2nd for brake?

For switching display modes, I see you have 4 buttons on the other side of the remote..

---

I was thinking the other day what would be the most precise / ergonomic way to control acceleration brake.. and at one point I actually thought about similar like you have made.. '**'thumb controlled lever''**

So yeh, interested to hear what you can say about it..
```

---
## \#5 Posted by: ThomasLefort Posted at: 2017-04-28T12:11:26.870Z Reads: 134

```
Sorry I forgot to explain this in details. The left triggers is for acceleration and the right one for brake. Brake has the priority over acceleration. For the moment, I don't find a better solution than elastic to home the triggers.

There is 4 buttons : 2 to switch the display (forward and backward), one to change the direction of the motor, and one for cruise control. I send information to the VESC like if it was a nunchuck.

I wasn't expecting a so good results with thumb controlled triggers. Your are sure that if you pressed the brake triggers, it will really brakes. And each one of the triggers has a wide range of movement. It make the control really smooth. 

I never skate before and I was wondering to concentrate on the road and on the command at the same time. I immediately forgot the remote when I started with my electric skateboard.

My first remote was a nunchuck with a bad ESC and I was afraid to be eject from the board every seconds...
```

---
## \#6 Posted by: Okami Posted at: 2017-04-28T12:16:13.641Z Reads: 114

```
[quote="ThomasLefort, post:5, topic:21945"]
and I was afraid to be eject from the board every seconds...
[/quote]

Totally understand you here :smiley:
Yeh, so it looks like the ergonomics of the triggers have come out very nicely for your design / remote..

Would love to test it out (the remote) one day in real life to see how it feels..

I also think a lot of ''magic'' is trapped in the way trigger comes back - how tight the spring / elastic band is.. 

Trigger for my mini remote seems to be a bit soft and I find that this sometimes might not give the best precision needed.. GTB's for that reason seem to be more firm, even if I havent tried one yet in my life :)
```

---
## \#7 Posted by: ThomasLefort Posted at: 2017-04-28T12:22:23.544Z Reads: 103

```
I had lots of luck with this elastic. They are tight enough to be unable to move them with a bit of force. And when I brake or accelerate I feel where I am because the tension grow. But it is still easy to move. 

I should try to find a better solution for this but as it worked like a charm I let it like this for the moment.
It would be better if the homing system was integrated inside the remote.
```

---
## \#8 Posted by: Okami Posted at: 2017-04-28T12:37:34.490Z Reads: 104

```
yeh, nice that it works as it is now!

Hard to say will you find a good ''substitute'' for the elastic band.. I remember from other projects on the internet, it is sometimes hard to replace the elasticity of rubber band with similar spring or other ''spring'' material, to make it bounce back in the same way as elastic band does..

Maybe someone who has dealt with a lot of spring mechanisms can help out to find the best 'substitute' to make the feeling of tension the same..

--

Though, as long as these elastic bands dont wear out or break apart, I assume it is okay (safe) to use them :)
```

---
## \#9 Posted by: Sander Posted at: 2017-04-28T21:49:33.531Z Reads: 89

```
Very nice remote!
I have done the same, just inside the winning remote ;)
All you need is just some more time spending in a circuit maker so you can make it smaller!
```

---
## \#10 Posted by: ThomasLefort Posted at: 2017-04-29T19:33:47.733Z Reads: 69

```
The winning remote ? I don't understand what you think about.

Yes, I could have made it smaller but I let it like this because I think that it is more confortable to hold. And every component are soldered on a flat 2 side PCB. I create lot of constraints for the general shape but it make the remote more reliable.
```

---
## \#11 Posted by: Sander Posted at: 2017-04-29T19:50:46.528Z Reads: 68

```
What I meant with the WINNING remote was that I built it inside of it, with oled etc.
[quote="ThomasLefort, post:10, topic:21945"]
Yes, I could have made it smaller but I let it like this because I think that it is more confortable to hold. And every component are soldered on a flat 2 side PCB. I create lot of constraints for the general shape but it make the remote more reliable.
[/quote]

Well more comfortable is better ;)
```

---
