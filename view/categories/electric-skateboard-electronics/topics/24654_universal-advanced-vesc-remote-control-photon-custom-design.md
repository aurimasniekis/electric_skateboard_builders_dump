# Universal Advanced VESC Remote Control (Photon) - Custom design

### Replies: 1120 Views: 56389

## \#1 Posted by: Wajdi Posted at: 2017-06-05T22:14:05.810Z Reads: 2024

```
Hello everyone,

For the past months I have been working on this project on and off trying to design an advanced and compact remote control for diy electic skateboards/longboards. 

[img]http://i.imgur.com/Gae13xZ.png[/img]

After doing some research trying to find the ideal remote for my DIY build, I was disappointed by how basic and unreliable all the available remotes are.

Why have such an advanced ESC like the VESC if we can't really take advantage of it? 

So I decided to start from scratch and design the ultimate universal remote that is both feature rich, compact, and ergonomic. 
The purpose of this design is to allow DIY builders to have access to a top notch remote that competes with the big brands out there. 

[img]http://i.imgur.com/Zop9VrM.png[/img]
[img]http://i.imgur.com/Dpjba4S.png[/img]
[img]http://i.imgur.com/4DdBjoa.png[/img]
[img]http://i.imgur.com/J1jZvsO.png[/img]
[img]http://i.imgur.com/sS5doJ2.png[/img]



Without further ado, here is the design breakdown:

**Hardware:**
Custom designed PCB specifically for this project.

* Powerful and fast cortex M0 32bit microcontroller.
* Built in LIPO charger 
* Built in Piezo Buzzer for alerts
* Built in 2.4Ghz transmitter receiver with a ceramic antenna amplifier for an extended range and better reliability.
* Soft power latching, turns on and off with a single push button
* Micro USB for charging.
* 0.95" Color OLED display.
* Smooth joystick control.
* Three push buttons 


[img]http://i.imgur.com/K2yi34S.jpg[/img]
[img]http://i.imgur.com/rq6QeGw.jpg[/img]
[img]http://i.imgur.com/boExLmI.jpg[/img]

**Software:**
Custom designed software to take full advantage of your electric skateboard.

* Well designed user interface with an advanced gauge.
* Displays remote battery level
* Displays electric board battery level
* Failsafe neutral throttle in case of disconnection
* Total distance traveled
* Buzzer warning when battery is low
* Custom throttle acceleration and braking sensitivity - Instead of having only **3** predefined riding modes like most other remotes do, you can adjust both acceleration and braking sensitivity separately. From -10 to 10 each, allowing for around **400** possible riding modes.
* Predefined wheel and gear ratios for speed calculation
* Ability to turn the buzzer on and off
* Detailed stats about your board, voltage, amperage, etc..
* Option to turn board lights on and off if you have them installed.
* Units change -Mile/KM
* Assign a function to the custom push button( Light control, cruise control...).

[img]http://i.imgur.com/kDu4nFM.png[/img]
Quickly put together prototype.

**Case:**
Last but not least, a custom designed enclosure that is very compact, ergonomic, and very portable. Only about **4.4 inches** long/ **11.4cm** and **1.8inches** wide/ **4.6mm**

[img]http://i.imgur.com/nADavwG.jpg[/img]
[img]http://i.imgur.com/sFDDJ7C.jpg[/img]
[img]http://i.imgur.com/gmN0uYj.jpg[/img]


**Cost:**
The cost to produce a single unit right now is fairly high, but certainly cheaper than the evolve remote, it should be less than 120$ and if we manage to order a large batch then we can **reduce the cost significantly**. Remote cost will factor parts prices, assembly, as well as my personal effort and time spent designing the hardware, software, and the whole thing from scratch.


I'm currently in the final stage, everything was designed, assembled, and tested.
If you are interested in this project, please vote on the following poll so that I can have a clear idea on how to take things from here. 
[poll]
* Yes! Count me in.
* not interested.
[/poll]
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-05T22:27:49.328Z Reads: 1586

```
Amazing work! But I have a couple questions:

1. What does left/right on the joystick do, wouldn't it be easier to using if the controller only pivoted on one axis?

2. Why not go for a slimmer profile? Putting the remote in my jeans pocket is super convenient which is why I never opted for the classic "steez" remotes. For this, my benchwheel remote works perfectly for me.

3. I'm assuming this will plug into the UART port on the VESC? Does this also mean the remote will be operating on bluetooth? Have you tested reliability in network congested environments? This seems to be a common concern amongst bluetooth based controllers. If it is bluetooth, which version will it be running, 5.0?

4. More of a suggestion, but you should include a little lanyard loop on the bottom for people to attach landyards :)
```

---
## \#3 Posted by: Wajdi Posted at: 2017-06-05T22:50:42.661Z Reads: 1492

```
Thanks for your suggestions, to answer your questions:
1. The left/right on the joystick is used to operate different sections of the menu, like increase/decrease values. It is more convenient than mapping everything to buttons.
2. The design right now is actually pretty slim, only around 3 cm. I can barely squeeze a lipo in there :smiley: However I will keep that in mind and see if I can tighten things up a little more.
3. Yes you can plug the transreceiver on UART. And no the remote does not use Bluetooth. Bluetooth is not really suitable for critical operations. The remote uses a straight 2.4Ghz based on the nrf24l01 controller. It was proven to be very reliable. Bluetooth is needed when you want to send and receive data to mobile devices, which is not the case here since the purpose of this remote is to provide all the necessary stats you need without using a smartphone.
4. I agree! I actually had that in my todo list, should be done by the end of the day.
```

---
## \#4 Posted by: evoheyax Posted at: 2017-06-05T23:11:55.520Z Reads: 1359

```
I have to say that I love your work so far. Really inspiring stuff TBH. But I have a feww questions:

Is this data coming from the VESCs them selfs?
If so, multiple VESCS?
Assuming the answer to both of those is a yes, how do you get the data if your only connected via ppm for both data and control?
Do you need to modify the VESC firmware?
Are there any other catches or drawbacks?

Regardless, it looks nice and I can't wait to see more about it!
```

---
## \#5 Posted by: sl33py Posted at: 2017-06-05T23:16:31.450Z Reads: 1266

```
My #1 concern on 2.4 is reliability.  I continue to come back to the GT2b because of the frequency hopping (or whatever they call it), which has been the most reliable in high congestion 2.4 areas.  I can consistently get drops on others riding along Alki beach w/ wifi from condos along the path.

Love the idea and also curious around how it integrates with the data from VESC.  And is this expected to work with VESC 6?
```

---
## \#6 Posted by: Jinra Posted at: 2017-06-05T23:57:05.125Z Reads: 1179

```
A follow-up to 2. perhaps you can move the pcb sideways and have the screen parallel with your palm instead of perpendicular.
```

---
## \#7 Posted by: Wajdi Posted at: 2017-06-06T00:01:44.264Z Reads: 1165

```
Thank you. To answer your questions:
1. Yes the data is coming from the VESC, multiple VESCs should be no problem, though I didn't test it yet.
2. Packets are sent and received from the VESC in intervals, control packets are given a higher priority and sent at a higher rate, received data is coming  as an acknowledgement payload. 
3. No, the VESC has already the UART protocol implemented, all you have to do is connect the transreceiver to the UART port. The transreceiver ( not shown yet ) is small device that I developed based on the arduino nano, and it has the nrf module built in. The transreceiver comes with open digital and analog ports, as well as spi to control custom stuff on your board like lights.
```

---
## \#8 Posted by: Wajdi Posted at: 2017-06-06T00:17:09.998Z Reads: 1110

```
To solve congestion problems, I implemented a channel selection that lets you change your operating frequency if you ever find yourself in a noisy environment. Frequency hopping is a good solution and in fact it can be implemented using nrf24l01, all we have to do is rapidly switch frequencies using a predetermined random function, the only problem is that we have to ensure that both transreceivers are kept in sync.
Regarding VESC 6, I don't see why it wouldn't, as long as the new firmware keep the UART protocol.
```

---
## \#9 Posted by: lrdesigns Posted at: 2017-06-06T00:54:55.246Z Reads: 1085

```
Looks very cool. Could you offer an electronics only version for people who have 3D printers?
Can it keep track of total millage? I know that's a feature a lot of people want.

*Edit. I would feel much safer if the remote and transceiver had plug in external antennas, like in RC gear. Maybe not totally necessary on the remote but on the board antenna position can make a big difference to the reliability of the connection. Being able to move the antenna to good location is really helpful.
```

---
## \#10 Posted by: Decdog Posted at: 2017-06-06T00:59:49.069Z Reads: 1038

```
Finally!!! This remote looks awesome
```

---
## \#11 Posted by: Wajdi Posted at: 2017-06-06T01:27:31.459Z Reads: 1012

```
Thanks, yes it does keep track of total millage, I will showcase all the detailed features in an upcoming video.
About the electronics only version, I will consider that.
About the antenna concern, I have been testing the module extensively, and I didn't have a problem with reliability. I will keep your suggestion in mind, and maybe add an antenna port on the vesc side.
```

---
## \#12 Posted by: Jinra Posted at: 2017-06-06T01:39:04.050Z Reads: 951

```
just curious what was your riding environment? I live in SF and the 2.4ghz congestion here can get pretty crazy.
```

---
## \#13 Posted by: lrdesigns Posted at: 2017-06-06T01:47:01.448Z Reads: 966

```
Yeah I'm sure its reliable under most conditions but there is always rare circumstances. I use the GT2B and experienced some drop outs when going over tram tracks. But due to it having a fail safe set to neutral it just meant a temporary loss of power. After this I moved the receiver antenna from under my rear foot to the middle of the board and never had another dropout. People with carbon fiber boards need to be extra careful of antenna location. If your transceiver can have a fail safe it would be great, I think its a very good safety feature. 
@squad in another thread broke his arm real bad when going over a tram track with a nano remote, if it had a fail safe this probably would not have happened. [nano dropout](https://www.electric-skateboard.builders/t/full-diy-custom-electric-caster-board-emax-gt5345-maytech-12s-esc-10s-10ah-lipo/18902/43)
```

---
## \#14 Posted by: Wajdi Posted at: 2017-06-06T03:09:34.965Z Reads: 885

```
Nothing as crazy as SF that's for sure :smile:
```

---
## \#15 Posted by: Wajdi Posted at: 2017-06-06T03:12:54.819Z Reads: 914

```
Good point, actually the transceiver has a failsafe function, received packets coming from the remote are checked against a threshold timeline, if there is a delayed response, it sets the VESC to neutral throttle.
```

---
## \#16 Posted by: saul Posted at: 2017-06-06T03:22:58.241Z Reads: 929

```
nice work. where did you get that color oled? I can't find fully color for a decent price...
```

---
## \#17 Posted by: lrdesigns Posted at: 2017-06-06T03:31:17.442Z Reads: 958

```
Excellent! That should prevent worst case scenarios.
```

---
## \#18 Posted by: NAF Posted at: 2017-06-06T03:57:35.648Z Reads: 996

```
Absolutely amazing !!!!!!! .....but there is one design flaw...it needs KILLSWITCH !! Otherwise it's going to have the same most hated feature as EVOLVE remote.

Here is what I am talking about starts at 2:16:

https://youtu.be/7gGj57t9N8E?t=2m16s
```

---
## \#19 Posted by: saul Posted at: 2017-06-06T04:15:47.080Z Reads: 965

```
lol shit got real at 4 min! :joy:
```

---
## \#20 Posted by: NAF Posted at: 2017-06-06T04:18:54.779Z Reads: 956

```
Also what a about simple TURN by TURN navigation connected to the phone ? would that be possible.? having such an amazing color display it would be a pity not to have a simple navigation..
```

---
## \#21 Posted by: High-roller Posted at: 2017-06-06T04:27:32.522Z Reads: 884

```
Aaand following! Well done, it's so great to see more and more designs for a compact remote with all these features! 
One thing, could you possibly add some kind of trigger to the front as well for people who prefer that? It doesn't have to be very big and pointy (like the evolve trigger), just enough for the index finger to push/pull against. 
That way you can choose what control method you prefer, as they both have plusses and minuses, and whichever button you're not using for that can be switched to use for an auxiliary feature.
```

---
## \#22 Posted by: Eboosted Posted at: 2017-06-06T07:51:31.633Z Reads: 825

```
Please, please, please make a trigger throttle
```

---
## \#23 Posted by: NAF Posted at: 2017-06-06T08:43:35.548Z Reads: 818

```
I totally agree. Not only triggers are better ..they can have better form factor...much more slimmer.
```

---
## \#24 Posted by: Ronny_CTS Posted at: 2017-06-06T09:25:03.324Z Reads: 834

```
Fantastic work! Looks amazing!

I think that reliability should be the main concern. I've seen a few people on the forum posting pics of X-rays with broken bones as consequence of remote disconnect and acidental flyoff's due to instance braking of full throttling. Doesn't look fun at all.

I also agree that a trigger could be incorporated alongside the toggle switch. That way you could program both too work together as a kill switch. 

Just my 2 cents.
```

---
## \#25 Posted by: will_manners Posted at: 2017-06-06T11:03:55.928Z Reads: 816

```
Your remotes features and the development you've put into this certainly look amazing! Definitely something to admire, however the most important aspect of the remote first and foremost should be safety. Not just in terms of connection reliability but failsafes to ensure accidental inputs don't result in catastrophic injury.

The highest priority should be safety and I think the form factor you're currently going for makes it too easy for accidental inputs. The exposed trigger really should have a dead switch so that it only activates when the dead switch is pressed. Without it, triggers get caught on pockets far too easily and accidental inputs are a common occurrence from my limited experience with the mini remote, (it's the reason my board got ran over by a car). I think boosted has that shit down in terms of form factor, safety precautions and ease of use.

I'm not sure how others feel but with every other available diy remote on the market, enertions, mini remote, winning, none of them have a dead switch or a means of minimising accidental inputs.
```

---
## \#26 Posted by: Wajdi Posted at: 2017-06-06T16:59:13.889Z Reads: 754

```
I don't remember the exact place I got it from, I had for over a year but it wasn't cheap.
```

---
## \#27 Posted by: Wajdi Posted at: 2017-06-06T17:02:33.151Z Reads: 758

```
Turn by turn navigation will require a smartphone, and an extra Bluetooth module. I think most people use their boards to commute in common areas, adding navigation is an overkill in this instance. Perhaps in future versions.
```

---
## \#28 Posted by: Wajdi Posted at: 2017-06-06T17:06:20.969Z Reads: 752

```
Since many of you requested a kill switch, I'm adding one as we speak, it will be adjustable from the menu to be either "Keep pushing " or "Push once" to activate. I also added a lanyard hook :slight_smile:
```

---
## \#29 Posted by: Print3r Posted at: 2017-06-06T17:58:30.604Z Reads: 734

```
The grip looks very ergonomic ... but how do you see the screen when you grip the remote. Also, make sure the screen is not too cluttered - adding a settings/stats view might help reduce screen clutter for the riding mode. How fast is your screen refresh time - are you using SPI or I2C and what library? Looks great, what price are you thinking of?
```

---
## \#30 Posted by: zel Posted at: 2017-06-06T18:26:33.421Z Reads: 727

```
@print3r he said price right now is $120 but he wants it to go lower
```

---
## \#31 Posted by: okp Posted at: 2017-06-06T18:30:34.353Z Reads: 715

```
great work man. count me in if that supports your project.
```

---
## \#32 Posted by: abenny Posted at: 2017-06-06T18:37:14.173Z Reads: 706

```
when do you think youll be selling these??? i want one sooo bad
```

---
## \#33 Posted by: Print3r Posted at: 2017-06-06T18:50:27.369Z Reads: 714

```
Sorry, I missed that. That is very expensive for an NRF, pcb and oled especially as the case is 3d printed - I would expect the first 50 of an abs injection moulded remote to be this price as the moulds in that case are very expensive ... but for a 3d printed remote. I am going to wait on @Sander's remote (www.electric-skateboard.builders/t/oled-remotes-under-development-please-leave-suggestions/22055/179) - it should be half the price and also with a bluetooth module and accompanying app, a charging power-in calculator  (though the screen will be monochrome not colour).
```

---
## \#34 Posted by: Wajdi Posted at: 2017-06-06T19:34:33.930Z Reads: 692

```
Thanks for the suggestion guys, the price will be cheaper than 120$ and not 120$. Once I finalize the design, I will calculate the first batch cost. It will be cheaper than evolves remote + universal + packing a lot more features like the kill switch, custom button programming, failsafe function, full range of riding modes, frequency channel selection, detailed states...etc.
```

---
## \#35 Posted by: Sander Posted at: 2017-06-07T09:28:52.222Z Reads: 690

```
Very cool and compact pcb, I love it!

I have a few questions:
How did you manage to upload the bootloader on the ATmega32U4?, did you need to make the HWB pin high or low?

How far range do you get with the nrf and which antenna cap is it?

Thanks alot!
```

---
## \#36 Posted by: rpn314 Posted at: 2017-06-07T11:08:04.114Z Reads: 703

```
I do like the design a lot. I gotta be honest though, saying "less than $120" is a lot of sticker shock. That's the price of some of the cheaper (insert whatever we're calling VESCs now). Even considering small runs, I can't figure how you're arriving at that cost. I've built and sold a few of Vedder's nunchuckRF for a few people around and it has not cost me anywhere near that (less than half of that in fact, fully finished!), and frankly the only difference is that you've got a buzzer and a screen.
```

---
## \#37 Posted by: Sander Posted at: 2017-06-07T11:42:06.294Z Reads: 703

```
I know too, its crazy how expensive it is. But just for making one remote, with no bulk price with pcb ordering and components + color oled + reciever pcb it easily cost over 120 dollars.

Its expensive to make only one,
but if you are making around 20 the price jumps very steep!
Probably down to 30 USD.
```

---
## \#38 Posted by: Wajdi Posted at: 2017-06-07T19:23:10.740Z Reads: 716

```
Thanks, I'm not using an Atmega, I'm using Atmel's SAMD cortex m0, a 32bit micro controller. It is faster, and has much more memory, ideal for larger software needs. Perhaps thats why you assumed that the parts would be cheap :slight_smile: I'm also using the same processor on the receiver side to ensure perfect synchronization.
The receiver has the same computational power as the remote, it has available ports for SPI, ADC, UART, digital and analog pins and forwarded +5 and +3v3 power supply from the VESC. The goal is that it won't only act as a receiver, but also as a custom extra processing unit for those who want to write custom code to operate led's, add an extra display on the board, and operate extra devices all without changing the VESC's firmware and overloading it.
```

---
## \#39 Posted by: Print3r Posted at: 2017-06-07T19:29:40.069Z Reads: 705

```
Can you give a digikey link to the SAMD cortex m0 as I cannot find the page for it. All the other SAMD chips are also cheap though e.g. https://www.digikey.com/product-detail/en/microchip-technology/ATSAMD10D14A-SSUT/ATSAMD10D14A-SSUTCT-ND/5226482. I do like that you have opted for 32 bit though.
```

---
## \#40 Posted by: Sander Posted at: 2017-06-07T22:29:11.849Z Reads: 703

```
Cool! Which bootloader are you using?
```

---
## \#41 Posted by: lrdesigns Posted at: 2017-06-08T08:00:35.119Z Reads: 640

```
I don't get this complaining about the price. If its so cheap and easy to make why don't you make your own or buy from another vendor who has a cheaper one? @Wajdi is not a factory he's just one guy trying to make something cool for the community. Unless there is competing products the cost is what ever makes it worth his time otherwise you have no product at all. I don't want to bring all this negativity to this thread it just really bothers me that people expect innovative small run stuff at Chinese factory prices. I want cheap and cool stuff too but you cant always tick all the boxes. :thinking: :nerd:
```

---
## \#42 Posted by: DeathCookies Posted at: 2017-06-08T08:05:21.562Z Reads: 613

```
Perfect conclusion! :ok_hand:
```

---
## \#43 Posted by: rpn314 Posted at: 2017-06-09T12:12:29.177Z Reads: 627

```
Because I think there's a way to get this at half the cost. And a few of us are working on things. @Sander, @Print3r and @lox897 for starters. I like what @Wajdi is doing, I'm frankly just trying to push him to do even better!
```

---
## \#44 Posted by: Print3r Posted at: 2017-06-09T12:30:45.267Z Reads: 631

```
I agree - there is a fine line between something being a necessary feature and just a price booster. The coloured screen just increases the price --> you are not going to watch videos on it because it is tiny and you should be focusing on riding + coloured screen means that you have to go with a 32 bit processor, which is more expensive than a 8bit (I would assume). Without the 32 bit processor the screen would have a super slow refresh rate and make the remote unusable. Apart from the high price, I think that this is an interesting project with a lot of excess power capability in the processor ... you could probably run some interesting video-overlay on the receiver processor and livestream to the phone over bluetooth with some work.

I think that it must be realised that this project will not be for everyone - the price, even if reduced by $20 is too high for most people (given that the case is not injection moulded, the screen is under your fingers and a joystick [very cheap] is used for input). The masses will probably go for @Sander's remote or use @lox897's version of Rolling Gecko's code as it is much cheaper to produce and the people developing it are not needing to make a living off selling theirs. @Sander's remote will also likely have some fun easter eggs in the code!
```

---
## \#45 Posted by: wiltz Posted at: 2017-06-10T11:37:32.497Z Reads: 578

```
I'm in. Looks like a great improvement over the Evolve GT remote.
```

---
## \#46 Posted by: Wajdi Posted at: 2017-06-19T17:42:05.317Z Reads: 599

```
Quick update guys, finished adding a safety button to act as a kill switch/cruise control. I also finished implementing distance traveled tracker and dynamic frequency selection for crowded areas.
The receiver now has an SMA antenna as many of you have requested it, this gives a theoretical range of around 1000 meters without obscuration. 
I will record a demonstration video once everything is assembled, it should be ready this week. :+1:
```

---
## \#47 Posted by: sprocket12 Posted at: 2017-06-19T19:12:02.601Z Reads: 612

```
I'm in.  Quality is what I'm most interested in.  If the 'extra' costs gives me safe, fast response, and a quality product that lasts, I won't have a problem spending more coin.
```

---
## \#48 Posted by: Silverline Posted at: 2017-06-21T14:34:52.757Z Reads: 624

```
If you`r sending to Europe.... I´m in.... totally cool project. Looking forward to some video :-)
```

---
## \#49 Posted by: Wajdi Posted at: 2017-06-27T20:19:25.116Z Reads: 687

```
Quick update: Major improvements in design, now using a 1.44" color display instead of the small 0.95". The result looks much better! More room for detailed data display as well as better user interface. 
Also the remote PCB has been updated and finalized to accommodate the new display.
Receiver PCB was finalized as well and its a simple plug and play to the VESC.
Still waiting on some components that should arrive any time now, and I will post a detailed video about the software.
If you haven't noticed already, my website where I will be selling this remote is http://eboardshop.net. You can sign up for the Newsletter to be notified about pre-order dates as well as the latest offers. 
[img]http://i.imgur.com/Zop9VrM.png[/img]
[img]http://i.imgur.com/Dpjba4S.png[/img]
[img]http://i.imgur.com/4DdBjoa.png[/img]
[img]http://i.imgur.com/J1jZvsO.png[/img]
[img]http://i.imgur.com/sS5doJ2.png[/img]
```

---
## \#50 Posted by: Decdog Posted at: 2017-06-28T02:55:26.488Z Reads: 611

```
Nice design! How much will you be selling them for?
```

---
## \#51 Posted by: Wajdi Posted at: 2017-06-28T18:10:28.940Z Reads: 600

```
Thanks, price is not set yet, I will post an update once I have everything calculated.
```

---
## \#52 Posted by: Silverline Posted at: 2017-06-28T18:21:50.808Z Reads: 601

```
Why did you chose the form factor like you did?
Is it okay , to throttle like that ? And isn't your hand blocking the screen ? I like this form factor https://m.aliexpress.com/s/item/32678995218.html?spm=a2g0n.orderList.0.0.T3wszd&#autostay to me it's more natural to have in hand and use
```

---
## \#53 Posted by: Wajdi Posted at: 2017-06-28T18:42:05.671Z Reads: 583

```
I felt that its the most comfortable to hold, inspired from the ps4 remote and wii nunchuck.
Also the screen is easily accessible even when riding.
```

---
## \#54 Posted by: abenny Posted at: 2017-06-28T18:52:29.235Z Reads: 563

```
bookmarked your site...im likely gonna order one once they come up for sale and play with it as soon as im home from school next summer :D
```

---
## \#55 Posted by: Jinra Posted at: 2017-06-28T18:53:27.197Z Reads: 539

```
I mentioned that as well. I much prefer a slimmer profile that easily fits in my pocket.
```

---
## \#56 Posted by: Silverline Posted at: 2017-06-28T20:16:08.489Z Reads: 542

```
I agree....

Would be cool, if we could choose between slim design and "fat nunchuck" design :slight_smile:
```

---
## \#57 Posted by: Hardwiring Posted at: 2017-06-28T20:38:33.835Z Reads: 524

```
Really looking forward to seeing how this goes down when there are units out there that are getting hands on testing, nice job btw
```

---
## \#58 Posted by: ThomasLefort Posted at: 2017-07-04T14:44:04.663Z Reads: 539

```
I've been working on a remote like yours, but I had lots of problems. Yours seems interesting. I signed up to your newsletter.
```

---
## \#59 Posted by: Wajdi Posted at: 2017-07-29T18:15:54.947Z Reads: 635

```
Hey guys, a little update of what I have been working one. During the past few weeks I have been focusing on testing and improving the software, I have also updated the receiver to incorporate an rp-sma antenna for a better range and reliability. A built in antenna is also available for those that prefer a low profile.
<img src="/uploads/db1493/original/3X/b/6/b68f2d68035725168ec312a8912ffd21d6eedce3.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/e/a/ea5f47f0e7180287973ac859841838fcadfd0de1.JPG" width="375" height="500">

The receiver has a lot of processing power due to its 32bit samd21 MCU. I have exposed SPI pins, 3v3, 5v, GND, and several GPIO pins. This will make it easy to add a display, control LED's, connect sensors, etc.
```

---
## \#60 Posted by: High-roller Posted at: 2017-07-29T20:59:27.443Z Reads: 630

```
This just gets better and better! 
I imagine that most folks will go for the low profile internal antenna, but having the option to switch is nice. The pins for adding more features is an incredible amount of flexibility!
```

---
## \#61 Posted by: Wajdi Posted at: 2017-08-03T23:06:33.118Z Reads: 651

```
Everything assembled together and prototype almost done!

<img src="/uploads/db1493/original/3X/f/4/f44fee5f291a2364e4e8c75b3a2f57a31535f346.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/c/b/cb75d7b822d10aff08726da86471a99b264558e9.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/0/e/0eb12adcc1ce6a73c4687b7052a6a4ffc64cab3e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/b/9bd4f5f4cf5db1949050864b57bec664b5737de3.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/f/5/f5da7b08b73387f1f381086728f1f4c304acb8df.JPG" width="375" height="500">
```

---
## \#62 Posted by: evoheyax Posted at: 2017-08-03T23:41:07.254Z Reads: 588

```
Please, TAKE MY MONEY!!!!!! *in a 5 year olds vioce*:  I want it!!!!!!!!!
```

---
## \#63 Posted by: NAF Posted at: 2017-08-04T03:30:45.920Z Reads: 584

```
Oh boy!! Sick!!! How much my friend? :slight_smile:
```

---
## \#64 Posted by: High-roller Posted at: 2017-08-04T10:39:47.820Z Reads: 579

```
Any chance of an early adopter's (read: beta) discount? 😉
```

---
## \#65 Posted by: Decdog Posted at: 2017-08-04T14:49:39.964Z Reads: 563

```
I NEED ONE.
10 chars
```

---
## \#66 Posted by: banjaxxed Posted at: 2017-08-04T15:38:42.928Z Reads: 558

```
I need another remote like I need trepanning, better get the drill ready
```

---
## \#67 Posted by: solidgeek Posted at: 2017-08-04T20:53:44.311Z Reads: 558

```
Well done!! I love your display and the interface you have made, looks very cool :smile: I am making my own remote based on an Arduino and a Hall Effect sensor, with a small OLED screen (128×32px). I would like your opinion on it some time!

I am curious to know if you have encountered any problems with the trigger button? Are you using a standard tacktile button or some other solution? All tacktile buttons I have tested seems to have a "deadzone" after it clicks where it doesnt conducts. Any thoughts on this?
```

---
## \#68 Posted by: Wajdi Posted at: 2017-08-04T23:54:28.878Z Reads: 550

```
Thank you guys for the positive feedback!
 @solidgeek Thank you! I saw your project and it looks awesome, I love the orange/black combination :grinning: I might try that, I have some orange filament left from other projects. Regarding your tactile problem. it seems weird, I'm using regular push buttons and didn't have any issue, the only thing I can think of are pullups/pulldowns, perhaps your pin is floating causing inconsistent readings.
```

---
## \#69 Posted by: solidgeek Posted at: 2017-08-05T00:01:42.649Z Reads: 579

```
Thanks! Yeah, the orange definitely gives it some character :P !

A floating pin was also my first thought, however, I am using Arduinos INPUT_PULLUP, so that should not be the problem. Thanks for the advice! I have ordered a few new buttons to try, hopefully, they work ;-) 

Good luck with your remote, it is truly a masterpiece! :D
```

---
## \#70 Posted by: Wajdi Posted at: 2017-08-07T19:54:02.927Z Reads: 594

```
Bench testing my prototype build, check it out :wink:

https://www.youtube.com/watch?v=x0iw8KbLJnc
```

---
## \#71 Posted by: High-roller Posted at: 2017-08-07T21:28:29.865Z Reads: 594

```
<img src="/uploads/db1493/original/3X/5/c/5c8213a5e9c32df02e14a4a67e2b5d126812774a.png" width="221" height="228">
```

---
## \#72 Posted by: Ackmaniac Posted at: 2017-08-07T22:41:16.894Z Reads: 566

```
No offence, but it seems to have a slow response to throttle inputs.
```

---
## \#73 Posted by: evoheyax Posted at: 2017-08-07T22:42:13.181Z Reads: 567

```
@Ackmaniac Maybe the baud rate is too low?
```

---
## \#74 Posted by: lrdesigns Posted at: 2017-08-08T01:29:56.330Z Reads: 599

```
[quote="Wajdi, post:59, topic:24654"]
I have also updated the receiver to incorporate an rp-sma antenna for a better range and reliability.
[/quote]

Hey @Wajdi awesome stuff so far, really appreciate the addition of an add on antenna for the receiver but I wonder why you used rp-sma connector and not a IPEX1 or IPEX4 which is common on RC receivers? Its the same antenna as the one you showed but without the protective sheaf and a much smaller connector. 
<img src="/uploads/db1493/original/3X/3/5/35bf5338a619121fefdf7c76ac690eed9332b795.png" width="690" height="310">
<img src="/uploads/db1493/original/3X/3/7/3791eb778f899bf4bea679562fbd7786f56a7c27.png" width="338" height="273">

If the connector is too expensive or hard to get alternatively you can just directly solder, but not as easy for most people. This is whats on the GT2B receiver. 

<img src="/uploads/db1493/original/3X/d/d/dd353e24a32f8252d558b571b6312212f1f3fde4.png" width="690" height="381">

https://www.amazon.com/NIDICI-IPEX4-Feeder-Antenna-Receiver/dp/B01M2BR2ZD/ref=pd_sbs_21_4?_encoding=UTF8&pd_rd_i=B01M2BR2ZD&pd_rd_r=80C3C0JH6RPC5FAZG3M3&pd_rd_w=MmKlu&pd_rd_wg=Bfolt&psc=1&refRID=80C3C0JH6RPC5FAZG3M3
```

---
## \#75 Posted by: Wajdi Posted at: 2017-08-08T02:13:24.343Z Reads: 553

```
It was intentional, I have sensitivity set on Low. I will make another video showing the different sensitivity options. It can go as fast as a blink of an eye.
```

---
## \#76 Posted by: Wajdi Posted at: 2017-08-08T02:15:41.915Z Reads: 550

```
Nice alternative, I will add that to my To-Do list, seems like a much compact solution.:+1:
```

---
## \#77 Posted by: devilpiggy38 Posted at: 2017-08-08T07:45:41.050Z Reads: 584

```
Add on..

I suggest you try holding the remote wearing this kind of skateboard gloves with hard plastic pad particularly on the palm.  I personally wear them for safety and I guess for most of the guys here too. You have the the design and functions I want it so badly...but the ergonomic design for gloves wearer, how does it function? handle? Safe? comfortable to hold? 

I'm currently using the Nano remote. It is very small in size, but the position of the remote on hand while wearing the glove makes the remote position slightly uncomfortable. 

Thanks mate! 

<img src="/uploads/db1493/original/3X/3/6/36bf6008aab823adfae0097c1dc54f8e04c5dcf7.jpg" width="500" height="500">
```

---
## \#78 Posted by: devilpiggy38 Posted at: 2017-08-08T07:48:37.411Z Reads: 572

```
I flew off my board at the speed of 50++km/h. The glove safe my BOTH my hand.
```

---
## \#79 Posted by: devilpiggy38 Posted at: 2017-08-09T05:52:21.625Z Reads: 582

```
apologize if i drifted topic.. this the the best interfacing wireless remote if anyone here can research about.

https://youtu.be/oWu9TFJjHaM
```

---
## \#80 Posted by: notger Posted at: 2017-08-10T19:57:47.534Z Reads: 574

```
Whow, just came across that Thing, its wonderful.

any idea when you will officially "release/sell" them ?

I'm interested !!


ps.: on your website it tells that ill get a conformation mail but i do not, am i signed in now ?
```

---
## \#81 Posted by: notger Posted at: 2017-08-10T20:29:58.747Z Reads: 557

```
Hi,
will it be possible to add some kond of pot to the programmable custom button on the remote, in order to controll a hydraulic breaking Servo ?

Cause i have a Magura Brake from Trampa wich i controll with a RC-servo, and i'd like to keep that option.

greets
Gernot

[http://www.electric-skateboard.builders/t/mmmsb-magura-mad-munkey-servo-brake-yeah/30195](http://www.electric-skateboard.builders/t/mmmsb-magura-mad-munkey-servo-brake-yeah/30195)
```

---
## \#82 Posted by: Wajdi Posted at: 2017-08-10T21:00:30.631Z Reads: 534

```
That would be possible. You can use the main throttle pot for that. When the throttle pot is pulled downward, it will apply regenerative braking, at the same time, you can configure one of the GPIO pins on the receiver to read the pot values and use that to control your braking servo. Two birds one stone solution :slight_smile:
```

---
## \#83 Posted by: notger Posted at: 2017-08-10T21:20:26.842Z Reads: 527

```
From where are you actually ?
```

---
## \#84 Posted by: notger Posted at: 2017-08-15T16:40:50.794Z Reads: 531

```
So the receiver is using the UART port.

would it be possible to use your receiver on UART port of the master VESC
and a HM-10 bluetooth module for @Ackmaniac 's Android app on the slave VESC 
or teh other way round if used in Dual-VESC Setup ?

greets
Notger
```

---
## \#85 Posted by: rpn314 Posted at: 2017-08-16T15:26:16.260Z Reads: 526

```
[quote="notger, post:84, topic:24654, full:true"]
So the receiver is using the UART port.

would it be possible to use your receiver on UART port of the master VESC
and a HM-10 bluetooth module for @Ackmaniac 's Android app on the slave VESC 
or teh other way round if used in Dual-VESC Setup ?

greets
Notger
[/quote]

Yes. I have an NRF24L01 module on my master and a bluetooth module on my slave. works well :)
```

---
## \#86 Posted by: Wajdi Posted at: 2017-08-16T19:12:05.547Z Reads: 494

```
Im from USA, and yes as @rpn314 stated, it should work just fine.
```

---
## \#87 Posted by: notger Posted at: 2017-08-16T19:27:25.265Z Reads: 512

```
That's great,....any idea when you'll start selling them and for what price ?

Do you plan to make different enclosures in the future? 
like Thumb or index-finger trigger enclosure ?

greets

Notger
```

---
## \#88 Posted by: Der6FingerJo Posted at: 2017-08-16T20:19:12.385Z Reads: 506

```
Can you explain to me why Bluetooth wouldn't be suitable? I'm using hc05 modules for my remote and I'm not sure if I get the rare dropouts because of my code or because of the Bluetooth modules. Considering switching to nrf. 
Besides, I'm very impressed by your design and it,alongside others, inspired me to make my own crude Arduino nunchuck OLED remote because I wanted to learn how to do this stuff. Thanks!
```

---
## \#89 Posted by: Wajdi Posted at: 2017-08-16T22:34:12.953Z Reads: 490

```
Thanks. I believe that Bluetooth is more suitable to interface smartphone devices, if i'm not mistaken, it uses a proprietary communication protocol with a predefined baud rate. Not really ideal if you want to do something like frequency hopping and advanced channel selection. 
I'm glad my work inspired you and I hope to see your project soon :slight_smile:
```

---
## \#90 Posted by: Wajdi Posted at: 2017-08-16T22:46:20.355Z Reads: 488

```
Perhaps in the future, if the project takes off I will get motivated to spend more time on it.
About the selling price, I finished setting up the store, and I think I'm ready to start the first batch.
I believe I can get all the necessary parts ready+assembly in about 2-3 weeks, hence I'm starting a Pre-Order batch. For the first batch, remote price should be 109$ + 19$ for receiver.
I think 109$ for the remote is a fair price seeing the amount of effort I have put into it, its still cheaper than evolves 120$ remote.
Pre-Ordering should open later today or first thing in the morning :relaxed::+1:
```

---
## \#91 Posted by: notger Posted at: 2017-08-16T22:49:00.032Z Reads: 463

```
preordering,...here in the forum, or via your website ?
```

---
## \#92 Posted by: dg798 Posted at: 2017-08-16T22:49:04.174Z Reads: 467

```
that is very cool.
great job!
```

---
## \#93 Posted by: jmasta Posted at: 2017-08-17T02:22:56.908Z Reads: 468

```
Looks great @Wajdi

There is definitely a market for an advanced remote like this

Like others have mentioned, I'd love to see a trigger version down the road!  Keep up the good work
```

---
## \#94 Posted by: SeanHacker Posted at: 2017-08-17T02:58:00.086Z Reads: 468

```
Take money now please. Thanks!!!!
```

---
## \#95 Posted by: Der6FingerJo Posted at: 2017-08-17T07:11:08.185Z Reads: 473

```
Alright, I thought Bluetooth would handle all the connection stuff like hopping itself and I just had to send some serial commands to it. You can see some pictures of the remote in my build thread, however it's not nearly as complex as yours. I don't have much real world experience with programming yet so I wanted to keep it simple.
```

---
## \#96 Posted by: notger Posted at: 2017-08-17T07:26:34.825Z Reads: 465

```
How easy, or will it be possible to update the "Firmware" if you would ever change teh interface design.
is it just USB Plug and Play or would you need some kind of Link to do that ?

(sorry I'm not a microcontroller person)
```

---
## \#97 Posted by: lrdesigns Posted at: 2017-08-17T07:50:46.106Z Reads: 453

```
[quote="Der6FingerJo, post:88, topic:24654"]
Can you explain to me why Bluetooth wouldn't be suitable?
[/quote]

2.4ghz is just more reliable. Bluetooth has a much shorter range than 2.4ghz and usually transmits at a lower power level. If you go into a city that has high density RF noise, bluetooth can easily be drowned out. And if your talking about RC 2.4ghz they have extra technology like frequency hopping to prevent interference when there are many other users on the same band.
```

---
## \#98 Posted by: NAF Posted at: 2017-08-17T08:18:14.737Z Reads: 441

```
2.4ghz is super reliable on my mini remote. It never failed me, not like the bluetooth connection which suck pretty bad when riding in the city.
```

---
## \#99 Posted by: notger Posted at: 2017-08-17T09:51:39.531Z Reads: 478

```
Hi,

could you post some Photos of the Final "release-version" please.
Also Photos from inside would be interesting. (Might make my indexfinger-mod by myself with an Madmunkey-enclosure if it fits)
Id like to know how the receiver PCB looks at the end including antenna.

And please post the measurements of the reiceiver PCB incl. overall height. wanna have a look if it fits into my VESC Enclosure.

greets
Notger
```

---
## \#100 Posted by: notger Posted at: 2017-08-17T09:56:23.359Z Reads: 487

```
[quote="Wajdi, post:82, topic:24654"]
That would be possible. You can use the main throttle pot for that. When the throttle pot is pulled downward, it will apply regenerative braking, at the same time, you can configure one of the GPIO pins on the receiver to read the pot values and use that to control your braking servo. Two birds one stone solution :slight_smile:
[/quote]

Sounds good:
But can i add a pot instead of the "_Assign a function to the custom push button._"
cause i wanna controll the Brake Servo seperate from regenerative braking.
The reiceiver would also need to spit out "PPM-Servo Language" and the possiblity to supply up to 5A Servo current for the high-torque Servo ??
```

---
## \#101 Posted by: vjsharpeyes Posted at: 2017-08-17T10:15:24.842Z Reads: 422

```
I am jelly of your skills. I wanna see a finished product, but I'll probably take one.
```

---
## \#102 Posted by: Der6FingerJo Posted at: 2017-08-17T10:40:05.952Z Reads: 434

```
Afaik Bluetooth too operates on 2.4. 
I thought using a pre-established protocol would be idiot proof and some time ago i got up to 80m Bluetooth connection from my quadcopter to my phone. 
Well I guess I will switch to nrf sometime.
```

---
## \#103 Posted by: Wajdi Posted at: 2017-08-20T01:47:15.755Z Reads: 439

```
Pre-ordering will open on my website http://www.eboardshop.net
I never did something like this, so here is my current plan, you guys tell me what you think:
First I will open Pre-Ordering, then wait about a week or less to get as many people on the first batch as possible. Next I will order everything from manufacturers, final assembly+testing should be done in about 2 weeks. So the overall process will take about 3 weeks. People that miss the first batch will be included in the next batch, and so on.
```

---
## \#104 Posted by: Wajdi Posted at: 2017-08-20T01:49:49.103Z Reads: 451

```
[quote="notger, post:96, topic:24654"]
How easy, or will it be possible to update the "Firmware" if you would ever change teh interface design.
is it just USB Plug and Play or would you need some kind of Link to do that ?
[/quote]


The remote has a micro usb port that is linked to the serial pins, so yeah, you can just plug the remote to your computer, and use arduino IDE to upload your sketch. I might open source my software sometime in the future if I finish cleaning it up.
The receiver tho, does not have a usb serial port, so you need an SWD programmer to upload a new firmware.
```

---
## \#105 Posted by: NAF Posted at: 2017-08-20T06:18:04.754Z Reads: 423

```
@wajdi can you post a video with all the menus and it's functionality ?
```

---
## \#106 Posted by: High-roller Posted at: 2017-08-20T06:40:44.533Z Reads: 430

```
Woah, out of stock already! Well, guess I'll wait for the next round...
```

---
## \#107 Posted by: Wajdi Posted at: 2017-08-20T15:54:22.487Z Reads: 464

```
[quote="NAF, post:105, topic:24654, full:true"]
@wajdi can you post a video with all the menus and it's functionality ?
[/quote]


Working on one right now.

[quote="High-roller, post:106, topic:24654, full:true"]
Woah, out of stock already! Well, guess I'll wait for the next round...
[/quote]
Its marked as out of stock because I didn't start the Pre-Order yet.:slight_smile:
```

---
## \#108 Posted by: SkaterBoy58 Posted at: 2017-08-22T04:34:46.101Z Reads: 481

```
Any idea when Pre-Orders will be open?  
Cheers
```

---
## \#109 Posted by: Wajdi Posted at: 2017-08-23T22:01:21.149Z Reads: 503

```
Hey guys, here is a quick video I made to show the different remote settings, I might add a thing or two before release, but this should give you a good idea of how things work. The remote enclosure was quickly 3d printed on low settings for fast prototyping. I'm also in the process of ordering a new 3D printer, probably the cr-10, because it has a larger volume, and far more superior quality than mine.
https://www.youtube.com/watch?v=NHkWKNrXExc
EDIT: I have also modified the PCB to add the tactile push buttons directly to it, less wiring, and better connectivity. I also improved the LIPO charging, at first it was charging with 100ma, now it does 500ma.
```

---
## \#110 Posted by: nw-esk8 Posted at: 2017-08-24T04:24:07.404Z Reads: 481

```
when will you please take my money? :confounded:

EDIT: registered for newsletter @ eboardshop... but my question still stands :)
```

---
## \#111 Posted by: Wajdi Posted at: 2017-08-26T16:57:05.799Z Reads: 452

```
Hey guys, Pre-Ordering is now finally available! Buy your reservation at http://www.eboardshop.net and get in the first batch :relaxed:
```

---
## \#112 Posted by: nw-esk8 Posted at: 2017-08-26T17:13:04.245Z Reads: 457

```
I went to place my pre-order, but it looks like the checkout wizard is charging state tax regardless of which state/location you specify, which isn't legal.  If you can fix that, I'll complete the checkout.  I'm assuming you don't have a physical presence in all 50 states :).

Also, you still thinking they should be available in about 3 weeks?  Thanks.
```

---
## \#113 Posted by: Wajdi Posted at: 2017-08-26T17:36:32.927Z Reads: 435

```
Thanks for the heads up, I think I fixed that. I have a limited knowledge when it comes to things like taxes.
```

---
## \#114 Posted by: nw-esk8 Posted at: 2017-08-26T17:51:42.810Z Reads: 444

```
Thanks-that appears to be resolved... but sorry, I have another detail I wanted to address on the next step...

Your ToC says "Returns are accepted within 30 days of the **original purchase date**. All returns must be in **unused state**, in it’s original packaging with the original packing slip."

Can that be changed to "date of delivery" and "the original state"?  Otherwise, if I buy today and the pre-order takes a week or two longer than expected and/or if I am shipped a broken or damaged device, I'm not covered/protected on the return (not that I'm planning on having to, but wanted to address). Thoughts?  Thanks.
```

---
## \#115 Posted by: Wajdi Posted at: 2017-08-26T18:12:47.249Z Reads: 416

```
Fixed, thanks for pointing that out. :+1:
```

---
## \#116 Posted by: nw-esk8 Posted at: 2017-08-26T18:20:03.829Z Reads: 417

```
Thanks for the super quick turnaround(s)... pre-order placed!
```

---
## \#117 Posted by: banjaxxed Posted at: 2017-08-26T19:50:43.980Z Reads: 438

```
Interested but $40 is kind of high for shipping but I guess that's what's on offer to ireland, is this a discount on a future price?
 With import fees this could be almost be a $200 controller.

What's the deal with spares in case if an accident or wear?

Ps: very cool congrats
```

---
## \#118 Posted by: Wajdi Posted at: 2017-08-26T21:31:34.649Z Reads: 432

```
Thank you, and yes international shipping is kinda expensive :frowning2:
About spare parts, I think I will add things like 3D printed shells etc.. to be purchased separately.
```

---
## \#119 Posted by: JLabs Posted at: 2017-08-27T01:34:16.232Z Reads: 432

```
For the remote, you can ship it in a 6x10 bubble mailer for about $10 to Ireland as I just shipped parts to @banjaxxed

It’s also a similar price to all of Europe
```

---
## \#120 Posted by: Wajdi Posted at: 2017-08-29T17:22:55.210Z Reads: 433

```
Hey guys, if you are interested and want to be included in the first batch, you can Pre-Order at www.eboardshop.net, only a few days left until I submit parts orders.:+1:
```

---
## \#121 Posted by: notger Posted at: 2017-08-29T18:20:53.511Z Reads: 421

```
Hi,
I really love your remote, but i have a similar issue like @banjaxxed.
 40$ shipping plu toll an tax in Europe is getting near 200$ then, thats not in my budget right now.
Still i understand the effort you put in and the price you demand.

i might wait until the remote has proofen stability and saved up some money.
maybe you could also find some cheaper shipping option for us europeans.
I recently paied 35$ for a 5kg ebike-kit from US, so there must be an cheaper option.

greets
Notger
```

---
## \#122 Posted by: Mickyboy Posted at: 2017-09-01T00:16:08.220Z Reads: 392

```
Is the final product 3D printed or not?
```

---
## \#123 Posted by: Wajdi Posted at: 2017-09-01T00:45:58.092Z Reads: 390

```
Yes it's 3D printed
```

---
## \#124 Posted by: Mickyboy Posted at: 2017-09-01T01:05:43.837Z Reads: 392

```
So the final finish will look more like the remote in the video than the pics at the top of the thread?
```

---
## \#125 Posted by: scepterr Posted at: 2017-09-01T01:19:05.536Z Reads: 380

```
@Wajdi have you considered a disassembled, print your own case option?
```

---
## \#126 Posted by: Wajdi Posted at: 2017-09-01T01:48:24.015Z Reads: 384

```
@Mickyboy What pictures are you referring to?
@scepterr I might offer that option as well if enough people are interested.
```

---
## \#127 Posted by: scepterr Posted at: 2017-09-01T01:49:10.866Z Reads: 388

```
I'm definitely interested, what do you think the price would be?
```

---
## \#128 Posted by: Wajdi Posted at: 2017-09-01T02:12:58.211Z Reads: 385

```
It would save about 10$ off the original price.
```

---
## \#129 Posted by: scepterr Posted at: 2017-09-01T02:19:16.504Z Reads: 412

```
At $99 I would do it, at $10 off might as well get it assembled with the case even if just to have the case to spare if you print your own

Also would it technically be possible to make an auxillary display communicating with the same transciever showing some limited stats that would be board mounted. Configuration would be done from the remote
```

---
## \#130 Posted by: Mickyboy Posted at: 2017-09-01T02:51:37.230Z Reads: 432

```
These photos. If the end product looks as polished as that then I'm all in. 
<img src="/uploads/db1493/original/3X/b/3/b3606788b8cc6a1dbd0cf18b8754d8953601b295.PNG" width="690" height="264">
```

---
## \#131 Posted by: vjsharpeyes Posted at: 2017-09-01T05:15:45.663Z Reads: 428

```
I too would like to see a closer look at the finish of the plastic housing.
```

---
## \#132 Posted by: notger Posted at: 2017-09-01T06:32:05.831Z Reads: 438

```
[quote="Wajdi, post:126, topic:24654"]
@scepterr I might offer that option as well if enough people are interested.

[/quote][quote="scepterr, post:129, topic:24654"]
At $99 I would do it
[/quote]

I'm interested too in that option, the cheaper the Prive the less Toll we Europeans have to pay.

Notger
```

---
## \#133 Posted by: Wajdi Posted at: 2017-09-06T18:57:21.866Z Reads: 467

```
<img src="/uploads/db1493/original/3X/8/0/80c073185dd1ff3abb7c6ca51622955da071fa57.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/a/a/aa592f10eb187ec638409bb078a931e7ba410abb.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/e/6e22114ffb4f70d2ed639c2b7581e0a712eb978c.JPG" width="375" height="500">

PCBs are in! So fresh and shiny. Time to start the final assembly.
```

---
## \#134 Posted by: Mickyboy Posted at: 2017-09-06T21:02:26.176Z Reads: 411

```
I have my finger hovering above the "buy" button! Just waiting to see how the final product actually looks and performs.
```

---
## \#135 Posted by: Wajdi Posted at: 2017-09-06T21:15:02.535Z Reads: 416

```
I ordered a new 3D printer, it should arrive sometime this week. Enclosure quality will improve significantly! I can't wait to try it out.
```

---
## \#136 Posted by: Mickyboy Posted at: 2017-09-08T11:30:31.945Z Reads: 408

```
I hear that 3D printer settings can make a big difference too. Here's hoping it looks like a premium product.
```

---
## \#137 Posted by: notger Posted at: 2017-09-08T16:46:35.458Z Reads: 419

```
Hmm, still loving that remote.

again my suggestion for us Europeans:
This is a DIY-community, so most here are DIY people.
please offer a DIY Kit.
with all needed parts but enclosure for self printing.
that should also lower the shipping cost, might fit in a envolope actually

greets
Notger
```

---
## \#138 Posted by: Wajdi Posted at: 2017-09-08T18:41:00.722Z Reads: 411

```
@notger I decided to start selling parts as a DIY kit, since many are interested. That way people will have the freedom to do whatever they like, it will also decrease the overall price. I will update the shop sometime this weekend or next week to add the new options.👍 
@Mickyboy Yes definitely! I have been experimenting with the printer settings for a long time until I found the perfect values. I probably wasted around 30 remote prints, no joke 😂
```

---
## \#139 Posted by: Mickyboy Posted at: 2017-09-08T21:18:48.185Z Reads: 403

```
Thanks for all your effort and time! Can't wait to see the final product!  If this turns out to be a winner, I will certainly spread the word!
```

---
## \#140 Posted by: navgor Posted at: 2017-09-10T21:31:25.271Z Reads: 411

```
I've got a Formlabs Form2 printer which produces aesthetically perfect prints, would love to give the casing a go on that. Could even do a small run for the community using the 'Tough' resin which matches ABS strength.
```

---
## \#141 Posted by: Mickyboy Posted at: 2017-09-11T03:46:24.552Z Reads: 384

```
Now you're talking!
```

---
## \#142 Posted by: nw-esk8 Posted at: 2017-09-23T03:03:06.675Z Reads: 398

```
How's the new printer?  Did you end up going w/ the CR-10?
```

---
## \#143 Posted by: Wajdi Posted at: 2017-09-23T05:30:18.793Z Reads: 420

```
The new printer is miles better than my old one, I will post some pictures tomorrow morning of the quality. I ended up getting the Anycubic I3 mega, very sturdy and excellent print so far. I was also working on implementing an LED control system on the remote and receiver software, because I know that once shipped, it would be hard to update the firmware, especially on the receiver, since it doesn't have a USB port. The lightning settings will allow to set RGB values from the remote, and apply it on the receiver. I also added several lightning animations like rainbow, marquee, etc for people that want to use LED stripes.
```

---
## \#144 Posted by: Wajdi Posted at: 2017-09-24T05:14:40.696Z Reads: 457

```
<img src="/uploads/db1493/original/3X/d/b/dbae0bdef87729fb3c03c9bfcc92bfecf5e28ac4.jpeg" width="375" height="500">
<img src="/uploads/db1493/original/3X/2/c/2c4dd40540a23092a3ab175f8214c0af62eb34fb.jpeg" width="375" height="500">
I also received connection cables, flat ones!
<img src="/uploads/db1493/original/3X/1/1/117e9ad81c17e0b53f2db8f7b166f098176875d2.jpeg" width="375" height="500">
```

---
## \#145 Posted by: banjaxxed Posted at: 2017-09-24T13:09:47.700Z Reads: 418

```
Interested in kit option what is it looking like price wise now?
```

---
## \#146 Posted by: rolexbene Posted at: 2017-09-24T18:50:22.541Z Reads: 414

```
Yes I too would be interested in the kit option, as I have my own printer.
```

---
## \#147 Posted by: High-roller Posted at: 2017-09-24T20:41:02.297Z Reads: 411

```
Same here!
```

---
## \#148 Posted by: Wajdi Posted at: 2017-09-24T20:48:18.529Z Reads: 412

```
Hey guys, I will be selling it as a kit.
If I understand correctly, you want everything dissembled for you to assemble the way you want? Or do you want connections pre-soldered?
```

---
## \#149 Posted by: SkaterBoy58 Posted at: 2017-09-25T02:58:49.207Z Reads: 398

```
Any idea when the first batch of pre-orders will be shipping
Thanks
```

---
## \#150 Posted by: High-roller Posted at: 2017-09-25T04:33:30.084Z Reads: 390

```
Personally I would prefer pre-soldered. I also have a 3d printer, so I'm planning on printing my own case, maybe adapting it somewhat.
```

---
## \#151 Posted by: Wajdi Posted at: 2017-09-25T04:57:43.767Z Reads: 410

```
I was extensively working on improving the software especially wifi range and speed, and I'm glad I didn't send out the remotes because I just increased its range by 10x, and the transmission speed is now probably 400% times faster! I have also added a menu option to set RGB values to control LED strips and such.
Better delay it by a couple of days and get an awesome remote than rush it and have problems later. I should wrap everything up by this week, I will keep you guys updated and thank you for waiting :+1:
```

---
## \#152 Posted by: SkaterBoy58 Posted at: 2017-09-26T22:52:10.494Z Reads: 407

```
Great - So will your spi allow for headlight , horn and the RGB LED lightshow?

Will the RGB LED require 5V separate power supply ?
Cheers
```

---
## \#153 Posted by: Wajdi Posted at: 2017-09-27T01:44:37.096Z Reads: 412

```
The receiver will have a digital pin to control LEDs for example, but they would still need a power source. The receiver will be able to control things, but does not provide power, it just forwards the 3.3v and 5V from the VESC. I don't know whats the max rating of the VESC power regulator, but I doubt it would be enough for a large number of LEDs.
Same thing applies to a horn and headlights.
I have plans to make a power control circuit as an add-on, it will be able to handle several amps of power, and can be easily used to power LEDs and such while controlling them from the remote.
```

---
## \#154 Posted by: SkaterBoy58 Posted at: 2017-09-27T03:55:56.323Z Reads: 395

```
Great - Thanks for this . I will design up a three mosfet switch circuit for LEDS with separate  5V power supply.

In addition to the three LEDs digital pins - how many separate binary pins are there for lights , horn , bell etc that can be activated from remote?

Cheers
```

---
## \#155 Posted by: High-roller Posted at: 2017-09-27T04:02:29.644Z Reads: 385

```
I bought some LED headlights that take 12 volts, so I'm using a dc step-down converter.
Would your power supply be able to go above 5 volts?
```

---
## \#156 Posted by: Wajdi Posted at: 2017-09-27T04:08:59.101Z Reads: 394

```
Receiver pinout is as follow: MISO, SCK, MOSI, D5, A0, A1, A2, 3V3 and GND
So basically D5, A0, A1 and A2 can all act as digital pins. If your three LEDs turn On and Off together, you just use one digital pin to control it, leaving you with 3.
```

---
## \#157 Posted by: SkaterBoy58 Posted at: 2017-09-27T04:14:12.298Z Reads: 392

```
Thanks for that - so will use D5 for horn and A0 A1 A2 for RGB leds.
 Looking forward to seeing what your light show animations  looks like.
```

---
## \#158 Posted by: Wajdi Posted at: 2017-09-27T04:37:18.685Z Reads: 398

```
Oh I see now what you meant by 3 pins for the LED's, one for each color line R, G, and B. :smile:
What I was working on is support for individually addressable LEDs, they require only 1 pin to change colors etc. However now that you have mentioned it, I will add support for regular LED strips as well, and you can choose your LED type from the remote. If its a individually addressable, then you just connect one control pin, if it's standard, you connect A0, A1, and A2 to the RGB pins.
```

---
## \#159 Posted by: Mickyboy Posted at: 2017-09-27T05:10:15.782Z Reads: 407

```
Forgive my ignorance, but how easy will this be to connect to my stock standard Raptor 2? Do I need to replace the receiver or will it work without any mods?
```

---
## \#160 Posted by: Wajdi Posted at: 2017-09-27T05:55:50.578Z Reads: 428

```
Theoretically you would just need to replace the receiver. I don't own a Raptor 2, but since it uses a VESC, it should be as easy as plugging the receiver on the UART port.
```

---
## \#161 Posted by: Wajdi Posted at: 2017-10-02T01:55:20.966Z Reads: 425

```
LED control demonstration! Let me guys know what you think. LED's are RGB, and you can change the color from the remote, I just didn't show the colors changing because I only had one Mosfet laying around :grinning:
https://youtu.be/Xg4cYkT1vF0
```

---
## \#162 Posted by: SkaterBoy58 Posted at: 2017-10-02T09:13:32.345Z Reads: 415

```
Looks great -so menu can set up either RGB with individual outputs or addressable through one output?
When do you expect to ship first batch as I have a build awaiting your remote to complete!
Cheers
```

---
## \#164 Posted by: banjaxxed Posted at: 2017-10-02T17:03:49.354Z Reads: 406

```
Take my money (just less than previously offered)
```

---
## \#165 Posted by: Wajdi Posted at: 2017-10-04T06:33:23.949Z Reads: 410

```
I finally managed to implement FHSS (Frequency-hopping spread spectrum)!
I have spent so many hours trying to develop a working solution, it is very time sensitive since both the receiver and transmitter have to be in synchronized agreement on what channel to hop next.
This allows the remote and the receiver to constantly switch frequencies in order to counter any interference, and thus creating a more reliable connection. 
Work is almost finished, and I should be able to start shipping by the end of this week :+1: 
Let's hope everything goes well :grin:
```

---
## \#166 Posted by: Kaly Posted at: 2017-10-04T22:55:14.732Z Reads: 391

```
Take your time :-)
```

---
## \#167 Posted by: SkaterBoy58 Posted at: 2017-10-06T06:49:14.429Z Reads: 397

```
Wajdi -

 Could the digital output drive a WS2811 IC for addressable LED strip?

Cheers
```

---
## \#168 Posted by: notger Posted at: 2017-10-06T08:29:18.716Z Reads: 419

```
Hi,

one more suggestion for cahnges or implementation for @Wajdi  (maybe also just later for a V.2 Version)

You receiver communicates via UART, right.
so, an amazing possibility would be to change "power-modes" with the remote.
maybe three different ones like (kids(300Watt) - adults(1000Watt) - maniacs(2000Watt))

@Ackmaniac s App and firmware allows to change powermodes via smartphone-app->bluetooth-module->UART 

so i guess this information could also be forwared by your remote an receiver ?

http://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888
```

---
## \#169 Posted by: Wajdi Posted at: 2017-10-06T22:11:44.965Z Reads: 386

```
@SkaterBoy58  Yes, it can drive both WS2812 and WS2811.
@notger Interesting, for Watt control I think the VESC needs to have @Achmaniac custom firmware uploaded. In my remote I  focus on stock VESC firmware. I don't know if there is a difference in the UART protocol between the stock version and @Ackmaniac one.
```

---
## \#170 Posted by: b264 Posted at: 2017-10-06T22:19:12.245Z Reads: 377

```
Please print it out of blue or pink plastic so it doesn't get mistaken for a gun in the hand by a trigger-happy cop
```

---
## \#171 Posted by: notger Posted at: 2017-10-07T07:01:27.879Z Reads: 387

```
with @Ackmaniac s Firmware its not just Watt-Controll witch ich really amazing compared to the old firmware or even the new VESC-Tool firmware.
It also allows  brake and reverse with ppm signals or cruise control via the second receiver cannel and lots of other nice stuff  !!!oh i should not forget throttle curve for braking and acceleration !!!!!!!!

would be amazing if you could couple up an make something compatible.

How is it actually looking with your DIY-kit ?
```

---
## \#172 Posted by: banjaxxed Posted at: 2017-10-07T08:02:49.524Z Reads: 365

```
Is there any sealing on the buttons/thumb stick? Would be great if it could take a little rain without imploding

Maybe sugru
```

---
## \#173 Posted by: Wajdi Posted at: 2017-10-07T22:15:07.811Z Reads: 381

```
@b264 Haha, sure. I was actually going to try different print colors :smiley:
@notger Nice! I will try to use his firmware on my VESC sometime this week, and see how it goes. About my DIY kit, i will launch it once I ship the first batch, I'm almost done, I just want to make sure everything is working as expected before shipping.
@banjaxxed Unfortunately no, the remote is not water resistant. Perhaps in future versions.
```

---
## \#174 Posted by: b264 Posted at: 2017-10-07T22:51:37.421Z Reads: 382

```
Not looking like we have a gun in our hand at night is important :stuck_out_tongue: Cops around here are a little jittery
```

---
## \#175 Posted by: banjaxxed Posted at: 2017-10-08T06:38:09.413Z Reads: 389

```
Cool I think sugru and corrosionx can help in the interim
```

---
## \#176 Posted by: Wajdi Posted at: 2017-10-12T22:23:53.574Z Reads: 425

```
I tried an orange color filament for the top cover and it looks awesome! Thanks @solidgeek for the idea :grin:

The seam in the middle is because I run out of filament mid-print. 
<img src="/uploads/db1493/original/3X/5/6/569b8fc9dde6ac7140cf018c79bb9beba7cf7855.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/c/e/ce007495d106f1acc09965fd268f5b4b10002ea5.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/2/a2685a0e3286c839d027aa74f2a412bef6e53eb6.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/7/9/791ffbf9760d7e405f6cdbdaa9c7b2f9506fa5b3.JPG" width="375" height="500">
```

---
## \#177 Posted by: Wajdi Posted at: 2017-10-13T03:47:04.569Z Reads: 429

```
A couple color options, whats your favorite? They all look darn good :grinning:

<img src="/uploads/db1493/original/3X/1/9/19372c1bff626e2fb12acdf5676d10aec0e001cc.jpg" width="690" height="491">
<img src="/uploads/db1493/original/3X/1/b/1b9f6c970ee5ccdcc5b81e2d187bcb8f9cc6360b.jpg" width="690" height="498">
<img src="/uploads/db1493/original/3X/c/a/ca480652651c2993294823dbd8de5bbf80b1b430.jpg" width="690" height="493">
<img src="/uploads/db1493/original/3X/b/8/b87f2712bd401b4c090aefd7cedeb94120b4b74c.jpg" width="690" height="495">
```

---
## \#178 Posted by: SkaterBoy58 Posted at: 2017-10-13T03:55:11.409Z Reads: 404

```
For me - White/Grey  one looks best
```

---
## \#179 Posted by: Ricco Posted at: 2017-10-13T12:46:40.806Z Reads: 406

```
The red and the white look best to me. I cant pick one clear winner.
```

---
## \#180 Posted by: smurf Posted at: 2017-10-13T18:06:48.220Z Reads: 400

```
I'll take one in blue!
```

---
## \#181 Posted by: Brianr058 Posted at: 2017-10-13T23:54:54.698Z Reads: 395

```
The only color your missing is green!
```

---
## \#182 Posted by: Genius2017 Posted at: 2017-10-15T22:04:26.168Z Reads: 373

```
@Wajdi I like the orange / black. For orders will you charge more for different colors? 

Also when will your code be available or is it not going to be available for people to modify / etc..? Great work..... Two thumbs up.
```

---
## \#183 Posted by: Wajdi Posted at: 2017-10-15T22:46:15.841Z Reads: 378

```
I only have black filament for now, I will start offering more colors during the next batch, and it will be free of charge.

I might release the source code in the future when I get some time to clean it up, right now it is not developer friendly at all :grinning:
```

---
## \#184 Posted by: SkaterBoy58 Posted at: 2017-10-16T03:44:10.313Z Reads: 376

```
Wajdi - Any idea on shipping dates ?

Cheers
```

---
## \#185 Posted by: High-roller Posted at: 2017-10-16T10:14:07.537Z Reads: 399

```
@Wajdi can I actually place an order yet or no? I'm still on the fence about whether to get a ready to use one or the kit.
```

---
## \#186 Posted by: Wajdi Posted at: 2017-10-16T21:01:41.822Z Reads: 419

```
@SkaterBoy58 Im waiting for micro USB cables to be delivered, I will include those with every order.
<img src="/uploads/db1493/original/3X/f/9/f9fb0f2d231e8a92081f7cee1d5df3936ca65d89.jpg" width="375" height="500">
Depending on how fast the remaining parts will get to me, I would say about a week.

Things I finished implementing:
* A reacting LED effect depending on throttle input, when throttle is half way LED will be half brightness, etc.., LED brightness will fade to current throttle percentage.
* Reacting LED effect depending on Temperature, LEDs color will fade to RED when PCB temperature rises, and BLUE when it's cool.
* Reacting LED effect depending on throttle state, BLUE when accelerating, and RED when braking. 
* Receiver will save and remember your settings.
* Added an option on the remote to limit throttle by percentage, useful for kids or someone that just started learning. Even if throttle is pushed all the way, it will only register value up to the specified percentage.  


@High-roller You can place an order as I'm about to wrap up the first batch. I will add a kit option in about a week or so.
```

---
## \#187 Posted by: High-roller Posted at: 2017-10-16T21:17:19.381Z Reads: 374

```
Great! Can you post the link to your order page?
```

---
## \#188 Posted by: b264 Posted at: 2017-10-16T21:19:06.665Z Reads: 384

```
What is the possibility of adding a bell?  Like the metroboard has, except with the piezo on the remote and not the board.  On a button pressed by index finger
```

---
## \#189 Posted by: Wajdi Posted at: 2017-10-16T21:36:46.858Z Reads: 384

```
@High-roller  http://www.eboardshop.net
@b264, There is a custom button on the remote, if you push on the joystick, it will set a digital pin on the receiver to control things like bells, etc. But if you want the actual piezo to be on the remote, it will require some work. The remote has a built in micro piezo but its not loud enough to act as a bell.
```

---
## \#190 Posted by: b264 Posted at: 2017-10-16T22:07:55.104Z Reads: 382

```
Is there any blank space or a void inside under where the index finger sits?
```

---
## \#191 Posted by: Wajdi Posted at: 2017-10-16T22:35:23.274Z Reads: 387

```
The index finger will normally sit on the cruise control/ kill switch button. Perhaps you can hack that button to dual task between cruise control and buzzer.
```

---
## \#192 Posted by: caustin Posted at: 2017-10-18T21:40:04.283Z Reads: 396

```
Just ordered, looks great!
```

---
## \#193 Posted by: Aborn Posted at: 2017-10-19T10:58:45.405Z Reads: 415

```
Will software updates be possible?

And do you mind explaining all the onscreen information?
```

---
## \#194 Posted by: Wajdi Posted at: 2017-10-20T06:24:07.590Z Reads: 415

```
<img src="/uploads/db1493/original/3X/e/8/e88a010768561fadfe5f8bd2c61fa8b67f10dc63.png" width="569" height="491">

Yes, software updates will be possible on the remote, however the receiver requires more involvement due to the lack of USB port.
```

---
## \#195 Posted by: notger Posted at: 2017-10-20T07:16:56.979Z Reads: 400

```
[quote="Wajdi, post:194, topic:24654"]
however the receiver requires more involvement due to the lack of USB port.
[/quote]


So i guess it need a programmer ? what kind ?
```

---
## \#196 Posted by: advongunten Posted at: 2017-10-20T09:38:56.889Z Reads: 386

```
-> Board Battery
Is it converted from the battery Voltage or Joule-measurement([mAh total - used]%)?
If a had a wish for free, i wish it would be the Joule-measurement.
Sure, that would need a settings entry for the total battery capacity.
But, in my opinion, its the best thing you can do - and this remote is one of the best ;-)!

-> VESC Temp
Does it displays two Temp if there are two vesc(via can-bus)?

-> Throttle Level
I would line up the throttle-lines (semi-circle) with the numbers (25,50,...).
Just a detail. Even without this, this is great and i'm lucky when i got mine in hands ^^!
```

---
## \#197 Posted by: Aborn Posted at: 2017-10-20T10:40:01.788Z Reads: 378

```
Great illustration!

The fuel guage looking half circle, is that the boards battery?
```

---
## \#198 Posted by: caustin Posted at: 2017-10-20T12:13:39.379Z Reads: 376

```
SWD programmer, STLinkv2 bootloader?
```

---
## \#199 Posted by: caustin Posted at: 2017-10-20T12:21:06.188Z Reads: 392

```
I would have to admit the @Ackmaniac FW functionality seems second to none, would be a shame if not able to integrate.  Things like the throttle curves for braking and acceleration and drive modes on the fly take your feature sets and expands dramatically.
```

---
## \#200 Posted by: Wajdi Posted at: 2017-10-20T18:16:05.276Z Reads: 415

```
@notger  Im using Segger J-link, JTAG SWD interface.
<img src="/uploads/db1493/original/3X/2/b/2bdf4e8ca2ae371b5f9f6dbca13793f220a8a8ec.jpg" width="666" height="500">

@advongunten For the Board battery, it currently calculates the percentage based on the battery voltage, however I like your suggestion, I think Joule measurement would be more stable because it doesn't rely on battery voltage. It would require an additional input value for the total AH but I think its worth it. Thanks.

About Vesc Temp, it should display the temperature of the master VESC if two are connected through CAN bus.

About that semi circle UI, I initially designed it to map the throttle value on the half circle, however after many testing, I found that it impacts the performance of the CPU and imposes a great delay on the main logic loop. So I disabled that temporarily until I find a better solution. The performance issue is coming from the display library, filling that half circle would require drawing and removing several lines, and that slows down the logic loop. I even pre mapped the values to memory to eliminate the mathematical calculations involved, but it's still not enough. I try to keep the logic loop as fast as possible with minimal delays to have a blinking fast transmission and response, and to keep FHSS synchronized with the receiver.
```

---
## \#201 Posted by: Wajdi Posted at: 2017-10-20T18:49:20.344Z Reads: 401

```
@caustin My remote should be compatible with his firmware, I will do a test today and let you know for sure. As long as the UART ptotocols are the same as the original firmware, it should work with no problems.
```

---
## \#202 Posted by: notger Posted at: 2017-10-20T19:54:22.111Z Reads: 394

```
[quote="Wajdi, post:201, topic:24654"]
As long as the UART ptotocols are the same as the original firmware
[/quote]

@Ackmaniac   are they the same ?

would be amazing if you both could "couple-up" and make some amazing hardware-firmware fusion.
```

---
## \#203 Posted by: Aborn Posted at: 2017-10-21T15:09:15.759Z Reads: 396

```
Keep in mind that lithium battteries dont discharge linearly voltage wise, you should calculate it from a discharge curve like this.
<img src="/uploads/db1493/original/3X/a/e/ae1a2da3706ba305d83910dbb74de4ac894c0b8c.gif" width="489" height="379">
```

---
## \#204 Posted by: ElskerShadow Posted at: 2017-10-21T16:46:09.960Z Reads: 371

```
Pre- ordered one. Amazing work. It’s expensive but happy to support and hope the development ends soon ! Cheers
```

---
## \#205 Posted by: Wajdi Posted at: 2017-10-21T20:45:32.143Z Reads: 361

```
I added support for PPM mode, now the remote can be used with any ESC that supports PPM. However with PPM there are no data, data is only available when using UART with a VESC.

I also think about only supporting Addressable LED strips, because they only require 1 data pin, and no additional hardware, they also have cooler effects. What do you guys think?
```

---
## \#206 Posted by: Wajdi Posted at: 2017-10-21T22:11:08.394Z Reads: 361

```
True, problem is discharge graph changes from battery model to other, and changes during the battery life cycle as well. Should we just adopt a median model?
```

---
## \#207 Posted by: nw-esk8 Posted at: 2017-10-21T22:24:26.763Z Reads: 364

```
Better than linear... or... maybe add an additional menu that let's you set the % levels (in increments of 10) to their corresponding voltage.

IE:
100% => 4.2
90% => 4.05
etc
```

---
## \#208 Posted by: b264 Posted at: 2017-10-21T22:24:29.402Z Reads: 355

```
[quote="Wajdi, post:200, topic:24654"]
Im[sic] using Segger J-link, JTAG SWD interface
[/quote]

Those don't run on Linux/Unix/BSD/Apple, right?  Only Windows?  :frowning:
```

---
## \#209 Posted by: Aborn Posted at: 2017-10-21T22:35:35.845Z Reads: 362

```
You should be able to find a universal one that might not be 100% accurate, but definitely better than a linear one

Maybe look at a cell like 25R since most people use those I think. But universal is possibly best. I'm not sure how different they are.
```

---
## \#210 Posted by: Wajdi Posted at: 2017-10-21T23:12:10.209Z Reads: 388

```
i think I will map the discharge following this graph 
http://www.ibt-power.com/bkencel/Graphs/LiIonDischGph.JPG
Seems to be a typical example.

About the battery percentage value, I think I will stick with the voltage based reading, because the Ah method won't really work since the consumed Ah value is being reset when the VESC is powered off. Even if we save the last session's consumed Ah locally on the remote, it will be hard to keep track of it when the board is plugged for charging. If anyone have suggestions please let me know. Thanks.

@b264 I used it on windows 7, I'm not sure there is a Linux/mac solution other than Virtual machines.
```

---
## \#211 Posted by: b264 Posted at: 2017-10-21T23:28:50.555Z Reads: 364

```
There isn't as far as I'm aware.  My friend uses the JTag and I thought that'd mention that.  He has to boot Windows inside a virtual machine on Linux Mint to use it
```

---
## \#212 Posted by: Aborn Posted at: 2017-10-21T23:33:52.503Z Reads: 356

```
Looks great :slight_smile:
```

---
## \#213 Posted by: Aborn Posted at: 2017-10-21T23:36:17.411Z Reads: 355

```
I don't know if it's possible but it would be cool to have a "total distance travelled" like on cars.
```

---
## \#214 Posted by: caustin Posted at: 2017-10-22T00:56:57.403Z Reads: 356

```
Haha, here’s a really bad idea, but maybe you can make it better. Make battery percentage value base user configurable and of person really wants Joule-based then they input pack size in Ah and if trip is paused the on restart (not knowing state again) it infers based on standing start voltage reading and V/Ah ratio. 😆
```

---
## \#215 Posted by: SkaterBoy58 Posted at: 2017-10-22T03:26:44.245Z Reads: 351

```
Only addressable leds is a good idea
Leaves other SPI for horn lights etc
Cheers
```

---
## \#216 Posted by: ElskerShadow Posted at: 2017-10-22T09:16:52.406Z Reads: 346

```
Yeah good idea. How much leds can handle the pin ?
```

---
## \#217 Posted by: advongunten Posted at: 2017-10-22T14:33:30.626Z Reads: 399

```
@caustin:
Thats a great idea. I almost always run the batteries down to zero on my drives, so joule-based would be great(for me).
On the otherside, i didn't think of, the remote doesn't get charge or discharge infos if its off. 
If you turn on the remote, its always in voltage-% would be a good compromis i think.

What about a battery-health indicator? 
Doesn't have to be on the drive-display but maybe in the settings.
New Batteries -> measurement of the internal resistance(say 5-10mOhm eq 100%) and save on remote.
After that you can compare the value to the initial one and with a choosen value, say 50mOhm eq 0% you can tell if we need to think of getting a new battery ^^. (diffVoltage/diffCurrent) should give us the internal resistance, if i'm right?
But the measurement has to be done if the battery is fully charged, otherwise the readings are incorrect!

And after that :blush:
we design our own BMS!
with memory for joule-base measurement, nextdrive-predictions for charge-cycle, means no-drive-insight-> automatically storage-charge, with resistance-heating or cooling depending of the ambient-temperatures while driving, 1 (or more) Amps balancing-current between each cell, cell-health monitoring, tesla-style charging-system:
2C-Charge-Current @ 4.1Volts, after that charge with 4.2Vmax to the end. Should be faster on 80% SOC this way.
Faster (save) Charge - faster back on the road :smiley: !

Hm, sorry for texting... had to let it out :slight_smile: 
Cu @ll
```

---
## \#218 Posted by: Wajdi Posted at: 2017-10-22T14:42:20.630Z Reads: 381

```
The pin is used for data, it can address as many Leds as you like, as long as you have enough power from your power supply. There is an option on the Light menu to set your Led strip pixel number.
```

---
## \#219 Posted by: Deckoz Posted at: 2017-10-26T15:24:50.500Z Reads: 402

```
@Wajdi

Looking to order. If I place today when should I receive the remote?
```

---
## \#220 Posted by: ElskerShadow Posted at: 2017-10-28T17:36:05.075Z Reads: 413

```
@Wajdi any updates on the remote ?
```

---
## \#221 Posted by: Wajdi Posted at: 2017-10-29T04:45:42.821Z Reads: 449

```
https://youtu.be/3syuywcEjos

Can you guys help me pick up a name for the remote?
```

---
## \#222 Posted by: Deckoz Posted at: 2017-10-29T14:43:08.146Z Reads: 436

```
SteezyRF

@Wajdi lol :)
```

---
## \#223 Posted by: Wajdi Posted at: 2017-10-30T05:28:36.680Z Reads: 426

```
Not bad :slight_smile: My current tempting name is Photon-X remote, what you think?
PS: I just added reverse option to the remote :grinning: its working great!
```

---
## \#224 Posted by: Aborn Posted at: 2017-10-30T06:31:55.157Z Reads: 420

```
Maybe just Photon, and then save the x for a future version =D. I think Photon sounds good :slight_smile:
```

---
## \#225 Posted by: notger Posted at: 2017-10-30T08:45:31.728Z Reads: 429

```
[quote="Wajdi, post:223, topic:24654"]
PS: I just added reverse option to the remote :grinning: its working great!
[/quote]

How does Reverse work ?
as example in ackmaniacs Firmware reverse works like a double-brake, the board just has to be under a certain and adjustable forward speed. otherwise your wheels will start spinning backward while you are actually going forward. (thats the case in the standard VESC Firmware)
```

---
## \#226 Posted by: NAF Posted at: 2017-10-30T09:16:10.405Z Reads: 401

```
@wajdi that's beautiful ! can you post which led strips did you use ?
```

---
## \#227 Posted by: Wajdi Posted at: 2017-10-30T14:33:31.527Z Reads: 397

```
@Aborn Sounds good!
@notger The trigger on the back of the remote is programmable through the menu, it can be a cruise control, safety switch, or reverse. In case of reverse, you push it once to change direction. If you happen to be already going at a certain speed while you pushed it, the board will start braking but your wheels won't start spinning backward.
@NAF Thanks! The receiver can drive any WS2812B RGB LED, just make sure its a WS2812B and runs at 5V. Also if the LED strip does not exceed 31 pixels, it can be powered from the receiver directly with no need of external power source.
```

---
## \#228 Posted by: longhairedboy Posted at: 2017-10-30T14:39:16.595Z Reads: 382

```
Thanks for building my new remote. I'm going to need a few of these.
```

---
## \#229 Posted by: caustin Posted at: 2017-10-30T14:52:06.657Z Reads: 384

```
Ultron lol
10 chars
```

---
## \#230 Posted by: mmaner Posted at: 2017-10-30T15:34:17.151Z Reads: 377

```
That is just...frak I don't know what to say.  Phenomenal.  I pre-ordered one.  When do you think they will ship?
```

---
## \#231 Posted by: caustin Posted at: 2017-10-30T16:02:37.963Z Reads: 366

```
Haha, hoping they are FIFO
```

---
## \#232 Posted by: notger Posted at: 2017-10-30T16:23:14.288Z Reads: 376

```
@Wajdi

So the DIY (print) Remote Kit (mostly interesting for Europeans) is sill postponed ?
are you still developing teh Remote Firmware or what is stopping you from selling them ?
and are you actually in contayt with @Ackmaniac about potential power.profile control, I mean that would make this Remote so amazing.

And another fancy addition concerning the LED feature would be to add an brake-light option so maybe that a separate red backlight or all the leds are turning red in case of braking ?
```

---
## \#233 Posted by: Dizzee Posted at: 2017-10-31T10:13:46.396Z Reads: 370

```
@Wajdi Is there anyway to make the remote work with several of your receivers as part of a Model Memory or E-Skate Memory? The remote looks great already but I'd be in for sure if I could buy one remote and a few receivers. As far as I know there is no other E-Skate remote with that feature. I bet you'd sell more remotes and a ton of extra receivers if you could make it work.
```

---
## \#234 Posted by: Wajdi Posted at: 2017-10-31T20:46:37.793Z Reads: 369

```
I just implemented a re-binding function inspired from the discussion of the firefly remote. It is necessary for people that want to use multiple receivers on the same remote. What was mostly stopping me from sending out the remotes is software improvement and testing. 

Today I finished assembling the first 10 remotes!
```

---
## \#235 Posted by: Wajdi Posted at: 2017-10-31T22:40:49.553Z Reads: 369

```
@Dizzee What do you mean by Model Memory? You can bind several receivers to the same remote, but incoming telemetry data will be randomly alternating.
```

---
## \#236 Posted by: Dizzee Posted at: 2017-11-01T07:53:07.403Z Reads: 390

```
@Wajdi The Model Memory allows you to save and recall everything you need to make switching between vehicles painless. Just select the stored vehicle from a list on the controller, that was previously configured and stored by the user, and you're ready to go without having to rebind or change anything else. In our case it could save the bound receiver along with the controller configuration. On the controller side all settings would be saved and stored so our button mapping, lighting schemes and so on can be instantly recalled. It was a major innovation when it was first introduced to the RC world. Once you experience it you'll never want to give it up. Take a look at how it was done on the FrSky Taranis or even an old Spectrum DX6i for examples of use. The Taranis uses opensource software so a peek at their coding may also help. I know you can't just copy it but it may give you some ideas. I really wish I had the patience for coding. It seems like such a cool way to create. My head just doesn't seem to be wired for it.
```

---
## \#237 Posted by: b264 Posted at: 2017-11-01T08:04:26.379Z Reads: 379

```
[quote="Wajdi, post:221, topic:24654, full:true"]
Can you guys help me pick up a name for the remote?
[/quote]

Call it "Widebody"
```

---
## \#238 Posted by: longhairedboy Posted at: 2017-11-01T11:16:38.067Z Reads: 372

```
i just ordered two of these.
```

---
## \#239 Posted by: longhairedboy Posted at: 2017-11-01T12:19:52.544Z Reads: 373

```
Also I agree, Photon is a killer name and just rolls off the tounge. ITs very sticky.  Its already kind of branded in my head, so you know its good.
```

---
## \#240 Posted by: Wajdi Posted at: 2017-11-01T16:03:41.400Z Reads: 382

```
@caustin Yes they are :slight_smile:

@notger I already implemented that feature, its called reactive effect, when you brake it turns your LEDs to red. Look by the end of the video to see it. About the kit option it still happening. I will announce it when its available. Very soon.

@Dizzee If I understand correctly, by Model Memory you mean saving user preferences? in that case thats already implemented in both the receiver and the remote. Any changes to lightening effects, sensitivity, stats, bindings, are all saved in in the micro controller memory.

@b264 Thanks but I will stick with Photon :grin:

@longhairedboy Thank you very much :slight_smile:
```

---
## \#241 Posted by: Deckoz Posted at: 2017-11-01T20:05:47.331Z Reads: 369

```
Soooo shipping this week like ya said right ? :)
```

---
## \#242 Posted by: Hardwiring Posted at: 2017-11-01T22:16:53.878Z Reads: 348

```
I'm looking forward to hearing more about this remote from the first batch of users, so far very interesting and tempting 
:+1:
```

---
## \#243 Posted by: Mikenopolis Posted at: 2017-11-01T22:24:43.262Z Reads: 338

```
Me too, can't pull the trigger until it's been tested and tutorials are up.
```

---
## \#244 Posted by: caustin Posted at: 2017-11-02T01:39:21.080Z Reads: 336

```
Kewl, one for each hand!  I want to see that video lol
```

---
## \#245 Posted by: longhairedboy Posted at: 2017-11-02T03:01:50.197Z Reads: 338

```
yeah cause i have a penny on each foot.
```

---
## \#246 Posted by: Deckoz Posted at: 2017-11-02T03:05:39.173Z Reads: 340

```
Why not just electrify some quadskates lol
```

---
## \#247 Posted by: longhairedboy Posted at: 2017-11-02T03:06:56.162Z Reads: 340

```
dude. If i just glued shoes to these pennies they would BE quads.
```

---
## \#248 Posted by: karatektus Posted at: 2017-11-02T05:42:37.254Z Reads: 347

```
@Wajdi quick security question since it has not been adressed yet: is the communication encrypted in any way? I would to see some scriot kiddie build a $20 box that sets the break or throttle to 100% of all passing riders.

Also: which frequencies are being used/at which transmit power does it operate?

Edit: Also: wouldnt it be better to just make a small hole for the lanyard? the printed ring will probably break of sooner or later.
```

---
## \#249 Posted by: longhairedboy Posted at: 2017-11-02T12:25:13.575Z Reads: 330

```
[quote="karatektus, post:248, topic:24654"]
wouldnt it be better to just make a small hole for the lanyard? the printed ring will probably break of sooner or later.
[/quote]

That's a good point. I didn't think about it but any dangly-doos will likely get knocked off during normal wear and tear.
```

---
## \#250 Posted by: karatektus Posted at: 2017-11-02T12:37:21.394Z Reads: 333

```
One more thing i cant get out of my head: wouldnt it be nice to have just a small 4-way joystick (like the one on fatsharks) for the remote control menu operationand a normal trigger(potentiometer) for the throttle? Its probably a little late but that would allow ppl to design their own cases and use any kind of trigger/stick/slider they like? (The image in my head is a boosted board remote with a screen and a little joystick on the side)
Its probably a little late now - maybe for v2? 

Furthermore: Is there a hybrid mode for the killswitch? like "Needs to be pressed to start driving - can be let go afterwards. If pressed WHILE driving -> cruise control"
```

---
## \#251 Posted by: Dizzee Posted at: 2017-11-02T15:16:29.871Z Reads: 321

```
That's part of it. What I'm asking for would allow the user to recall several configurations, each bound to a separate receiver. All the user does after the initial binding and setup is select the file name used  to be completely ready to hop on a different board. No rebinding or re entering anything unless making changes. If I'm not explaining it well enough please look at the radio models I listed earlier and search for the feature. Many RC radios for planes and quadcopters have this feature. It's a a standard feature in that hobby. Multiple saved configs for the same receiver can be part of it but that is not the primary purpose.
```

---
## \#252 Posted by: Wajdi Posted at: 2017-11-02T15:56:24.444Z Reads: 341

```
@karatektus The remote uses FHSS, therefore it would be very hard to interfere with its communication. 

it constantly hops between frequencies from 2.400 - 2.4835GHz. About transmit power, I don't have proper measuring tools, but it should be somewhere around 7dBm-10bBm. Adequate level for electric skateboard application, anything more and it will be an overkill + more power consumption.

Btw the battery on the remote can last more than 22 hours continuous, and over 30 days sleep mode.

The lanyard dongle is really tougher than it looks :grinning: I can't break it with both my hand at full force. It has 100% infill and it bounds very well with the case. 

About the redesign, maybe for V2, right now the remote is very compact and functional. Thanks for the suggestions.
```

---
## \#253 Posted by: Wajdi Posted at: 2017-11-02T16:02:22.049Z Reads: 345

```
@Dizzee I see what you mean. It should be possible to do. I will add it to my ToDo list and push it as an update later on. I can't work on it right now because I know may people want their remote ASAP :grinning:
```

---
## \#254 Posted by: Wajdi Posted at: 2017-11-02T20:53:06.585Z Reads: 380

```
<img src="/uploads/db1493/original/3X/8/b/8b566c492f97338f2df932b2b4ffbd6959e7f698.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/3X/8/3/8372c66bb7db34bbe5167bebf3e7420fc2ef638d.jpeg" width="375" height="500">

I’m post processing the 3D printed covers, what do you guys think? It’s much smoother and looks better in real life.
```

---
## \#255 Posted by: ElskerShadow Posted at: 2017-11-02T21:25:27.309Z Reads: 356

```
It looks great IMO. I think i will change the colour with my 3D printer if u share the files !
```

---
## \#256 Posted by: Holyman92 Posted at: 2017-11-02T21:30:00.065Z Reads: 353

```
i will be pre-ordering one soon, any idea when the ship outs will start?
```

---
## \#257 Posted by: Ricco Posted at: 2017-11-02T22:00:21.851Z Reads: 354

```
Those look great!  What did you do for post processing?  Did you use an acetone vapor chamber?
```

---
## \#258 Posted by: Wajdi Posted at: 2017-11-02T22:13:50.316Z Reads: 358

```
@ElskerShadow Cool! I will share the printing files pretty soon.
@Holyman92 I already sold out all my current units, I have placed a new order for parts and I should receive them in about 2 weeks from now. Hopefully they won't sold out before they arrive :sweat_smile:
@Ricco I used sanding, acetone, filler primer and paint coat.
```

---
## \#259 Posted by: Holyman92 Posted at: 2017-11-02T22:39:26.399Z Reads: 351

```
hey man i will use a nunchuck from a wii until u get stock if they sell out again
```

---
## \#260 Posted by: Wajdi Posted at: 2017-11-02T23:40:31.350Z Reads: 348

```
I recommend you pre-order now to reserve a spot, parts might ship sooner :slight_smile:
```

---
## \#261 Posted by: Holyman92 Posted at: 2017-11-03T00:04:11.706Z Reads: 355

```
i will as soon as my money hits my bank lol
```

---
## \#262 Posted by: ElskerShadow Posted at: 2017-11-03T08:56:09.354Z Reads: 342

```
I can sense a soon to come invasion of posts about this remote when we’ll get them. 
Seriously this remote will be a game changer for the DIY community
```

---
## \#263 Posted by: notger Posted at: 2017-11-03T09:47:57.800Z Reads: 368

```
For Sure.

I'm still waiting for some experiences.
Just lately i detroied two Mad-Munkey-GT2B remotes in quite Hard crashes.
I actually just ride offroad-MTB in really harsh terrain.
So i'm not sure if this amazing PHOTON remote is the right thing for me, or if i should just stock tons of GT2Bs for all my crashes.

But @Wajdi , again, if you ever think of cooperating with @Ackmaniac and making your remote compatible with his firmware (mainly the power.profile change)   i will be in the game.
i might just have to think about a Hardcore-Hadshell-Indexfinger-Trigger-Encloser  Alternative.
Cause riding harsh-offroad with a Thumb remote is not really possible in my experience.

But maybe you come up with a Index-Hardcore-Photon-Extreme Version as second option.

Until then i'm curious about all the experience .

Ang again. Amazing work youve done for the e-sk8 community!!
```

---
## \#264 Posted by: Wajdi Posted at: 2017-11-03T18:43:59.419Z Reads: 380

```
<img src="/uploads/db1493/original/3X/f/6/f61484e2ea83448fdb9ec14efe2cf1294ffdee29.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/f/b/fb2b23aaee02b5e6c043fb90ccbbc6e3870bb7b6.JPG" width="666" height="500">

This is what the final post processing result looks like, a smooth matte finish.
```

---
## \#265 Posted by: longhairedboy Posted at: 2017-11-03T18:45:40.914Z Reads: 361

```
That's not bad. Jake and i were talking about what we could do to polish them a little until you get the injection molding down. maybe some brushed on resin and a coat of enamel. 

Ours would be red of course!
```

---
## \#266 Posted by: chinzw Posted at: 2017-11-03T18:48:17.677Z Reads: 358

```
You can use high fill primer and then tumble the parts. That should give nice smooth matte finish.
```

---
## \#267 Posted by: Wajdi Posted at: 2017-11-04T21:36:11.921Z Reads: 353

```
Anyone has experience with injection molding? Do you know how much it approximately costs? 
Post processing those enclosures takes a lot of time, and I don't always have success with it. So I decided to keep it as is for now, it looks more consistent.
```

---
## \#268 Posted by: karatektus Posted at: 2017-11-04T21:41:26.561Z Reads: 349

```
for low runs its way cheaper to just use a sla printer i guess
```

---
## \#269 Posted by: DavidBanner Posted at: 2017-11-04T21:42:27.150Z Reads: 343

```
Injection moulding usually only makes sense with big runs, the moulds are not cheap to produce
```

---
## \#270 Posted by: Wajdi Posted at: 2017-11-04T22:36:16.146Z Reads: 342

```
I have access to an SLA printer, I will give it a try and see how tough the printed part is. I know it is more accurate than  FDM, I'm just worried about the strength.
```

---
## \#271 Posted by: DavidBanner Posted at: 2017-11-04T22:39:33.452Z Reads: 358

```
[quote="Wajdi, post:270, topic:24654"]
I have access to an SLA printer,
[/quote]

Nice! I can't wait to see what the results are like...
```

---
## \#272 Posted by: karatektus Posted at: 2017-11-04T22:39:45.917Z Reads: 357

```
SLA print it and do a casting mould. Good quality and still cheap
```

---
## \#273 Posted by: Hardwiring Posted at: 2017-11-05T15:44:31.437Z Reads: 378

```
It looks fine for now print wise and it's what people signed up for so they should be happy..... maybe offer case upgrade later for the first batch?? Still gonna wait and see how she performs in the wild before I pull the trigger.... 

pretty sure it'll be an awesome game changing remote, I really want one already, but this ain't my first forum so i'll await the release 

<img src="/uploads/db1493/original/3X/c/4/c41d849c63ec1ceb38cbfd5870e85ee6f092de32.gif" width="384" height="384">
```

---
## \#274 Posted by: Wajdi Posted at: 2017-11-05T15:50:29.644Z Reads: 365

```
That's what I have decided to do, I will keep it 3D printed with max setting, because Im getting inconsistent results with post processing, plus the paint leaves a weird smell on the remote. 
With max settings it takes about 10 hours to print 1 remote at 1.0mm accuracy, but its worth it.
```

---
## \#275 Posted by: notger Posted at: 2017-11-05T16:23:03.183Z Reads: 351

```
Hi,

ask @FLATLINEcustoms  Joel, he drid Molds for his Mad-Munkeys.
So he might know more about costs, and id you look at the difference of the encolure Quality Mold or Print it's amazing.
```

---
## \#276 Posted by: mishrasubhransu Posted at: 2017-11-06T19:31:32.018Z Reads: 339

```
[quote="Wajdi, post:274, topic:24654"]
bout 10 hours to print 1 remote at 1.0mm accuracy, but its worth it.
[/quote]

 Why don't you send it to shapeways.com and get it printed in "strong and flexible plastic" which is basically nylon. I use it for various thick and thin robot parts and it has yet to disappoint me.
```

---
## \#277 Posted by: Wajdi Posted at: 2017-11-06T20:09:45.770Z Reads: 338

```
Thanks for the suggestion, the 3D prints are actually of very good quality and strong. :+1:
```

---
## \#278 Posted by: lrdesigns Posted at: 2017-11-07T01:23:11.790Z Reads: 354

```
For injection molding you need to make at least 1000 parts to break even. Even in china a really cheap tool for this would be at least $2000 usd, but the more normal price is closer to $5000. If your lucky you can put both halfs in one tool and not have to buy two molds. :anguished:

SLA makes very nice prints but the material is usually quite brittle and colors very limited. Some printers have suitable materials though, Formlabs have a resin that is similar to PP which is very impact resistant, would be good for a remote. 

Making a silicone mold from a SLA print is a good middle ground though for quantities around 200 pieces.
```

---
## \#279 Posted by: Mikenopolis Posted at: 2017-11-07T01:32:09.341Z Reads: 353

```
What about those filaments with carbon fiber?

Making molds are expensive as hell. My dad made products back in the 80's and 90's and had to sell a few houses he owned to fund his inventions. He died 13 years ago before all the great tech gadgets we enjoy existed. He would've loved 3d printing.
```

---
## \#280 Posted by: ossieeskar Posted at: 2017-11-07T10:20:53.438Z Reads: 356

```
Will you be selling anytime soon? Can I order one as soon as you do? It looks awesome
```

---
## \#281 Posted by: Wajdi Posted at: 2017-11-09T05:05:44.238Z Reads: 403

```
Design in progress.
<img src="/uploads/db1493/original/3X/7/f/7f218dcfeca8f91c37992d3e3e7adc6a000a90ef.png" width="560" height="500">


Hey guys, I had several improvement ideas for the Photon remote that I was saving for version 2, but I decided to upgrade it right now and send everyone the newest/improved version. It won't be cool to send an old version to everyone that waited that long, just to release version 2 after a couple weeks.

The improved version has:

* A much slimmer body
* Even more reliable connectivity, using PA/LNA modules that have accurate antenna impedance matching network.  
* 900mAh battery with over 20 hours continuous/30 days sleep
* Redesigned PCBs now with built in Joystick, more reliable.
* Receiver PCB now has dedicated port for WS2812B RGB strip
* And a couple hardware redesign/tweaking for optimization

<img src="/uploads/db1493/original/3X/b/6/b6bf7be8f1a12407fa334728fc0e7e8a0eb0a722.png" width="560" height="500">

New PCBs are already in the fabrication stage, I should receive it in about a week and a half. 
New enclosures are being 3D printed now. I should be able to assemble the new version as soon as I receive the PCBs. Assembling/testing will only take 1-2 days.

Let me know what you think!
```

---
## \#282 Posted by: Wajdi Posted at: 2017-11-09T08:43:12.840Z Reads: 407

```
Updated design, much more slimmer, and ergonomic! size is reduced by almost 50%. 

<img src="/uploads/db1493/original/3X/b/6/b6bf7be8f1a12407fa334728fc0e7e8a0eb0a722.png" width="560" height="500"><img src="/uploads/db1493/original/3X/3/c/3c0366ea9d6b27e6ac7f77c0eb5658fee77e98dd.png" width="560" height="500"><img src="/uploads/db1493/original/3X/1/3/1312445425d146f85bf3e051d2cb41307c060592.png" width="560" height="500">

Let me know what you think.
```

---
## \#283 Posted by: notger Posted at: 2017-11-09T09:10:13.685Z Reads: 407

```
I really like it, i actually asked myself how much electronics must be in htere that i has to be that big.

Another Question again: :sweat_smile:  do you think you will Design a Index-Finger-Trigger Version, or will that be up to the Cummunity as soon the first PCB-DIY-Set are out for sale ?
As template there are quite some proofen designs like:
https://www.thingiverse.com/thing:2066350
https://www.thingiverse.com/thing:1550237
https://www.thingiverse.com/thing:1625376
https://www.thingiverse.com/thing:922378
```

---
## \#284 Posted by: Print3r Posted at: 2017-11-09T14:22:45.232Z Reads: 380

```
What post-processing are you using?
```

---
## \#285 Posted by: NAF Posted at: 2017-11-09T14:35:50.962Z Reads: 383

```
Looks awesome. What did you use to polish it like that?
```

---
## \#286 Posted by: longhairedboy Posted at: 2017-11-09T14:46:51.078Z Reads: 378

```
my god its beautiful.
```

---
## \#287 Posted by: caustin Posted at: 2017-11-09T14:59:48.675Z Reads: 382

```
Looks great, much improved, not much I can add other than maybe a fiercer font for PHOTON brand engraving!  Of course @longhairedboy will also want that in red, for performance boosting purposes lol.
```

---
## \#288 Posted by: longhairedboy Posted at: 2017-11-09T15:10:16.966Z Reads: 371

```
the very thought of a red photon remote makes me want to sob softly out of pure elation.
```

---
## \#289 Posted by: Brianr058 Posted at: 2017-11-09T16:36:24.495Z Reads: 369

```
that's a cad not production
```

---
## \#290 Posted by: Ricco Posted at: 2017-11-09T17:05:13.291Z Reads: 362

```
That's not the post he's referring to
```

---
## \#291 Posted by: Wajdi Posted at: 2017-11-09T17:22:13.275Z Reads: 375

```
@Print3r @NAF I used sanding, acetone, filler primer and paint coat, but I won't be post processing the cases anymore because the paint coating leaves a weird smell on the remote, especially on hot conditions. 

@notger @longhairedboy Thank you! glad you guys liked the new redesign. This version is much more compact it makes the old design looks so big!

@caustin Thanks! If you guys have font suggestions please let me know :slight_smile:
```

---
## \#292 Posted by: longhairedboy Posted at: 2017-11-09T17:25:57.680Z Reads: 361

```
Have i mentioned i NEEEEED THEEEEEESE. 

Lord Skatan, grant me patience for the things i feel i can't wait for. And DO IT NOW.
```

---
## \#293 Posted by: Deckoz Posted at: 2017-11-09T19:30:19.220Z Reads: 360

```
I need mine too...my remote is broken lol... Was expecting a shipping label last week :frowning:
```

---
## \#294 Posted by: Brianr058 Posted at: 2017-11-09T22:35:51.895Z Reads: 362

```
I predict 30 days minimum for the first batch pre-orders to see product. maybe a x-mas present to ourselves!:unamused:
```

---
## \#295 Posted by: Deckoz Posted at: 2017-11-09T23:25:33.549Z Reads: 377

```
Are you speaking for him? If not...lol.

<img src="/uploads/db1493/original/3X/7/6/76e854c38f288038f53676104a752ea0e1af1d55.png" width="281" height="500">
```

---
## \#296 Posted by: banjaxxed Posted at: 2017-11-09T23:28:03.006Z Reads: 364

```
Can you incorporate an android phone? It's wonderful
```

---
## \#297 Posted by: Brianr058 Posted at: 2017-11-09T23:43:42.748Z Reads: 356

```
I may as well be but no this is just me hoping I see my remote before x-mas! I'm now forced to purchase another remote If I wish to ride my first build in a week!
```

---
## \#298 Posted by: Wajdi Posted at: 2017-11-10T01:00:51.275Z Reads: 358

```
@Deckoz @Brianr058 @longhairedboy  I will do my best to get it going in about 2 weeks :slight_smile:
```

---
## \#299 Posted by: Wajdi Posted at: 2017-11-12T05:16:21.215Z Reads: 363

```
@notger I might design an index finger version in the future, but it I don't have a definite date yet. Of course the community can always get creative with the DIY kits (I will be offering those soon)

@banjaxxed What do you mean, Like an android app?
```

---
## \#300 Posted by: banjaxxed Posted at: 2017-11-12T07:12:52.650Z Reads: 354

```
I was only kidding , I meant that it should incorporate an actual android phone...although that could end up being a thing in the future...
```

---
## \#301 Posted by: kanguru007 Posted at: 2017-11-13T10:27:00.815Z Reads: 353

```
The most important thing for me: what is the control update rate?
(I'm getting ready to VESCify my Bamboo GTX because of its slow update rate)
```

---
## \#302 Posted by: scepterr Posted at: 2017-11-13T10:39:39.350Z Reads: 341

```
Slimmer version in 2 weeks?
```

---
## \#303 Posted by: longhairedboy Posted at: 2017-11-13T12:24:39.970Z Reads: 353

```
[quote="banjaxxed, post:300, topic:24654"]
I meant that it should incorporate an actual android phone
[/quote]

Then when your remote gets infected with malware you can just tap past the ads to get to your throttle control!
```

---
## \#304 Posted by: Necromenz Posted at: 2017-11-13T17:33:23.689Z Reads: 357

```
Hi,

I like the remote! I have any question. 
1.Has anyone use the remote with a Dual Vesc6 system?
2. can i use the nrf chip of the Vesc6?

Thx for help.
```

---
## \#305 Posted by: Deckoz Posted at: 2017-11-13T18:16:12.686Z Reads: 348

```
No one has it yet......

:(
```

---
## \#306 Posted by: Wajdi Posted at: 2017-11-13T19:40:35.992Z Reads: 349

```
@Necromenz 1. It should work with dual VESC setup, you can run a CAN bus, and connect the receiver to the master VESC.
2. The remote comes with its own receiver, you don't need to use the nrf chip of the Vesc.
```

---
## \#307 Posted by: Necromenz Posted at: 2017-11-13T20:00:20.983Z Reads: 336

```
Thx for your awnser.
I ask for the Vesc6 because a old or wrong UART command brick the STM32 Chip of the Vesc6 .
```

---
## \#308 Posted by: Wajdi Posted at: 2017-11-13T20:04:39.773Z Reads: 336

```
Interesting, I wasn't aware of that, do you have more information on this?
```

---
## \#309 Posted by: longhairedboy Posted at: 2017-11-13T20:16:16.454Z Reads: 334

```
That's an interesting bug. Can it be recovered by reloading the firmware?
```

---
## \#310 Posted by: Necromenz Posted at: 2017-11-13T20:24:46.917Z Reads: 381

```
Yes you can fix it with a stm32link. I brick one of my Vesc6 with a bt Modul over UART.

Here are the post of hexacopter Bens awnser out of the Beta Forum : 


The maybe most important thing I noticed was the behavior connecting a BT 4.0 module to the UART port and use the metr.at logging app to see if some data could be read. I thought it just couldn’t connect and doesn’t read any data because of a different serial protocol, but it was much worse. Connecting the app to the VESC just fried the STM32. No LEDs were blinking after a reboot and the VESC wasn’t found any longer over USB. Tried different things, but just flashing an old VESC firmware over JTAG with an STLink V2 revives the VESC. Looks like nothing is damaged permanently, but not everyone is able to flash a new firmware over JTAG and I am not 100% sure if really nothing of the hardware was damaged by this. But amazing that it is so easy to brick the STM just with a few UART commands. Wasn't expecting that.

SO TO ALL BETAs. DONT USE ANY OLD SMARTPHONE APP TO CONNECT TO YOUR VESC OVER BLUETOOTH, WHEN YOU DONT WANT TO RISK TO BRICK YOUR NEW VESC 6.

I have only tested with the metr.at app and investigate with Roman (the developer of the app) the following. It looks like command codes for COMM_GET_MCCONF and COMM_GET_APPCONF are 0E and 11 in FW3.24, when in the old FW2.18 the codes are 0D and 10. So instead of sending COMM_GET_MCCONF in metr.at app, I was probably most likely sending COMM_SET_MCCONF. Because of this my VESC was bricked afterwards. We fixed that behavior and also analyzed the serial data so data logging for FW3.24 should work in future versions of the app. But the best way would be getting the source code of VESC Tool and the firmware so we can confirm that and also compile the GUI for Mac.

Ben:

For now I don't recommend using any old app or device with the new firmware since the communication protocol has changed quite a bit. Also, I don't really like the model of making closed source apps that communicate with the VESC, so I would like to get support for mobile devices into the code base of VESC Tool as soon as possible. There are already preparations for that by separating the communication and configuration code from the user interface. 

I hop it helps.
```

---
## \#311 Posted by: longhairedboy Posted at: 2017-11-13T20:56:06.037Z Reads: 330

```
i just bought a couple of those from Dexter. I'm going to try downgrading back to 2.18 on one of my older VESC-Xs.
```

---
## \#312 Posted by: Necromenz Posted at: 2017-11-13T21:04:43.058Z Reads: 328

```
I dont know if its allways happens. It couldt be fix with a newer fw or it works with this Modul.
That is the reason why i asked if it works with the Vesc6.
```

---
## \#313 Posted by: Wajdi Posted at: 2017-11-13T23:59:03.195Z Reads: 334

```
Seems like the issue only happens on COMM_GET_MCCONF/COMM_SET_MCCONF commands which I don't use. 
There is a difference between Vesc 6 and Vesc 4 firmware when dealing with UART communications, mainly when reading the data packet, on Vesc 4 firmware it has 7 x float16 (2 bytes * 7)  data for temperature readings, while on Vesc6 it only has 2 x float16 ( 2 bytes * 2).

My remote is compatible with both versions, however I only tested on Vesc 4 because that's what I have right now.
```

---
## \#314 Posted by: PredatorBoards Posted at: 2017-11-14T00:59:31.760Z Reads: 339

```
Add some higher weight springs to the x-axis and you have yourself an awesome product. Talk with @Ackmaniac and see if a more fleshed out version of Torque Vectoring is possible. I'd pay good money for that.
```

---
## \#315 Posted by: ShutterShock Posted at: 2017-11-14T01:10:19.072Z Reads: 332

```
Yeah thats just a render
```

---
## \#316 Posted by: Ricco Posted at: 2017-11-14T01:49:46.506Z Reads: 327

```
They were referring to the pictures of the post processed cases way before the rendering
```

---
## \#317 Posted by: ShutterShock Posted at: 2017-11-14T02:23:45.307Z Reads: 326

```
Ah. My bad
```

---
## \#318 Posted by: Necromenz Posted at: 2017-11-14T09:43:37.404Z Reads: 341

```
Thx for the Informations!
You ship the Remote to Germany? So i will preorder the Remote and Test with my Vesc6.
```

---
## \#319 Posted by: SkaterBoy58 Posted at: 2017-11-19T23:04:56.896Z Reads: 353

```
Wajdi - Could you please post a photo or sketch of receiver showing dimensions and wiring - just designing enclosure  internal layout and need to allow enough space
Cheers
```

---
## \#320 Posted by: Wajdi Posted at: 2017-11-19T23:18:06.373Z Reads: 358

```
Here are the dimensions, in mm. Let me know if you need something else.

<img src="/uploads/db1493/original/3X/b/2/b21ab72c799de76a0ddc08f12b18c3da7d83e866.PNG" width="315" height="162">
```

---
## \#321 Posted by: Wajdi Posted at: 2017-11-19T23:19:01.679Z Reads: 349

```
Yes I ship to Germany :slight_smile:
```

---
## \#322 Posted by: SkaterBoy58 Posted at: 2017-11-20T01:51:23.873Z Reads: 335

```
many thanks -
 is the antenna in that receiver pcb footprint?
and what form are the pin-outs ( JST ?) or are they solder points
```

---
## \#323 Posted by: Wajdi Posted at: 2017-11-20T03:11:58.998Z Reads: 330

```
Yes antenna is within that PCB footprint.
The UART port on the most left side is a 6pin JST PH 2mm pitch. The connector will be pre-soldered, unless you prefer not. 
The 3 pins on the bottom right side are solder points for a WS2812B LED strip.
The 9 pins on the top are various digital and analog pins, two pins on those will be used to enter automatic binding mode. A pre-soldered 2 pin male header will be installed on the binding pins, and a jumper will be provided.
```

---
## \#324 Posted by: SkaterBoy58 Posted at: 2017-11-20T04:09:37.755Z Reads: 343

```
Wajdi - Thanks for that - so UART connector  will be pre-soldered so I could use a 6pin JST female to female to connect receiver UART to VSEC UART port?

Regarding the 9 pin header - does this need a 9 pin JST with two of these as binder or a separate 2 pin JST ( binding) with the balance on a 7 pin JST plug?

Any chance of a wiring diagram showing the external connections ?

Cheers
```

---
## \#325 Posted by: Wajdi Posted at: 2017-11-20T04:54:43.975Z Reads: 363

```
Yes, the female to female connector cable will also be provided.
Here the wiring diagram to get a better idea.

The MISO, SCK, and MOSI pins will be removed in next versions, I don't see any practical use of it.

<img src="/uploads/db1493/original/3X/1/9/196a1be9182f14181d20cfa9b5f13fb27738230c.PNG" width="400" height="240">
```

---
## \#326 Posted by: scepterr Posted at: 2017-11-20T05:03:19.817Z Reads: 360

```
2-3 coats of this provides a soft touch rubber feel to any prints, great at filling imperfections too
<img src="/uploads/db1493/original/3X/3/f/3fa528f3c87591d5bc7fd61f8c76710daaa4f40a.jpg" width="576" height="499">
 http://a.co/am4d8Hn
```

---
## \#327 Posted by: Wajdi Posted at: 2017-11-20T05:05:40.398Z Reads: 334

```
Awesome! didn't know about this, did you try it? I'm curious to see the results.
```

---
## \#328 Posted by: scepterr Posted at: 2017-11-20T05:06:21.108Z Reads: 322

```
Yeah I'll post some pics tomorrow, spent the last couple days painting prints 😋 no post processing other than paint
```

---
## \#329 Posted by: Wajdi Posted at: 2017-11-20T05:07:01.690Z Reads: 318

```
Cool, thanks for sharing, I will order one :grin:
```

---
## \#330 Posted by: scepterr Posted at: 2017-11-20T05:14:07.767Z Reads: 314

```
Just make sure it's the low gloss one, also I haven't checked if there are other colors...😉
```

---
## \#331 Posted by: SkaterBoy58 Posted at: 2017-11-20T05:24:28.989Z Reads: 330

```
Hi Kanguru007 - I have just finished upgrade on my BGT with dual VESCs  with CAN data - Have ordered this remote but operating on a spare RC remote in the mean time.  Let me know if you want any details or the VESC motor/app data files
Cheers  ( PS Are you in Aus?)
```

---
## \#332 Posted by: Wajdi Posted at: 2017-11-20T05:34:39.575Z Reads: 322

```
@kanguru007 Sorry I missed your post, update rate is less than 1ms, that's with driving the large RGB LCD, constantly refreshing data, performing FHSS, Interactive UI, and smoothing out the analog inputs. Its fairly optimized, and pretty impressive performance from the 32bit CPU.
```

---
## \#333 Posted by: SkaterBoy58 Posted at: 2017-11-20T05:54:13.115Z Reads: 333

```
Waji
 Thanks for that 
What is maximum allowable voltage on the RGB +3V3   . I have a 12V supply in board for lights etc. and want to power the receiver  LED circuitry off this rather than using VESC supply.( The LED strip has +12V    data in    and  0V connections)

Also - the D5,  A0 and  A1 Digital outputs - presumable these can directly connect to a gate pin on a N Channel MOSFET  for driving horns , lights etc
```

---
## \#334 Posted by: Wajdi Posted at: 2017-11-20T06:06:06.560Z Reads: 323

```
Sorry I made a small mistake on the PinOut picture, the +3V3 pin on the led port is actually +5V coming from the VESC through the UART cable, you can easily use a 5 pin UART cable instead and feed your 12v supply to the 6th pin.

Regarding the D5 and A0 pins they can be used as gate controllers for your Mosfets. A1 is used to drive the LED strip so it’s not available.
```

---
## \#335 Posted by: Wajdi Posted at: 2017-11-20T07:04:39.330Z Reads: 342

```
Here is a detailed Pinout, if you want to use your +12v supply, you can connect it to either of the circled locations, just make sure you have common ground by connecting your supply ground to the GND pin.

<img src="/uploads/db1493/original/3X/0/5/05a64adff99317a0f59b78ffc2fedde498799f13.PNG" width="400" height="240">

What LED strip will you be using? is it WS2812B or similar?
```

---
## \#336 Posted by: SkaterBoy58 Posted at: 2017-11-20T08:07:36.765Z Reads: 333

```
WS2811 5050 RGB LED Strip Light Waterproof Addressable Tube DC12V Black Shell BN

It has three connections   1)+12V     2)data input   and     3)  0V  

So if I read your post correctly I can connect board +12V supply to pin 6 of receiver UART plug  and then connect

+12V wire   from led strip to receiver  +5V  pin
data input wire  from led strip to receiver A1 pin
0V wire from  led strip to receiver GND pin
0V from 12V supply to received GND pin
```

---
## \#337 Posted by: Wajdi Posted at: 2017-11-21T01:42:17.176Z Reads: 320

```
Yes that should be it.
```

---
## \#338 Posted by: SkaterBoy58 Posted at: 2017-11-22T23:36:15.357Z Reads: 331

```
Wajdi - Is the UART +5V connection( pin 6 )  hard wired to the +5V on LED strip conn via pcb track?  

I would like to power receiver from VESC ( via UART pin 6 ) but power LEDS from separate 12V supply with common  0V ?

BTW - What is your latest forecast date for shipping first batch?

Cheers
```

---
## \#339 Posted by: Wajdi Posted at: 2017-11-23T00:07:37.947Z Reads: 367

```
Yes UART +5v(pin 6)  is hardwired to +5v LED strip conn via pcb trace.

However the receiver is not powered from that +5v pin, its powered from the +3v3 pin (pin 5). So you will be able to power the receiver directly from the UART connection, even if you use pin 6 for something else, in this case, +12V.

An update on latest development: I received the new PCBs, and they are perfect. They fit nicely on the new enclosure, and the built in joystick footprint makes it more compact and firm. 

<img src="/uploads/db1493/original/3X/6/0/60f1684d5d1c8042b7cca619deccd866f0fb3b4e.jpg" width="588" height="500"><img src="/uploads/db1493/original/3X/2/4/247bfa2e91f12a5323d021c98f6ac81b0fdf6d72.jpg" width="531" height="500">

I added an auto-calibration wizard to the remote menu, it is very easy to re-calibrate the joystick in case it was changed or was de-calibrated for some reason. During the calibration process I also added a deadzone adjustment.
I'm pre-soldering the PCBs as we speak, and waiting for the new nrf24 modules to be delivered, it should take a couple days before I have everything nicely put together.
```

---
## \#340 Posted by: Wajdi Posted at: 2017-11-23T01:15:25.407Z Reads: 355

```
What Vesc FW are you guys using? Seems like everyone is running different versions which makes it harder to keep track of. If you guys can tell me what HW and FW versions you are using it would help me create a wider compatibility. 
Perhaps there should be a a new thread with a poll to see what everyone has.
```

---
## \#341 Posted by: nw-esk8 Posted at: 2017-11-23T03:06:47.707Z Reads: 350

```
Err on the side of newer/latest, IMO.
```

---
## \#342 Posted by: SkaterBoy58 Posted at: 2017-11-23T03:47:51.126Z Reads: 332

```
HW 4.12  FW 3.31

Cheers
```

---
## \#343 Posted by: ElskerShadow Posted at: 2017-11-23T15:54:20.534Z Reads: 324

```
So can we expect our remotes for chrismas ? Or will it be in January ? :)
```

---
## \#344 Posted by: Wajdi Posted at: 2017-11-23T16:04:26.085Z Reads: 329

```
Before Christmas for sure, you can expect it to be shipped any day now. I soldered the PCBs yesterday, and I'm flashing the software as we speak. :+1:
```

---
## \#345 Posted by: ElskerShadow Posted at: 2017-11-23T16:11:03.990Z Reads: 343

```
Great news. My hype is non-scalable right now.
```

---
## \#346 Posted by: Wajdi Posted at: 2017-11-23T18:57:25.843Z Reads: 367

```
Fresh and shinny :slight_smile:

<img src="/uploads/db1493/original/3X/c/d/cdfd7b8514ff4b3f498fba801c65431f7e8dbc48.JPG" width="375" height="500">
```

---
## \#347 Posted by: uigiroux Posted at: 2017-11-24T21:58:47.093Z Reads: 350

```
I was looking for a remote for my Carvon V4's build, and just came across yours and wow it looks amazing!  One question I have though, is since I'll be running 2 VESC's, I'll need 2 transmitters to make it work, so will you be able to provide extra transmitters for those of us who have multiple motors /VESC's?
```

---
## \#348 Posted by: Wajdi Posted at: 2017-11-24T22:04:33.464Z Reads: 336

```
@uigiroux Yes. I will add an option to purchase the receiver standalone.
```

---
## \#349 Posted by: uigiroux Posted at: 2017-11-24T22:08:58.554Z Reads: 333

```
Awesome, so have you figure out what your remote will cost, and how much will an extra transmitter be?  Do you have a projected date for when these will be ready to ship out?
```

---
## \#350 Posted by: karatektus Posted at: 2017-11-24T22:47:41.047Z Reads: 338

```
[quote="uigiroux, post:347, topic:24654"]
on I have though, is since I'll be running 2 VESC's, I'll need 2 transmitters to make it work, so will you be able to provi
[/quote]

you only need one receiver per board. regardless of the amount of vescs/ motors. they should talk via canbus.
```

---
## \#351 Posted by: Wajdi Posted at: 2017-11-24T22:49:23.220Z Reads: 344

```
Yes, I already have the remote on Pre-order, 129$ for the remote+receiver, and 39.99$ for the receiver standalone. This is an introductory price, and it will more than likely increase a bit once it is finalized.
The production cost and effort involved into making those remotes is so much high compared to the revenue I make from it.
```

---
## \#352 Posted by: uigiroux Posted at: 2017-11-24T22:53:29.350Z Reads: 338

```
And these work with the VESC - X (FOCBOX) right?
```

---
## \#353 Posted by: Wajdi Posted at: 2017-11-24T23:00:28.943Z Reads: 345

```
Yes, they are compatible with the FOCBOX. Btw what firmware version are you using?
```

---
## \#354 Posted by: uigiroux Posted at: 2017-11-25T02:05:53.680Z Reads: 353

```
Lol none right now, I'm getting my parts together to do my build soon.  I'll probably get the one that Enertion's got on sale. Not sure which version that is..
```

---
## \#355 Posted by: Wajdi Posted at: 2017-11-26T00:30:29.501Z Reads: 373

```
Flashed and almost ready to be dispatched. 

<img src="/uploads/db1493/original/3X/0/4/04ca54eb2844a5654002268cd6e04665502778e9.jpg" width="375" height="500">
```

---
## \#356 Posted by: ElskerShadow Posted at: 2017-11-26T11:41:27.538Z Reads: 366

```
Show us a picture of the barbone remote with the screen please ! Wanna see that georgous body in action
```

---
## \#357 Posted by: Wajdi Posted at: 2017-11-29T00:43:36.003Z Reads: 374

```
<img src="/uploads/db1493/original/3X/8/2/8206771ac28b6c53306446545b6c3ccf0e0647b5.JPG" width="551" height="500">
```

---
## \#358 Posted by: Skyv4n Posted at: 2017-11-29T01:05:48.837Z Reads: 364

```
Nice job ! can you add turn and brake lights control like [this](https://hackaday.io/project/20364-animated-led-braketurn-signals-for-rc-and-esk8#menu-description) and use the buzzer like a horn ?
```

---
## \#359 Posted by: Wajdi Posted at: 2017-11-29T01:14:35.990Z Reads: 368

```
@Skyv4n Thanks, yes its definitely possible, it already has horn/buzzer digital control built in and WS2812B lights driver. Turn signals and reactive brakes are already added and working :slight_smile: I will post a demo video about it.
```

---
## \#360 Posted by: Deckoz Posted at: 2017-11-29T13:52:07.243Z Reads: 357

```
Looking good @Wajdi
```

---
## \#361 Posted by: Genius2017 Posted at: 2017-11-30T00:20:13.770Z Reads: 361

```
@Wajdi Sweet!
```

---
## \#362 Posted by: Hardwiring Posted at: 2017-11-30T23:58:07.103Z Reads: 345

```
Nice....... you do beautiful work..... so errr how's it going in the wild..... what are the first customers finding with lag etc? Just wondering because it still looks really good 👍
```

---
## \#363 Posted by: mmaner Posted at: 2017-12-01T14:23:17.714Z Reads: 346

```
@Wajdi what is the delivery time looking like?  Do you think we will get delivery by Christmas?
```

---
## \#364 Posted by: Wajdi Posted at: 2017-12-01T14:43:16.108Z Reads: 349

```
Yes, most of them were packed yesterday :slight_smile: Monday will start shipping those bad boys out, going to miss them tho :frowning2:
```

---
## \#365 Posted by: MorrisHsu Posted at: 2017-12-01T16:48:31.119Z Reads: 344

```
It looks great～
Where can I buy it?
```

---
## \#366 Posted by: Wajdi Posted at: 2017-12-01T18:54:35.865Z Reads: 344

```
You can buy it at www.eboardshop.net
```

---
## \#367 Posted by: ElskerShadow Posted at: 2017-12-02T12:20:21.713Z Reads: 344

```
How many will ship ? 
Hope i’ll get mine next week then !!!
```

---
## \#368 Posted by: Lobap Posted at: 2017-12-02T13:03:00.755Z Reads: 350

```
Awesome, very nice work!
```

---
## \#369 Posted by: Knives186 Posted at: 2017-12-02T14:36:15.629Z Reads: 353

```
Can you post a picture of the completed remote and receiver?
```

---
## \#370 Posted by: Deckoz Posted at: 2017-12-02T14:42:10.188Z Reads: 361

```
[quote="Wajdi, post:364, topic:24654"]
Yes, most of them were packed yesterday :slight_smile: Monday will start shipping those bad boys out, going to miss them tho :frowning2:
[/quote]

Sweet baby Jesus.
```

---
## \#371 Posted by: Whitehawk Posted at: 2017-12-04T10:05:24.874Z Reads: 357

```
+1 I'm interested with one remote but I would like to see the final design with a picture.
Thank you !
```

---
## \#372 Posted by: Kug3lis Posted at: 2017-12-04T11:24:01.453Z Reads: 371

```
The screeen looks same module as Evolve is using :D
```

---
## \#373 Posted by: uigiroux Posted at: 2017-12-06T02:39:21.844Z Reads: 400

```
When will your next shipment be ready?
```

---
## \#374 Posted by: Wajdi Posted at: 2017-12-06T04:33:37.224Z Reads: 422

```
I have been working on an enclosure for the receiver and it turned out to be pretty good! Here are some pictures of the final product. I started shipping those in FIFO, assembling one of those really takes up a LOT of time, much more than I ever expected, so please be patient :slight_smile:

<img src="/uploads/db1493/original/3X/7/8/78a2eec899266cef04cddd7a7420845b6d9a1e18.jpg" width="500" height="500"><img src="/uploads/db1493/original/3X/3/c/3c226095a996dc9a728b12b533896d581ae62dae.jpg" width="500" height="500"><img src="/uploads/db1493/original/3X/d/4/d4b41fb3d5d2f418d04af33ffb94dd8d936e9c99.jpg" width="500" height="500"><img src="/uploads/db1493/original/3X/c/3/c35d18016d0a3182771435842286aaa0c9d2d275.jpg" width="500" height="500">
```

---
## \#375 Posted by: mishrasubhransu Posted at: 2017-12-06T05:20:06.692Z Reads: 396

```
Looks good, but I was wondering if you ever gave shapeways nylon("strong and flexible plastic")  a try? Did it turn out to be too expensive?
```

---
## \#376 Posted by: Wajdi Posted at: 2017-12-06T05:34:23.833Z Reads: 409

```
The remote enclosure is very strong, I bet if a car rolls over it it won’t break, serious! :grin:  I have set the walls to be very thick with 100% infill. 

I didn’t try shapeways but I expect it to be very expensive.
```

---
## \#377 Posted by: uigiroux Posted at: 2017-12-08T02:06:24.515Z Reads: 413

```
Hey I just created a thread where I mention your remote and I figured who better to ask than you about what I am trying to do.  I want to create my own deck with an LCD on the top front like in the FIBOARD
 <img src="/uploads/db1493/original/3X/3/3/339e61cbc84d97ef5d28b74b7c64b7d399d701eb.jpg" width="690" height="383">

Since you have many of those stats on your remotes LCD, how hard would it be to create something like this to put on my custom deck?
```

---
## \#378 Posted by: danielz Posted at: 2017-12-08T03:53:58.879Z Reads: 406

```
Just use a cheap android phone, set it to autoboot when power is applied via usb and then auto open whatever app you use for telemetry. I used to do this with a tablet in my car. You can even set a nice custom boot logo. Ill be adding one to my board at some point.
```

---
## \#379 Posted by: uigiroux Posted at: 2017-12-08T04:13:25.608Z Reads: 406

```
That's a good idea but I was thinking of something more propose built.  Could I install one of those apps on a raspberry pi and hook that too a LCD and mount it up there?
```

---
## \#380 Posted by: ElskerShadow Posted at: 2017-12-08T06:41:33.255Z Reads: 400

```
You would need to develop a program for the rasberry pi and i think that a rasberry pi + screen etc will be too bulky
```

---
## \#381 Posted by: wafflejock Posted at: 2017-12-08T06:56:50.735Z Reads: 397

```
Raspberry Pi zero is pretty small and probably can still deal with driving an LCD through HDMI (pretty sure it still has fairly decent gpu capabilities) That said you would need some sort of plexiglass box or something to protect it all and do some vibration dampening I imagine.

B/W OLEDs and using an arduino or other low power MCU will be less power hungry for sure but not much smaller volume wise.
```

---
## \#382 Posted by: ElskerShadow Posted at: 2017-12-08T07:02:56.099Z Reads: 380

```
Yeah arduino would be bettery I think
```

---
## \#383 Posted by: PredatorBoards Posted at: 2017-12-08T07:04:04.390Z Reads: 392

```
May I interject? Dont bother with board-mounted data clusters. You really shouldn't be staring straight down and dropping your focus on the road, even if it's for a second. Good chance if you're checking the speedometer, you're likely going 'fast' and thus already in a riding situation that requires every possible millisecond for reacting to hazards. You're better off just buying a smartwatch and loading an odometer app.
```

---
## \#384 Posted by: wafflejock Posted at: 2017-12-08T07:21:14.605Z Reads: 379

```
Yeah actually totally agree even having the voltage/amperage meter on the board I would only look at at when I was stopped or making a conscious effort to stare at it in which case I was splitting attention between riding and looking at numbers.
```

---
## \#385 Posted by: Wajdi Posted at: 2017-12-08T18:30:43.947Z Reads: 379

```
It depends on the route you want to take to build it, if you are going to design a custom hardware + software then it will take a lot of time to finally polish it. If you are going to use pre-made arduino board then you would still need to develop the software, find out what display you might want to use, is it RGB or just monocolor like the one they use? Figure out the power requirements for each component and build everything into a compact module.

To be honest I like the idea of a built in display on top of the deck, of course you don't want to stare at it when you are going over 20mph or even slower. But it would be very cool to have it display your battery percentage and some stats when you first power on your board, and taking a glimpse at it from now and then when you come to a full stop..
```

---
## \#386 Posted by: uigiroux Posted at: 2017-12-08T19:52:02.925Z Reads: 352

```
Yeah I was thinking of using it not so much while actually riding the board but like the apps where it shows the telemetry from the VESC on performance data I could pull it up there rather than have to use a phone or smart watch etc..
```

---
## \#387 Posted by: nw-esk8 Posted at: 2017-12-08T21:22:02.399Z Reads: 340

```
You've started shipping :grinning:?  

I think I had the first order placed... are you sending any updates/tracking details on shipment?
```

---
## \#388 Posted by: Wajdi Posted at: 2017-12-08T21:31:49.195Z Reads: 338

```
Yes, PM me your order #, I will check and send you your tracking info.
```

---
## \#389 Posted by: nw-esk8 Posted at: 2017-12-08T21:42:10.850Z Reads: 345

```
I was never emailed anything after the order was placed... I will have to check when I get home to check to see if the order # was on the order confirmation screen, but the corresponding paypal confirmation was sent to my email at Sat, Aug 26, 2017 just before 11:20 AM (from WA state).
```

---
## \#390 Posted by: Wajdi Posted at: 2017-12-08T21:44:33.134Z Reads: 348

```
Got it, I will send you the tracking number by email, I'm working on adding a shipment tracker on the website.
```

---
## \#391 Posted by: Deckoz Posted at: 2017-12-08T23:29:13.880Z Reads: 354

```
Shipped and excited.... Yesssssss
```

---
## \#392 Posted by: Brianr058 Posted at: 2017-12-09T01:28:56.139Z Reads: 358

```
post a pic when you receive it!
```

---
## \#393 Posted by: ElskerShadow Posted at: 2017-12-11T12:53:57.182Z Reads: 353

```
How much have shipped yet ?
```

---
## \#394 Posted by: nw-esk8 Posted at: 2017-12-12T21:16:51.920Z Reads: 355

```
I'll have to defer to Wajdi for the official response, but I don't think any have been physically shipped yet (the label for mine has been created, but it's still in pre-shipment status and _I think_ I have the first order).
```

---
## \#395 Posted by: ElskerShadow Posted at: 2017-12-14T07:55:39.822Z Reads: 344

```
Yeah so no remote for chrismas, fortunately my secret santa spoiled me so I’m willing to wait till january with the carvon V4
```

---
## \#396 Posted by: mmaner Posted at: 2017-12-14T14:06:49.314Z Reads: 333

```
Looks like mine will be delivered monday :).  Really looking forward to this.
```

---
## \#397 Posted by: Deckoz Posted at: 2017-12-14T20:12:49.629Z Reads: 326

```
Same here :)

Edit: actually its gonna be delivered saturday
```

---
## \#398 Posted by: Bensaida Posted at: 2017-12-14T20:19:17.655Z Reads: 335

```
@Wajdi if i bought the remote this saturday, when will it ship?
```

---
## \#399 Posted by: Mikenopolis Posted at: 2017-12-14T20:35:29.099Z Reads: 335

```
Keep us updated. I can't wait to see what the experience is with this remote!
```

---
## \#400 Posted by: longhairedboy Posted at: 2017-12-14T20:40:28.451Z Reads: 349

```
[quote="Wajdi, post:359, topic:24654"]
@Skyv4n Thanks, yes its definitely possible, it already has horn/buzzer digital control built in and WS2812B lights driver. Turn signals and reactive brakes are already added and working :slight_smile: I will post a demo video about it.
[/quote]

unfffgghhegfuuhghghhhhahaah
```

---
## \#401 Posted by: nw-esk8 Posted at: 2017-12-14T21:27:56.003Z Reads: 359

```
Looks like mine will be arriving Saturday as well... Now I just need a board to go w/ it :) (I have all components ready for a beastly MTB setup, but haven't started on it yet... this is/was the final piece).
```

---
## \#402 Posted by: DEEIF Posted at: 2017-12-15T19:58:24.206Z Reads: 351

```
Hey can you link me the website for this
```

---
## \#403 Posted by: BoostedBuilder Posted at: 2017-12-15T20:08:30.945Z Reads: 373

```
http://eboardshop.net
```

---
## \#404 Posted by: DEEIF Posted at: 2017-12-15T20:10:09.678Z Reads: 376

```
Thanks @BoostedBuilder
```

---
## \#405 Posted by: Wajdi Posted at: 2017-12-16T07:14:42.775Z Reads: 385

```
The Photon remote MEGA guide is here! I tried to document every single function of the remote, explaining what each option does, and what values to set it to. I included pictures of all the menus as well. 
I'm still going to expand it further but this should get everyone going. 

http://forum.eboardshop.net/t/photon-remote-mega-guide/37
```

---
## \#406 Posted by: SkaterBoy58 Posted at: 2017-12-16T08:08:04.759Z Reads: 366

```
Wajdi -Thanks for that
Just one query re Reactive effect for leds and turn indicators

Do you need to programme in the pixel no range for right hand side (for indicator) and pixel no range for left hand indicator?
 Cheers
```

---
## \#407 Posted by: Wajdi Posted at: 2017-12-16T08:19:23.977Z Reads: 359

```
Reactive effect is the first mode, it uses the first 3 leds for left, next 4 for brakes, and next 3 for right, total of 10 LEDs. I will add that info to the guide.
```

---
## \#408 Posted by: SkaterBoy58 Posted at: 2017-12-16T08:36:18.816Z Reads: 358

```
Can these nos of leds  be changed to suit the total no of leds on the strip?
```

---
## \#409 Posted by: Deckoz Posted at: 2017-12-16T15:17:35.299Z Reads: 365

```
Nice on the wiki section! I look forward to adding anything I can!
```

---
## \#410 Posted by: Wajdi Posted at: 2017-12-17T21:18:02.375Z Reads: 381

```
Hey guys,
I have been having mixed results using the following nrf modules, they perform well on bench test but once in the streets they have been reported to cause dropouts. I ordered a batch of a better performing modules that are shielded, and I will keep you updated about it’s performance.

Bad modules.

<img src="/uploads/db1493/original/3X/2/e/2e9447d12dc1d3d8a51167c30c6cb0cf8ff2d2c2.jpeg" width="225" height="225">

Good modules.
<img src="/uploads/db1493/original/3X/d/9/d938afad25896e8c0b014a2ed2266223a18e1f3e.jpeg" width="300" height="300">

If anyone that received my remote so far is having connection problems, contact me and I will send you v0.2 of the receiver free of charge minus shipping.
```

---
## \#411 Posted by: longhairedboy Posted at: 2017-12-17T21:22:19.550Z Reads: 362

```
Thanks!

I was having random intermittent dropouts on both throttle and telemetry. 

So far though i'm really impressed with the basics. The stick feels good. The grip will be better once its got some kind of coating on it.
```

---
## \#412 Posted by: Ixf Posted at: 2017-12-18T04:23:52.833Z Reads: 364

```
Love it! can't wait for to get my hands on one!
```

---
## \#413 Posted by: Wajdi Posted at: 2017-12-18T05:24:05.541Z Reads: 379

```
I will add that in next update.
Here is a preview of the Photon updater currently a work in progress.

<img src="/uploads/db1493/original/3X/f/3/f322b655b23f59d3e175e4118f40b379bd2828ef.PNG" width="614" height="308">

Auto update fetcher and flash programmer in one.
```

---
## \#414 Posted by: ElskerShadow Posted at: 2017-12-18T08:33:49.143Z Reads: 366

```
@longhairedboy why areyou allways the first to get the fancy new things ? Hahah
```

---
## \#415 Posted by: Skyv4n Posted at: 2017-12-18T10:33:21.627Z Reads: 360

```
Can you develop please ?
```

---
## \#416 Posted by: longhairedboy Posted at: 2017-12-18T12:50:54.477Z Reads: 370

```
@ElskerShadow  because i volunteer to pay full price for partially developed products so i can give my feedback and influence development. 

@Skyv4n right now i don't trust it beyond experimentation, the dropouts are intermittent but frequent. But the new radios will likely resolve that problem. 

Its a new product, the bugs will be shaken out. And when they do this remote is going to kill it. 

Once allthe features are working correctly and reliably and this thing has some kind of comfort grip coating on it i'm done. I'll have my dream remote. 

Once we get there though we'll need to do a lot of throw testing. The new Maytech remotes are indestructible unless you grind them or slide on them somehow. This needs to be close to that in durability. I don't expect miracles because it uses more sensitive components and has a multiple axis thumb stick which requires more consideration but i think it can come close.
```

---
## \#417 Posted by: Deckoz Posted at: 2017-12-18T14:58:20.526Z Reads: 353

```
Damn..that's pretty sheisty about the drop outs... Mine got delayed delivery til today. So I guess I'll see if I have the same issue... :(
```

---
## \#418 Posted by: Wajdi Posted at: 2017-12-18T16:05:13.327Z Reads: 345

```
Don’t worry, connectivity issue is really an easy fix, most of those nrf modules have bad batches mixed in. 
Thankfully it’s a problem caused by the modules manufacturer and not my design, so no big redesign or delays. The shielded modules should provide a far superior connection, with virtually no dropouts, it does also have an IPX antenna which amplifies the signal even further.
```

---
## \#419 Posted by: longhairedboy Posted at: 2017-12-18T17:27:26.540Z Reads: 344

```
all of that is music to my ears :slight_smile:
```

---
## \#420 Posted by: Deckoz Posted at: 2017-12-18T21:59:46.911Z Reads: 360

```
@longhairedboy do you have the Receiver pinout? Mine came with a 6pin JST for older 4.6-4.9 hardware... Not a 7pin like on the focboxes/4.10-4.12/vesc6's

edit nvm... goes into the bottom 6 pins... ..
```

---
## \#421 Posted by: Deckoz Posted at: 2017-12-18T22:44:55.146Z Reads: 369

```
Just rode about 4 miles with it. Looking good so far <img src="/uploads/db1493/original/3X/1/c/1c4720e49dff0638eb6a44f2d31c0a8687ac259e.jpg" width="374" height="499">
```

---
## \#422 Posted by: Wajdi Posted at: 2017-12-18T22:55:12.958Z Reads: 357

```
Awesome! it feels really good seeing happy customers :slight_smile:
```

---
## \#423 Posted by: Deckoz Posted at: 2017-12-18T22:56:28.903Z Reads: 355

```
Cruise control 😍
```

---
## \#424 Posted by: Mattmccrary8 Posted at: 2017-12-18T23:54:42.728Z Reads: 361

```
How was it? Mines coming soon! We want details mate
```

---
## \#425 Posted by: Deckoz Posted at: 2017-12-19T00:25:57.837Z Reads: 386

```
Dude I'm in love. So things of note cause I just rode again. Pistol grip doesn't work. Let me explain

Nano remote what I'm used to. Pistol grip
<img src="/uploads/db1493/original/3X/4/b/4b240cf84318587a1fbd02cf9087e3d6c884f61d.jpg" width="374" height="499">

Pistol grip on the Photon. Feels really weird because it's wide
<img src="/uploads/db1493/original/3X/7/9/792da5d226ca568e38a266c289bf0eec60565205.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/8/e/8efd27315b8ab300b2cdfeaf781dc841cd6771e2.jpg" width="374" height="499">

Modified pistol with index on the cruise. Feels amazing
<img src="/uploads/db1493/original/3X/d/9/d936569ea97af1e4bcb792f68eea07e18434c4a2.jpg" width="374" height="499"><img src="/uploads/db1493/original/3X/9/0/90190270c5e0e1f37988b4d637b01e0ffafe6dbf.jpg" width="374" height="499">

The last pics feel great with a modified pistol grip. Plus index on the cruise control is just amazing. Being able to tap it and hold speed up and DOWN hills is a nice perk. 

The update rate of the speedo seems to be quite often... Taking a wild guess here but 8x a second(@Wajdi to confirm) is what it looks like, so pretty good. While riding it updates and is the perfect size for a 'glance' like driving a car.

The Y axis spring feels to be tighter then X, which is a good thing as it helps you forget about the side to side movement while using the joystick as the throttle.

I'm over all really impressed with it. The menus are nicely organized, all configurable values have ranges that they should with the exception of drive ratio for calculating distance limited to tenths. Ie I have 3:1 drive ratio which would be .33, I can only set .30. however @wajdi is addressing hundredths in the next firmware update. All other values seem to be configurable as would be needed.

There's also onboard throttle limiting. Which seems to work good. 

On the VESC, it feels best if you set the nunchuck tab deadband to 0, as having deadband on the remote configurable let's you get a better feel without doubling up on deadband.


Anyway....I'll share more as I ride...
```

---
## \#426 Posted by: scepterr Posted at: 2017-12-21T08:10:48.894Z Reads: 350

```
Try this out, gives satinny soft feel, apply coats to desired plushness 
https://www.electric-skateboard.builders/t/universal-advanced-vesc-remote-control-custom-design/24654/326
```

---
## \#427 Posted by: ElskerShadow Posted at: 2017-12-21T08:44:08.742Z Reads: 369

```
The best profuct for that is optimus !!
Gets any PLA smooth or mat or shiny ! 
https://www.filament-abs.fr/produit/produit-de-lissage-optimus/
```

---
## \#428 Posted by: Deckoz Posted at: 2017-12-22T16:31:48.366Z Reads: 365

```
<img src="/uploads/db1493/original/3X/5/c/5c5961f7c8db56bf7027e28cffd62cb20952b1bf.jpg" width="375" height="500">
```

---
## \#429 Posted by: ElskerShadow Posted at: 2017-12-22T19:53:15.681Z Reads: 356

```
@Wajdi how many have shipped yet ?
```

---
## \#430 Posted by: longhairedboy Posted at: 2017-12-22T20:04:44.658Z Reads: 362

```
i breifly tested mine long enough to know i need the new receiver. @Wajdi is  sending me one soon though. I'm pretty pumped about this remote. I'm hoping to be able to use it all next year in my builds.

https://www.instagram.com/p/BdBGJbAFx2r/?taken-by=longhairedboy
```

---
## \#431 Posted by: SuperBen Posted at: 2017-12-22T22:10:48.633Z Reads: 351

```
I love the design of this remote, been silently following for quite a while. Will be using this for the 2018 build I'm slowly pulling together
```

---
## \#432 Posted by: Brianr058 Posted at: 2017-12-27T03:28:22.695Z Reads: 345

```
Very nice, I'll patiently wait until all the bugs are worked out and readily available! Please keep us posted!
```

---
## \#433 Posted by: Deckoz Posted at: 2017-12-27T03:33:35.828Z Reads: 357

```
@longhairedboy set the sensitivity to 10.0 I believe it is a bug with the ramping code. The things that feel like "drop outs" are really just me trying to reengage throttle while at speed and the motors seem to studder/cog like a desync.  But it's from the throttle sensitivity trying to ramp the throttle smoothly upto where your thumb is in too small of percentages while already moving... basically making the motor act like a stepper.

10.0 is direct input with no ramping. Rides completely fine. After that. If you need sensitivity ramping do it with the throttle curves like we always have.. I believe @Wajdi is going to be removing the sensitivity and setting it back to default as direct input(10.0) since throttle curves are built in to acks bldc tool and the vesc tool..

Once the UI bugs with text and a couple settings are fixed, sensitivity set to be direct input(10.0 instead of 1.0) and deadband adjustable in the menu vs during calibration only. 

Functionally the remote is where it should be and rides how any other thumb remote I've tried does with the benefits of a screen..
```

---
## \#434 Posted by: longhairedboy Posted at: 2017-12-27T12:11:40.467Z Reads: 336

```
thanks for the info and background! We're not using Ack's firmware yet, and there's plenty of hardware out there that isn't. It's still too easy to fuck shit up in there in my opinion, so we're waiting for just a little more maturity. Hopefully this ramping code bug will be fixed and not just eliminated along with the functionality it lives in. Additional means of fine tuning the ride experience are necessary and should be considered worth the extra work. In the mean time, that seems like a solid workaround and i'm going to try it.
```

---
## \#435 Posted by: Deckoz Posted at: 2017-12-27T14:07:58.000Z Reads: 337

```
@longhairedboy Oh if your not using ack code or vesc tool with throttle ramping..then direct input is what your used to.. set that shit to 10.0 and ride son :)

If you need to dumb it down for people you can still set the throttle % on the remote to limit speed...and then amps in the vesc for acceleration just leave the sensitivity on the remote at 10 to remove the drop out/stutter feel.
```

---
## \#436 Posted by: longhairedboy Posted at: 2017-12-27T14:22:56.981Z Reads: 331

```
We're basically in love with the new maytech remotes because of the way they seem to process the PPM, both in slow and fast modes. Its much better than the Steezes. I'm hoping to emulate some sort of middle ground specifically for a given rider with these photons.
```

---
## \#437 Posted by: GrecoMan Posted at: 2017-12-27T14:30:34.046Z Reads: 330

```
I love the new maytech remotes.

I really love this remote. I just can’t justify the price tag.  Any chance of these decreasing in price sometime soon? i’d love to pick one up.
```

---
## \#438 Posted by: Deckoz Posted at: 2017-12-27T14:39:09.843Z Reads: 325

```
Just remember the fast modes and slow modes limit the ppm swing/endpoints...which is effectively what limiting the throttle % will do. As it remaps the curve of the throttle over the throw of the stick... 

The maytech and nano remote in slow mode are about 70% ppm throw. If you set the remote to have 70% throttle. It will map that 70% across the stick like the other remotes and feel basically identical.
```

---
## \#439 Posted by: longhairedboy Posted at: 2017-12-27T14:58:48.814Z Reads: 330

```
in BLDC Tool the ppm meter says slow mode is at 80% on the new maytech's. I have yet to try an Nano X. 

Are they the same internally?
```

---
## \#440 Posted by: Deckoz Posted at: 2017-12-27T15:15:53.998Z Reads: 363

```
Yea they are basically the same internally. Some of the old ones are 70% some are 80%. But yea...try limiting throttle to .70 or .80, it feels identical to "slow mode" depending on which generation remote you previously had. The great news is you can fine tune it even further then just 80 or 100... You have the full range of 20-100 for options :)

:slight_smile:
 
<img src="/uploads/db1493/original/3X/3/b/3b1b9cdcf922aa1c0c59c6a33282921778651611.jpg" width="374" height="499">
```

---
## \#441 Posted by: Wajdi Posted at: 2017-12-28T00:21:02.906Z Reads: 358

```
Great news everyone! new modules are in! I had several packages being delayed because of the Holidays, but we should pick up the speed now. 

I have started assembling the new receivers using the new nrf modules and its AMAZING! the range and signal quality is outstanding! I have ditched all the old modules because most of them were faulty and they caused me all this delay!

Check this out:
<img src="/uploads/db1493/original/3X/f/f/ff47daff142d099431c5c0408425bb5e78334958.jpg" width="380" height="158">
```

---
## \#442 Posted by: ATLesk8 Posted at: 2017-12-28T01:32:22.232Z Reads: 345

```
Just out of curiosity if I were to order today what would be the estimated lead time?
```

---
## \#443 Posted by: Wajdi Posted at: 2017-12-28T03:09:40.635Z Reads: 336

```
As of right now, it would be around 2 weeks. Current pending pre-orders will be shipped out right after new year's day.
```

---
## \#444 Posted by: Wajdi Posted at: 2017-12-28T05:47:01.052Z Reads: 340

```
What's your opinion about the piezo buzzer? I'm working on the new batch and I don't know if its worth keeping. Due to its size, its really hard to hear it on noisy environments.
```

---
## \#445 Posted by: mishrasubhransu Posted at: 2017-12-28T15:48:49.018Z Reads: 334

```
are you going to put antenna on both receiver and transmitter. That should make it bullet proof.
```

---
## \#446 Posted by: Deckoz Posted at: 2017-12-28T16:12:41.947Z Reads: 334

```
@wajdi Keep the peizo. It's the only way I can tell I held the power button long enough to turn it off haha...
```

---
## \#447 Posted by: nw-esk8 Posted at: 2017-12-28T22:36:03.118Z Reads: 333

```
Hey-

I haven't finished my board (probably at least few weeks out after realistically accounting for other stuff that is on my radar), but is the receiver that I was sent with my order going to kill me?  That would be disappointing :sweat:...
```

---
## \#448 Posted by: Wajdi Posted at: 2017-12-28T23:24:05.776Z Reads: 336

```
@nw-esk8 I hope not :smile: If you experience dropouts send me a message and I will send you the new version.

@mishrasubhransu Yes, both remote and receiver will have antennas. I'm having an astonishing range with the new receiver modules.

@Deckoz Ok its here to stay then :slight_smile:
```

---
## \#449 Posted by: nw-esk8 Posted at: 2017-12-28T23:56:04.980Z Reads: 331

```
Any thoughts on pro-actively sending replacements to those with a decent likelihood of having a faulty module?

...or do you think the defect rate is low enough not to be concerned?  

I know the remote is an ongoing work in progress in areas, but to be honest, I'm not feeling super happy about hearing that these were sent out with (potentially) defective receivers before being able to have even hooked mine up... and correct me if I'm wrong (I've only skimmed recent posts so I could be off here), but it sounds like this may have been more or less a known issue before they were shipped.  If that's the case, considering reliable transmission is kind of the minimum requirement for any remote, I'm not sure I agree with the onus being on the consumer here, but I'm interested in your thoughts (and/or any other details I may have missed).
```

---
## \#450 Posted by: Wajdi Posted at: 2017-12-29T00:09:20.347Z Reads: 341

```
There are faulty nrf modules mixed in the batch I ordered, and even tho they performed well on my bench tests, they are just bad units. I didn't notice the issue until I already sent out a handful of orders, but luckily the problem was caught before a larger amount was shipped. That's why I halted the project and ordered the new modules. I was very disappointed and frustrated, but sometimes bad things happens, and we just need to make it better.

If you experience problems, just hit me up and I will send you the new replacement. This project is still under heavy development and is by no means complete.
```

---
## \#451 Posted by: jamiex Posted at: 2017-12-29T00:53:13.134Z Reads: 357

```
This looks awesome!
Once they are tested I'll be buying one!
```

---
## \#452 Posted by: Wajdi Posted at: 2018-01-04T03:01:03.178Z Reads: 363

```
I have been working on assembling pending orders, and at the same time fixing all the reported bugs. 
I did a major software improvements:

* Optimized speed, now around 310% faster
* Faster refresh rate on the display
*  Faster speedometer update rate
*  Faster stats reading.
* Improved UI with bigger numbers, clearer and cleaner
* Improved menu fonts
* Added hundreds support to ratio setting
* Fixed padding issue for larger wheel size
* Fixed total distance calculation
* Fixed cell count calculation
* Added signal power control setting

Here is a quick comparison video, notice how boot-up and accessing menus is now faster.

https://www.youtube.com/watch?v=pSNllbi8z08
```

---
## \#453 Posted by: Deckoz Posted at: 2018-01-04T03:11:21.409Z Reads: 345

```
So

Where do I download :)
```

---
## \#454 Posted by: Wajdi Posted at: 2018-01-04T03:16:50.009Z Reads: 343

```
Download coming soon, I'm still doing final touches on the updater tool.
```

---
## \#455 Posted by: E1Allen Posted at: 2018-01-04T07:18:16.961Z Reads: 340

```
On my list of 15th payday purchases👍👍👍
```

---
## \#456 Posted by: Mattmccrary8 Posted at: 2018-01-04T14:07:05.871Z Reads: 332

```
So sick! Can’t wait for this bad boy 🤘🏼🤘🏼🤙🏼🤙🏼🤙🏼
```

---
## \#457 Posted by: skelstar Posted at: 2018-01-04T23:08:23.789Z Reads: 342

```
You're using the u8g2 library right? What font do you use for the main figures (ie the "32" in the picture). I struggle with finding fonts I like.

.... if you don't mind me asking.
```

---
## \#458 Posted by: Wajdi Posted at: 2018-01-05T01:02:14.146Z Reads: 339

```
Font name is akashi. I also do spend a lot of time fiddling with fonts, probably way more than necessary :slight_smile: It needs to satisfy my aesthetic standards :grin:
```

---
## \#459 Posted by: skelstar Posted at: 2018-01-05T02:22:05.572Z Reads: 345

```
Ahhh... you created your own from a TTF file? I have yet to do that (I'm lazy).

(http://tenbytwenty.com/?xxxx_posts=akashi)
```

---
## \#460 Posted by: NickB Posted at: 2018-01-08T14:12:25.598Z Reads: 346

```
Hi 

how water proof is the remote

I have an application calling for a waterproof remote.


thanks Nick
```

---
## \#461 Posted by: longhairedboy Posted at: 2018-01-08T14:15:58.087Z Reads: 339

```
when can we expect replacement receivers? I have an older one, and the range is buggy even with the adjustments that were suggested.
```

---
## \#462 Posted by: Deckoz Posted at: 2018-01-08T14:42:45.914Z Reads: 332

```
[quote="longhairedboy, post:461, topic:24654"]
when can we expect replacement receivers?
[/quote]

This and the update!!! :)
```

---
## \#463 Posted by: Deckoz Posted at: 2018-01-08T14:43:31.360Z Reads: 322

```
It's not waterproof.
```

---
## \#464 Posted by: longhairedboy Posted at: 2018-01-08T14:51:42.217Z Reads: 326

```
it may not even be rain proof.
```

---
## \#465 Posted by: Deckoz Posted at: 2018-01-08T14:57:28.100Z Reads: 336

```
I corrosionX my internals except the LCD, I Conformal coated. 

So mines rain proof now. But definitely not water proof
```

---
## \#466 Posted by: mmaner Posted at: 2018-01-09T18:10:56.718Z Reads: 332

```
What's the ETA on the replacement receivers?  Im dieing to use this remote :slight_smile:
```

---
## \#467 Posted by: Wajdi Posted at: 2018-01-10T04:11:17.069Z Reads: 327

```
I shipped several orders today, and will be shipping some more tomorrow. Receiver replacement as well as the updater will be done by Friday if not earlier.
```

---
## \#468 Posted by: mmaner Posted at: 2018-01-10T04:20:48.398Z Reads: 326

```
Awesome.  I'm happy tonoay for shipping at least, om me your PayPal address and the cost. Thanks brother.
```

---
## \#469 Posted by: Wajdi Posted at: 2018-01-10T04:35:50.506Z Reads: 324

```
You are welcome. Shipping is free to the US for the replacements.:+1:
```

---
## \#470 Posted by: ElskerShadow Posted at: 2018-01-10T09:59:29.497Z Reads: 326

```
Recieved my tracking number today ! 
So the remote you send was with old module ?
```

---
## \#471 Posted by: Wajdi Posted at: 2018-01-10T14:22:59.424Z Reads: 326

```
No, everyone is getting the latest version, yours included.
```

---
## \#472 Posted by: longhairedboy Posted at: 2018-01-12T15:04:21.149Z Reads: 340

```
Just wanted to mention that i tried all of the suggestions i got for getting the old receiver to play nice until the new ones came. I was still getting interference and drop out like behavior. 

However, this time i was running FOC. In BLDC mode i would get dropouts or whatever on occasion, but nothing serious. In FOC mode, something else is happening i think because not only did i get that interference, i also got some kind of weird signal spike and then a mostly-dead VESC-X that can no longer detect sensors in a known good motor. 

it may be nothing but an old abused ESC finally kicking it but its also possible that it choked on something the receiver sent it then puked and died on its way to deliver the current pulses.
```

---
## \#473 Posted by: Deckoz Posted at: 2018-01-12T17:22:30.110Z Reads: 335

```
I only run sensored FOC and I've been. Fine on my focboxes


I had a sensor die on one of my motors before the photon... I tested other motors on the same focbox then replaced the sensor.. as the sensor board went bad(specifically one hall sensor so two of three and the temp we're reading)

Specifically I've been running ack 2.54 or 3.100 if that matters to you.
```

---
## \#474 Posted by: Wajdi Posted at: 2018-01-12T17:23:28.165Z Reads: 337

```
Receiver works just like any other remote, it only sends commands to Vesc to control the motor, and they are the same for BLDC as well as FOC. If you have problems with FOC mode it’s definitelty Vesc related.
```

---
## \#475 Posted by: Deckoz Posted at: 2018-01-19T21:19:59.206Z Reads: 322

```
@Wajdi when should we be getting the firmware update and the updated receiver?

And when will the case files be available...I've been waiting as I'd like to Mill the case out of POM or aluminum.
```

---
## \#476 Posted by: ElskerShadow Posted at: 2018-01-19T21:22:23.129Z Reads: 324

```
My remote just passed thru customs wether i get it this week end or monday. I’m so Excited it’s a shame my battery is not working anymore still have to resole this issue first before using it
```

---
## \#477 Posted by: SkaterBoy58 Posted at: 2018-01-21T02:53:22.536Z Reads: 329

```
Wadji
How do you activate variuos reactive effects for leds.I cant see it on lights menu .

Also -will the firmware update contain settable pixel no for left indicator, brake and right indicator leds?

Cheers
```

---
## \#478 Posted by: Deckoz Posted at: 2018-01-21T12:29:16.253Z Reads: 312

```
Use the right bottom button besides power.click it
```

---
## \#479 Posted by: SkaterBoy58 Posted at: 2018-01-21T12:49:03.230Z Reads: 310

```
nothing on right button under menu/lights?
```

---
## \#480 Posted by: Deckoz Posted at: 2018-01-21T13:49:58.532Z Reads: 301

```
No just click it while your out of the menu... riding... It cycles light modes
```

---
## \#481 Posted by: SkaterBoy58 Posted at: 2018-01-21T14:46:00.889Z Reads: 301

```
Thanks for that
Is there a list of the light modes anywhere?
Cheers
```

---
## \#482 Posted by: Deckoz Posted at: 2018-01-21T14:53:02.975Z Reads: 298

```
Have you checked out the forum.eboardshop.net

I know there's a visual run through of them in one of his YouTube videos..
```

---
## \#483 Posted by: Wajdi Posted at: 2018-01-21T22:47:50.249Z Reads: 303

```
Yes, as @Deckoz mentioned, the right button is dedicated for lightning, you cycle through the different effects by clicking it once. A long press will turn it off. 
Light effects are saved on power off.
The new receivers will have two ports for LEDs, one for front lights, and one for back lights. Each one needs a separate 10 LED strip if you want front and back lightning.
As for now, the number of LEDs used for signals and brake effect is set to 10, it is not adjustable for the moment. I'm also working on a video tutorial and finishing the software updater.
```

---
## \#484 Posted by: caustin Posted at: 2018-01-21T23:21:15.234Z Reads: 302

```
I know this cane up earlier in the thread, but does anyone have a link to the simplest best all-in-one LED strip for dummies for this, just want for a base level proof of concept lol.
```

---
## \#485 Posted by: Wajdi Posted at: 2018-01-21T23:32:16.751Z Reads: 304

```
Any WS2812B RGB LED would do. I recommend WS2812B based one, with density of 60LEDs/ 1M.
Here is an example https://www.ebay.com/itm/WS2812B-5050-RGB-LED-Strip-30-60-144-LEDs-M-ws2812-IC-Individual-Addressable-5V/262452005540?hash=item3d1b5bcaa4:m:mkMwXOyKYoE3TxVrA-ee05w
```

---
## \#486 Posted by: SkaterBoy58 Posted at: 2018-01-21T23:35:47.907Z Reads: 306

```
Wadji - Do you have a wiring diagram of new receiver?
```

---
## \#487 Posted by: Wajdi Posted at: 2018-01-21T23:41:03.920Z Reads: 316

```
Im working on it, I will post it today or tomorrow hopefully.
```

---
## \#488 Posted by: ElskerShadow Posted at: 2018-01-22T14:13:32.107Z Reads: 336

```
![image|375x500](upload://isJrAKLmPi3fD4mGbidZp7gBTPk.jpg)

Recieved the remote this morning ! I noticed there was no cables to connect to the VESC in the BOX. Dunno where to find one. 129 $ for an amazing remote but no cable to use it :stuck_out_tongue:
```

---
## \#489 Posted by: Deckoz Posted at: 2018-01-22T14:22:02.180Z Reads: 330

```
I'm sure @Wajdi did it by accident

If your in a hurry to use it I can't remember if it's 2.0mm or 2.54mm

2.0mm 6pin
https://www.ebay.com/i/262895398646

2.54mm 6pin
https://www.ebay.com/itm/10-SETS-JST-XH-2-54MM-6-Pin-Female-Double-Connector-with-Flat-Cable-200MM-USA/262894297299?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D20160908110712%26meid%3De86bc99f8a874d37b922da546ffb69c7%26pid%3D100677%26rk%3D6%26rkt%3D30%26sd%3D262895398646&_trksid=p2385738.c100677.m4598
```

---
## \#490 Posted by: ElskerShadow Posted at: 2018-01-22T14:26:48.376Z Reads: 307

```
I'm not in a hurry it's raining non stop since 1 month in Paris so I do a lot of work on all my boards but can't ride em :stuck_out_tongue:
It's USA link so long shipping, will try to find a EU seller or if @Wajdi can send me a little cable il a letter it could be great
```

---
## \#491 Posted by: Wajdi Posted at: 2018-01-22T14:39:22.290Z Reads: 300

```
Oups, Im sorry man, I don't know how did that happen.:sweat: I always double check, but I guess I somehow missed it. I will send you one soon.
```

---
## \#492 Posted by: ElskerShadow Posted at: 2018-01-22T21:21:09.959Z Reads: 295

```
I don’t know if i’m missing something but i can’t turn on the remote. When i recieved it it wouldn’t turn on ( battery was dead I suppose )  and i’ve put it on charge the whole afternoon. After the charge the remote turned on once, i haven’t touched anything just went to see the menu etc... and since then it won’t turn on. I press button A as stated in the guide on the photon forum but nothing happen. I will put on charge the remote again see what happend... 
when i plug in the remote to the computer i can see «  photon remote  plugged in » but i still can’t turn it on
```

---
## \#493 Posted by: Deckoz Posted at: 2018-01-22T22:31:00.613Z Reads: 303

```
@ElskerShadow 

rrr hey... so take the two screws out..and the screws off the pcb... and unplug the lipo...and replug it in..

I bet the battery went dead and soft switch got stuck on and the chip(MCU) got stuck in retard mode(it happens called brown outs).

make sure you turn it off :)

its happened to me...i accidentally left mine on.. was really confused.

@Wajdi
```

---
## \#494 Posted by: Wajdi Posted at: 2018-01-23T14:21:42.711Z Reads: 300

```
Hi,
As @Deckoz  said this usually happens when the battery is discharged, MCU gets stuck in sleep mode sometimes, to solve this just unplug the battery and plug it back again. I'm releasing a software update that should prevent this from happening.
```

---
## \#495 Posted by: ElskerShadow Posted at: 2018-01-23T15:23:51.590Z Reads: 301

```
Yeah i did the plug unplug and it worked. I was sure it was nothing bad since it was booting the remote. 
I only had a little chance to test it but it was indoor because everything is wet. And let me tell you that you developped one hell of a remote... 
my only complain for now is that the buttons are hard to press Even without gloves ( i have big hands )
```

---
## \#496 Posted by: Mattmccrary8 Posted at: 2018-01-25T15:33:22.017Z Reads: 297

```
How do I get the receiver in binding mode. Got everything set up except for that. I’m so confused
```

---
## \#497 Posted by: Deckoz Posted at: 2018-01-26T03:54:42.206Z Reads: 328

```
Got the new receiver an Lookiee it came with a whip
![1516938606226-1186285797|375x500](upload://2rZ0vRuAynublmbf2PfUdU1SEIY.jpg)

Wish I had the updated firmware :frowning: @Wajdi 

[quote="Mattmccrary8, post:496, topic:24654"]
I’m so confused
[/quote]

Use tweezers. Short this connection before you power it on. 

![1516938776850-905154955|375x500](upload://mKgVei3kWX4HCn3kaVgmTDRzAi4.jpg)
```

---
## \#498 Posted by: lrdesigns Posted at: 2018-01-26T05:19:53.499Z Reads: 319

```
Very happy :smile: to see this has a replaceable antenna, and shielded transceiver. Should provide a very reliable connection. Also the antenna can be placed outside of a metal or carbon enclosure. :money_mouth_face: 

@Wajdi , just out of curiosity. what chipset is the transceiver? 

![image|505x488](upload://1Dx5GyygEnCYfuRo8Qd2gWQEH3S.jpg)
```

---
## \#499 Posted by: ElskerShadow Posted at: 2018-01-26T07:56:03.638Z Reads: 328

```
@Wajdi told me by MP that apparently that the « bind » pins are not the good ones, it’s the soldered ones ![image|326x500](upload://it6HJBZBcxhrqTZBWKszWsFqKni.jpeg)
```

---
## \#500 Posted by: Wajdi Posted at: 2018-01-26T15:19:43.234Z Reads: 307

```
@lrdesigns  Thanks! It is indeed very reliable, its an nrf24 still.
@Mattmccrary8 @Deckoz The new binding port is the long pad with an opening underneath the enclosure. The software update is 99% done!
```

---
## \#501 Posted by: Deckoz Posted at: 2018-01-26T15:21:03.206Z Reads: 311

```
Ah...hmm I've been deceived by the silk screen "bind"

Thanks :) 

I assume I cannot run the new receiver without the update?
```

---
## \#502 Posted by: Wajdi Posted at: 2018-01-26T15:21:44.348Z Reads: 303

```
Yes sorry about that, the port was later changed in software :laughing:

I don't think it will bind without an update because the packets have been changed, the new receiver and new software now supports up to 4 receivers, with one master and 3 slaves, I also fixed the total distance counter, and tweaked other things. 

It should be really just a couple hours before I release it.
```

---
## \#503 Posted by: Mattmccrary8 Posted at: 2018-01-26T17:54:32.035Z Reads: 309

```
[quote="Deckoz, post:501, topic:24654"]
Thanks
[/quote]

Ok so when will I be able to get this bad boy hooked up
```

---
## \#504 Posted by: Deckoz Posted at: 2018-01-26T17:57:21.757Z Reads: 321

```
Now... Do the same thing I said but short the two solder pads on the bottom with tweezers instead of the ones I pointed out

![15169893978801309476203|375x500](upload://tO5WSv62vFFehV8w7y8X1ri1lZw.jpg)
```

---
## \#505 Posted by: Mattmccrary8 Posted at: 2018-01-26T17:59:57.046Z Reads: 305

```
How do I short them, that’s my question. Can I do it with a small screw driver
```

---
## \#506 Posted by: Mattmccrary8 Posted at: 2018-01-26T18:00:30.324Z Reads: 300

```
Mine doesn’t have any openings on the bottom like yours
```

---
## \#507 Posted by: Deckoz Posted at: 2018-01-26T18:00:33.891Z Reads: 303

```
Tweezers :)
```

---
## \#508 Posted by: Deckoz Posted at: 2018-01-26T18:01:14.249Z Reads: 290

```
Pop the top off and hit the two solder pads in the picture @ElskerShadow circled then :)
```

---
## \#509 Posted by: Mattmccrary8 Posted at: 2018-01-26T18:11:24.870Z Reads: 293

```
Just did it. Ok so my last problem is getting my dual motors to work. Is there another setting I need to change so the dual works?
```

---
## \#510 Posted by: Deckoz Posted at: 2018-01-26T18:27:51.691Z Reads: 294

```
Canbus 

Set master to ID 0 with multiple esc over can checked

Set slave to iD of 1 with send status over can checked
```

---
## \#511 Posted by: Mattmccrary8 Posted at: 2018-01-26T18:36:13.176Z Reads: 284

```
Did all of that and still nothing with the slave motor. I’m so confused
```

---
## \#512 Posted by: Deckoz Posted at: 2018-01-26T18:58:58.105Z Reads: 283

```
You have control mode enabled on the slave? (Current no reverse w/ brakes)
```

---
## \#513 Posted by: Mattmccrary8 Posted at: 2018-01-26T19:56:32.549Z Reads: 274

```
Yes I do. Should I not?
```

---
## \#514 Posted by: Deckoz Posted at: 2018-01-26T20:14:13.112Z Reads: 283

```
Can you connect usb to one and can fwd to the other?

Ie plug usb into master and type 1 and check can fwd? And get a successful connection?
```

---
## \#515 Posted by: Mattmccrary8 Posted at: 2018-01-26T21:04:51.317Z Reads: 289

```
Ok I got it all figured out. I didn’t add multiple esc on the nunchuck tab. Got everything working.

Only downfall is, whenever give it throttle it cuts off after 5 seconds. Hopefully the update fixes this today. Had no brakes at 20mph was bad
```

---
## \#516 Posted by: Wajdi Posted at: 2018-01-26T21:51:24.928Z Reads: 285

```
Glad you got it sorted out.
About the cutout, this shouldn't be happening, what value do you have on "SIG", under control settings?
```

---
## \#517 Posted by: scepterr Posted at: 2018-01-27T05:49:45.048Z Reads: 290

```
Damn I think I've run out of reasons not to order one 😋
```

---
## \#518 Posted by: SkaterBoy58 Posted at: 2018-01-27T13:42:04.423Z Reads: 337

```
Hi Guys - Having a bit of trouble getting photon to connect to vesc - any clues

Photon  remote binds OK with receiver - remote light flashes green showing connection
steady green light in receiver
VESC is focbox with 3.34 FW
Have set App to UART with 115200 baud rate
Photon remote does not show any vesc data and shows 255.2 in FW rectangle at top of remote

Photon receiver is V0.1

Thanks
![IMG_3268|666x500](upload://kw2tbaWB5a94hXmsKiUDuxLrdxS.JPG)![IMG_3267|666x500](upload://h9ZeykYa4lkpOEsB1MFGcYYNOsD.JPG)![IMG_3271|666x500](upload://mTLr3QLxPMFRd4Z9NCgWBoL7cyW.JPG)![IMG_3266|666x500](upload://cPWU77aZBhLvfHycWWT6dVRW8v1.JPG)
```

---
## \#519 Posted by: Mattmccrary8 Posted at: 2018-01-27T16:21:07.147Z Reads: 309

```
Has anyone figured out how to eliminate the cut outs. My remote won’t stay connected longer than 5 seconds at a time. I’ve wasted 5 hours on this thing
```

---
## \#520 Posted by: mmaner Posted at: 2018-01-27T16:40:18.830Z Reads: 305

```
You need the new receiver, talk to @Wajdi
```

---
## \#521 Posted by: Wajdi Posted at: 2018-01-27T16:58:03.655Z Reads: 302

```
@Mattmccrary8 Seems like an odd issue, can you check if there is any fault on the VESC? 
@mmaner He already has the new receiver, which has an outstanding range, I suspect there is something else causing him problems.
```

---
## \#522 Posted by: Wajdi Posted at: 2018-01-27T16:58:51.141Z Reads: 301

```
@SkaterBoy58 The latest vesc firmware is not supported yet, but its an easy fix, I will PM you a modified firmware to solve the problem.
```

---
## \#523 Posted by: mmaner Posted at: 2018-01-27T17:02:33.847Z Reads: 288

```
I haven't tried my new RX yet, but in the bench I walked 40 feet away and it still work Ed perfectly with zero lag. That's with the enclosure mounted.
```

---
## \#524 Posted by: Mattmccrary8 Posted at: 2018-01-27T21:19:43.706Z Reads: 287

```
I’m send big you a video but I have no idea what’s going on
```

---
## \#525 Posted by: Deckoz Posted at: 2018-01-27T22:20:35.683Z Reads: 290

```
Me too as I'm on ack 3.100 across everything instead of 2.54. Now. :p

(Hopefully the firmware update does this?)
```

---
## \#526 Posted by: SkaterBoy58 Posted at: 2018-01-28T01:34:06.139Z Reads: 293

```
Wadji   
If I put +12v external supply on +5V pin -
wont that put this 12V supply back on VESC 5V circuitry with not good consequences?
```

---
## \#527 Posted by: Wajdi Posted at: 2018-01-28T01:35:46.878Z Reads: 294

```
You can only use +12v external supply on the receiver +5v pin if its disconnected from the vesc.
To disconnect it from the vesc you can unpin it from the UART cable.

@Deckoz I think Ack firmware should work fine, but I did not test it tho.
```

---
## \#528 Posted by: StickSk8s Posted at: 2018-01-28T02:47:55.860Z Reads: 290

```
So how would I get one of these once finalized? New to the forum and e boarding in general. The work you've done on this is amazing
```

---
## \#529 Posted by: Wajdi Posted at: 2018-01-28T02:52:59.884Z Reads: 290

```
You should be able to order one on http://eboardshop.net/product/advanced-electric-skateboard-remote/
```

---
## \#530 Posted by: StickSk8s Posted at: 2018-01-28T03:00:31.054Z Reads: 277

```
Thanks alot! The remote looks awesome. Can't wait
```

---
## \#531 Posted by: SkaterBoy58 Posted at: 2018-01-28T03:15:20.925Z Reads: 283

```
Wadji  
maybe a good hint to include in your mega guide re cutting +5V from vesc if using external supply for leds!
```

---
## \#532 Posted by: danggilmore Posted at: 2018-01-30T00:33:12.949Z Reads: 285

```
@Wajdi

hi,

purchased 5 days ago. sent you an e-mail for an estimated ship date and havn't gotten a response. sent another e-mail this morning. 

i would think i would deserve a response after purchasing a 100+ dollar remote.......

thanks.
```

---
## \#533 Posted by: Deckoz Posted at: 2018-01-30T00:44:44.807Z Reads: 272

```
They take about three weeks dude... it'll be ok.
```

---
## \#534 Posted by: danggilmore Posted at: 2018-01-30T00:57:27.910Z Reads: 278

```
i'm not stressin bout lead time. i got plenty of time. i just feel that not responding is kinda lame. when you spend hard earned money, communication is what you deserve. IMO
```

---
## \#535 Posted by: cesargrimmelprez Posted at: 2018-01-31T23:09:30.111Z Reads: 279

```
Imo he's done a shit ton for this community by making a whole new remote. He's constantly working on updates and how he can improve the product, so just sit back and wait, its the same with other vendors...
```

---
## \#536 Posted by: Kaly Posted at: 2018-02-01T00:00:47.340Z Reads: 292

```
[quote="danggilmore, post:534, topic:24654"]
not responding is kinda lame.
[/quote]

This is my problem with some members of the community and why i keep to myself sometimes but not today, the main point is that you have no idea, even how to IMAGINE or where to START a project like this and because you paid the man some miserable amount of money for him to make a FAVOR  for you, because this is what this remote is for the community, now you come to throw some dirt by calling his attitude LAME and act like you are deserving because he can not respond back to you immediately. If your hard earn money is so important just send me your PayPal and I’ll refund your payment but you will have to just leave the man alone until he get back to you when he can.
```

---
## \#537 Posted by: caustin Posted at: 2018-02-01T00:21:40.904Z Reads: 279

```
Agreed and many times over. This is not Amazon, people who have been on the forum as long as everyone on this thread seems to be, know better.
```

---
## \#538 Posted by: Deckoz Posted at: 2018-02-01T00:47:09.642Z Reads: 276

```
I love mine...it was well worth the wait. 

But I still wanna get step files to Mill the case from aluminum :(
```

---
## \#539 Posted by: mmaner Posted at: 2018-02-01T01:00:27.703Z Reads: 271

```
That's a frikkin weapon 😀
```

---
## \#540 Posted by: danggilmore Posted at: 2018-02-01T01:41:49.264Z Reads: 293

```
@kaly 

i didn't throw any dirt but im about too..... to you and you only.

i NEVER said his attitude was lame. i've never spoken to him so how can i make a judgement on him or his character. i said "not responding is kinda lame" and i do think i deserve a response after spending over a hundred dollars. like i said IMO. which means in my opinion. i wasn't attacking anyone such as your attacking me.

he's made a company with a website and a product. this isn't a favor. it's a business transaction. i have the utmost respect for what he's made and appreciate him in the community or else i wouldn't have purchased.

why don't you go back to reddit and argue with more customers like i've seen on mulitple occasions.......? 

i've been nothing but positive and supportive to every person i've ever interacted with on this forum. if you think throwing dirt is asking for a response........your not worth the two minutes i took typing this.

thanks for your input ERNIE. first and only response KALY NYC will ever hear from me. 

good day sir.
```

---
## \#541 Posted by: SkaterBoy58 Posted at: 2018-02-01T01:43:57.263Z Reads: 282

```
Deckoz  - Do you know what VESC FWs the new receiver is compatible with?  Cheers
```

---
## \#542 Posted by: Kaly Posted at: 2018-02-01T02:04:33.740Z Reads: 288

```
I am pretty sensible to people taking jabs ( small ones or hard ones) at someone doing great thing. 
The man can't get back to you right away regardless if  you paid or not. He is in the early stage of developing something for the community that really need and he is making it a reality.
This is not attacking you but talking straight up.
```

---
## \#543 Posted by: ElskerShadow Posted at: 2018-02-01T09:05:44.187Z Reads: 282

```
And what a thing ! I waited months for this remote but each day of wait was worth it. Defenitely a game changer in the DIYcommunity
```

---
## \#544 Posted by: Mattmccrary8 Posted at: 2018-02-01T16:32:11.022Z Reads: 274

```
Has anyone received the remote with the antenna and got it working correctly. Could you post pictures of all vesc setting because mine disconnects after 5 seconds and won’t rebind now. Any help is appreciated
```

---
## \#545 Posted by: uigiroux Posted at: 2018-02-01T17:39:04.619Z Reads: 276

```
Just to clarify, if your running dual motors, you only need one receiver, just have the vesc connected, right?  I don't need a receiver for each vesc do I?  I was just looking at buying one and one of the things it said was 'supports up to four receivers' so I didn't know if that was for a 4WD build, 1 receiver for each vesc...?
```

---
## \#546 Posted by: Deckoz Posted at: 2018-02-01T17:48:40.534Z Reads: 276

```
one receiver, two or more esc's over canbus. multiple receivers for multiple boards...
```

---
## \#547 Posted by: uigiroux Posted at: 2018-02-01T17:56:46.900Z Reads: 277

```
Ok got it, ty!
```

---
## \#548 Posted by: Deckoz Posted at: 2018-02-04T01:42:12.129Z Reads: 285

```
@Wajdi

 http://forum.eboardshop.net/t/photon-updater-guide/55

You posted the updater guide... But where's the download link?
```

---
## \#549 Posted by: Wajdi Posted at: 2018-02-04T05:43:03.530Z Reads: 311

```
Photon updater download now available at http://eboardshop.net/product/photon-updater/
List of firmware files now available at http://forum.eboardshop.net/t/firmware-update-download/59/1

http://forum.eboardshop.net/uploads/default/original/1X/5ceae37007cad7c7a68ae23f528ede531391b565.PNG
http://forum.eboardshop.net/uploads/default/original/1X/18d70c748207a1bd6f85f542cc5b7b8827096b4f.PNG
```

---
## \#550 Posted by: SkaterBoy58 Posted at: 2018-02-05T09:31:38.596Z Reads: 298

```
Hi Deckoz  - wondering if you have upgraded your firmware yet?

I have but cant get the remote to communicate with vesc . I am running 4.12HW and 3.100 FW which I think is the same as you.

Could you please PM me your motor and app files or give any pointers on critical settings in 3.100 FW to get the remote to communicate with vesc.

Thanks a lot
```

---
## \#551 Posted by: SkaterBoy58 Posted at: 2018-02-06T07:43:35.816Z Reads: 296

```
Wadji - Is this comment relating to modified firmware for remote or receiver ?

I have updated remote FW but still cant communicate with vesc ( on 3.30 FW)

Do I need a receiver FW update?

Thanks
```

---
## \#552 Posted by: Deckoz Posted at: 2018-02-06T15:18:43.742Z Reads: 303

```
[quote="SkaterBoy58, post:550, topic:24654"]
critical settings in 3.100 FW to get the remote to communicate with vesc.
[/quote]

I have it running on the old firmware. Will update the remote tonight and let you know.
```

---
## \#553 Posted by: Wajdi Posted at: 2018-02-06T19:50:05.159Z Reads: 310

```
It was tested on VESC FW 2.18, 2.54, and should work on all versions from 2.18 up to 3.32. You can use an earlier version than 3.33 on the VESC.
Make sure that the baud rate is set to 115200.

![IMG_1703|375x500](upload://qpn9jrDZaxqVAfBzftTI2kR2naG.JPG)

I also have several of the remotes assembled for people that pre-ordered, and I'm just waiting for an NRF batch from China, that I ordered a month ago, to be shipped to me to send them out. I hate when this happens, sometimes I get my packages in 1-2weeks, sometimes it just get lost causing unnecessary delays...
```

---
## \#554 Posted by: SkaterBoy58 Posted at: 2018-02-07T00:18:12.495Z Reads: 291

```
Deckoz  - Thanks a lot - really want to get this outstanding remote sorted and working on FWs 3.100  and 3.32
```

---
## \#555 Posted by: Darklinks Posted at: 2018-02-07T01:00:32.381Z Reads: 289

```
I hope my remote is One of those 😬😬 I been waiting a while for it now can’t Waite to try it
```

---
## \#556 Posted by: ElskerShadow Posted at: 2018-02-08T15:01:56.534Z Reads: 299

```
Mate could you answer the PM I sent you ? I dunno what to do with the remote. I recieved it 1 month ago and could use it 1 time. After spending 10 days to find a way to bind the thing, i finally made it. After a single use the connection of the remote was lost. Since then IMPOSSIBLE to bind the reciever with remote and I am sure i done everything right.

I would like to add too that i've been waiting and been very patient overall, I recieved a remote ( month late ) without Jumper,  no Cables for connection between VESC and Reciever , no charger + i had to pay 70 euros of VAT - when jerry sent me the 600 euros carvon V3 i had not to pay a single penny in VAT- ( 200 euros for a remote i still can't use after a month understand that i'm salty ). I have not complained of anything of this to you and systematically accepted the circumstance wether it was the longs delays, or missing stuff in the package. I am just asking for one thing, a decent customer service with fast answers. Other's can do it so you can as well. 

And seeing you been around on the forum and not answering my inquirie makes me mad. Customers problems should be solved, especially when they are among the first that pre-ordered.
I'am sending this message after spending again couple hours trying everything to bind the remote, did everything like on your guide. Jumped the PCB as it should be and did everything meticulously, I get the orange light but it will never bind.
 I loved this remote from the first sight, it's very practical since the only thing I can do with it is look at it
```

---
## \#557 Posted by: Wajdi Posted at: 2018-02-08T15:21:03.579Z Reads: 293

```
Hey @ElskerShadow

I don't know if Im missing something or what, but I never received notification of your PMs. I usually respond within 24 hours. Any one had this happen before? I iterally had to go though all previous messages to see yours, and the forum never sent me notification. It didn't even receive an email notification.

Regarding your issue, check PM, I'm sending you instructions on how to solve this.
```

---
## \#558 Posted by: lennylogs Posted at: 2018-02-08T15:50:19.859Z Reads: 283

```
I haven't received my remote yet, but for what it's worth, @Wajdi has always responded to my emails within a day or two
```

---
## \#559 Posted by: Jreamer Posted at: 2018-02-08T15:56:01.258Z Reads: 282

```
Check his post from 2 days ago.
```

---
## \#560 Posted by: Wajdi Posted at: 2018-02-08T16:51:00.353Z Reads: 281

```
FW 0.21 released with the following changes:

- Reduced power consumption when in sleep mode.
- Fixed a bug related to binding issues
- Fixed instances of “on awake” boot up freezing.

Can be downloaded here http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#561 Posted by: ElskerShadow Posted at: 2018-02-08T17:00:18.837Z Reads: 284

```
The PM’s might get messy i guess. Checking them to solve this, snow has melted and remote needs to be tested on the field ! :slight_smile:
```

---
## \#562 Posted by: mmaner Posted at: 2018-02-09T14:16:22.371Z Reads: 280

```
@Wajdi is anyone else having driver problems?  I cant seem to get the device driver to load...

![image|208x120](upload://rHXx9FGwVBt2PWX920wVT246416.png)
```

---
## \#563 Posted by: Wajdi Posted at: 2018-02-09T14:34:07.028Z Reads: 275

```
@mmaner Do you have the Arduino IDE installed? if not, download and install it. It does have the necessary drivers.
```

---
## \#564 Posted by: zyphaz Posted at: 2018-02-09T16:19:33.816Z Reads: 273

```
Just ordered one, can't wait!  

I assume the next wave is still for pre-orders right?  How long is the est. lead time for orders placed now?
```

---
## \#565 Posted by: Wajdi Posted at: 2018-02-09T16:49:46.912Z Reads: 276

```
Thank you. I’m trying to get all the parts needed before the Chinese New Year holiday, which is next week, especially since my last nrf package was lost and now I need to wait for a new one :weary:
I should have all the parts by next week, and will start shipping them out.
```

---
## \#566 Posted by: mmaner Posted at: 2018-02-09T17:19:27.857Z Reads: 273

```
I just ordered a second one too.  My kid is gonna crap his pants :slight_smile:
```

---
## \#567 Posted by: stormboard1 Posted at: 2018-02-09T17:52:22.247Z Reads: 271

```
why are some of the remotes smaller in the picture above?
```

---
## \#568 Posted by: Deckoz Posted at: 2018-02-09T17:54:39.141Z Reads: 270

```
The newest pcbs have integrated cruise control button. Meaning the length of the neck above the stick can be shorter. As the button is on the pcb vs wired to the pcb
```

---
## \#569 Posted by: stormboard1 Posted at: 2018-02-09T17:57:28.222Z Reads: 267

```
cool was wondering was it just the printer, man these look so good between the remotes and the bluetooth speaker with wheels serious workmanship :sunglasses:
```

---
## \#570 Posted by: oripaamoni Posted at: 2018-02-09T19:02:52.923Z Reads: 270

```
Wow this is amazing... great work! What the lead time if I order now, Also how many are out there? I love the design and functionality but I am a bit afraid to venture away from my tried and true gt2b based remote.
```

---
## \#571 Posted by: mmaner Posted at: 2018-02-09T22:39:04.852Z Reads: 278

```
[quote="Wajdi, post:563, topic:24654, full:true"]
@mmaner Do you have the Arduino IDE installed? if not, download and install it. It does have the necessary drivers.
[/quote]

I've tried 2 PC's, multiple USB cables, both old and new Arduino IDE...even tried to manually install the driver but the device manager still doesn't see the driver for the remote?  Any suggestions?  I feel like I'm missing something bviouse here :slight_smile:
```

---
## \#572 Posted by: Wajdi Posted at: 2018-02-09T23:41:24.980Z Reads: 265

```
Which Windows OS are you using?
```

---
## \#573 Posted by: mmaner Posted at: 2018-02-10T02:07:57.939Z Reads: 270

```
Windows 7 pro x2 and Windows 10 Enterprise.
```

---
## \#574 Posted by: Wajdi Posted at: 2018-02-10T02:14:06.331Z Reads: 287

```
Here is a guide on how to install the driver, Photon remote uses same bootloader as arduino zero. https://www.arduino.cc/en/Guide/ArduinoZero#toc3
Let me know if it works.
```

---
## \#575 Posted by: mmaner Posted at: 2018-02-10T02:15:36.919Z Reads: 303

```
I'll give it a shot, thanks for.posting that.
```

---
## \#576 Posted by: uigiroux Posted at: 2018-02-10T03:59:41.565Z Reads: 315

```
Although I'm for sure buying the Photon remote, I just came across this one: 
![Screenshot_20180209-200956|667x500](upload://mW5MGwB8LRYu5iYD8ZnrRDcp3nf.jpg)
https://evolveskateboardsusa.com/products/r-2-remote
The Evolve R2.  I really love its design and separate  triggers for accelerate and brake, but I am pretty sure your Photon has more features.  Can you say what features yours has over the R2?  Also, I think I recall you saying something about making another design of your remote for those who prefer trigger style.  Is that something you are planning once you get all the bugs sorted out in the current model by any chance?
```

---
## \#577 Posted by: codespanker Posted at: 2018-02-10T05:48:51.154Z Reads: 304

```
The evolve r2 only works with evolve boards. This is universal
```

---
## \#578 Posted by: Exiledd_Top Posted at: 2018-02-10T05:54:06.426Z Reads: 304

```
I don't think you read it correctly he's mererly using it as a design example wanting something as a R2 design with same features as his current remote @codespanker
```

---
## \#579 Posted by: uigiroux Posted at: 2018-02-10T11:34:50.674Z Reads: 308

```
That's correct! Lol
```

---
## \#580 Posted by: SkaterBoy58 Posted at: 2018-02-11T06:54:06.192Z Reads: 323

```
@Deckoz   - How did you go with vesc FW3.100 communicating with photon?
```

---
## \#581 Posted by: Deckoz Posted at: 2018-02-13T20:07:09.225Z Reads: 336

```

@mmaner I had trouble too...but here's what I did

 So first things first. The Updater rely's on the following C++ redistributable package(x86)

https://www.microsoft.com/en-us/download/details.aspx?id=52685

second... open Computer management , Uninstall the photon if it has a driver. Then right click, and "update driver"

"Browse my computer for driver software"
"Let me pick from a list of device drivers on my computer"
Click "Have Disk"

Navigate to your Arduino Installation, goto the Driver Folder, and select the "arduino.inf"
![image|681x500](upload://teDhI3FMU99PsqtO2BZjLMtdiFs.png)

Select "Arduino LLC(www.arduino.cc)" and find Arduino Zero in the right hand list

![image|617x209](upload://siUtErx01UHo1oF3cE0ju29iY1l.png)

After Install, it should now have a COM Port.

![image|600x289](upload://5luUG0fMxQ1M2DhWtiULGjJTm83.png)

Once you click flash it is going to reboot into bootload/DFU mode which you also do not have the driver for, repeat the above process and instead this time select Arduino Zero Bootloader 

![image|607x227](upload://jALS6OjECv7fmKo7053mxU3Dr7Q.png)

Refresh the ports list so that you see the DFU Com, and then reflash.

Should now be updated

![IMG_20180213_143651|374x499](upload://s447eaqTMLyG78aQ19kWammYIzH.jpg)


@SkaterBoy58 

 After updating, and using the new receiver, I cannot control with 3.100 either. 

I could communicate with both 2.54 and 3.100 on the original receiver...however the original receiver doesn't work after updating... and I also see the same thing you do "255.2" @Wajdi
```

---
## \#582 Posted by: mmaner Posted at: 2018-02-13T20:20:13.851Z Reads: 294

```
Great write up, I really appreciate it.  I haven't tried again since Friday, new puppy and bronchitis so...
```

---
## \#583 Posted by: Wajdi Posted at: 2018-02-13T20:26:52.411Z Reads: 285

```
Great tutorial @Deckoz thanks for taking the time to write this up. Can anyone point me to the source code of FW 3.100? I will look into this today.
```

---
## \#584 Posted by: Deckoz Posted at: 2018-02-13T20:28:20.119Z Reads: 289

```
Hmmm.

@Ackmaniac would you mind sharing your changes to UART with @Wajdi to help get this working   :)
```

---
## \#585 Posted by: SkaterBoy58 Posted at: 2018-02-13T23:28:05.340Z Reads: 295

```
@Wadji  - Maybe you could re-flash your vesc FW to both 3.100 and 3.32 and see if the remote uart comms works OK and let us all know if any issues.

It could be quite limiting for the photon remote if it can only work on FW 2.18 as I think most DIYers would be well beyond 2.18 and some uart apps (such as metr) do not fully function below vesc FW 3.29.  

Most would also want to use VESC Tool and I think the vesc FW for the first public release of the VESC Tool (0.81) in Sept 2017 was vesc FW 3.28. AFAIK you cannot use the VESC Tool on vesc FW 2.18.( bldc tool only)

Just a idea - maybe  the remote could have the vesc FW as a user selection in the control menu - and then your mcu smarts takes care of everything else?. Pretty sure the uart libraries etc. for the various FWs are open source. 

 I think some vesc FWs updates do not change the uart libraries so there may not be too many different versions to code up. 

Cheers
```

---
## \#586 Posted by: Deckoz Posted at: 2018-02-13T23:37:46.905Z Reads: 274

```
Currently it auto detects everything below 3.32, that includes 2.11-2.18, Ack 2.54, and all vesc tool releases before 3.32. 

It's not so much the libraries. But the data packet structure :)
```

---
## \#587 Posted by: SkaterBoy58 Posted at: 2018-02-13T23:57:42.106Z Reads: 273

```
no worries -I cant get it to communicate on any 3.xx FWs
```

---
## \#588 Posted by: Deckoz Posted at: 2018-02-13T23:58:54.731Z Reads: 275

```
When you are checking for connection on the other firmwares, you have Real time data enabled on the right hand bar of the VESC tool correct?
```

---
## \#589 Posted by: lock Posted at: 2018-02-14T00:00:38.270Z Reads: 291

```
[quote="Deckoz, post:586, topic:24654"]
It’s not so much the libraries. But the data packet structure :slight_smile:
[/quote]

^ this

About the only thing an external app should rely across all VESC versions is the VESC reporting what firmware it has. Really an app should check what firmware is running on the connected VESC and then decide if it's supported or not. There doesn't seem to be any consideration for backwards compatibility, so you can't assume future versions will use the same data packets or even the same message ids. To support multiple firmware versions you'd have to include the details of the datatype definitions ([`datatypes.h`](https://github.com/vedderb/bldc/blob/5348662197c69a00b7bdea42423674e339db3976/datatypes.h)) for each firmware.
```

---
## \#590 Posted by: SkaterBoy58 Posted at: 2018-02-14T00:31:50.215Z Reads: 288

```
yes -but cant even get basic telemetry comms (vesc input voltage ,vesc fw version etc.) on remote to work (with no vesc tool connected)
```

---
## \#591 Posted by: Wajdi Posted at: 2018-02-14T00:53:34.725Z Reads: 294

```
[quote="Deckoz, post:586, topic:24654, full:true"]
Currently it auto detects everything below 3.32, that includes 2.11-2.18, Ack 2.54, and all vesc tool releases before 3.32.
[/quote]
That's correct, I will be testing all versions today and report back what works and what not, I dont really understand why they keep changing the COMM_GET_VALUES data structures every now and then, at least make it backward compatible, all changes that have been done to the COMM_GET_VALUES packet aren't really that useful, or maybe they can just leave COMM_GET_VALUES alone, and create a new packetid to shove all the extra unnecessary stuff to it.
```

---
## \#593 Posted by: JasperM Posted at: 2018-02-24T11:11:15.744Z Reads: 280

```
Hey Wajdi,

Any news on the pre-orders shipping?

Is my order in the ones that are awaiting the NRFs?
Order #228

Cheers
```

---
## \#594 Posted by: uigiroux Posted at: 2018-02-24T17:32:46.503Z Reads: 268

```
What's the wait roughly around?
```

---
## \#595 Posted by: LEE Posted at: 2018-02-25T15:36:50.744Z Reads: 259

```
I am waiting for shipment from the end of last year.
By the way, are the two LED ports total 5V1A?
```

---
## \#596 Posted by: Darklinks Posted at: 2018-02-25T15:48:05.670Z Reads: 269

```
I don’t know what going on but he told me he would ship my remote last week and he didn’t. Reached out to him again and have not hard for him again
```

---
## \#597 Posted by: uigiroux Posted at: 2018-02-26T00:57:14.115Z Reads: 265

```
I have a question about using this remote with the VESC 6 clone, the ESCape.  I was told that the ESCape has NRF built in, and because of this a receiver isn't needed to connect a remote.  It's that true and does it apply with this remote, or do we need the receiver this remote comes with to run on the ESCape?

Another question, I know you can connect this receiver to a Y cable and connect to two VESC's.  Is it better to just connect this way, or connect to just one VESC and use CANBUS with master/slave setup?
```

---
## \#598 Posted by: Deckoz Posted at: 2018-02-26T01:06:26.920Z Reads: 260

```
This remote is designed for uart connection and Nunchuckcontrol over canbus.

If you use pom you won't get any of the stats making it a regular remote...and a worthless screen..
```

---
## \#599 Posted by: uigiroux Posted at: 2018-02-26T01:17:57.614Z Reads: 272

```
Ok, so receiver allows for the telemetry to be seen on screen. 

Is it better to connect receiver to both VESC or just one and use CANBUS?  Or even put a receiver on each VESC?
```

---
## \#600 Posted by: Deckoz Posted at: 2018-02-26T01:19:04.813Z Reads: 272

```
It only connects to one via UART. You must use canbus for two vescs
```

---
## \#601 Posted by: uigiroux Posted at: 2018-02-26T01:20:13.887Z Reads: 290

```
I thought there was a cable that connected to the receiver and then split so you could connect to both VESC, eliminating the need for CANBUS.
```

---
## \#602 Posted by: Deckoz Posted at: 2018-02-26T01:23:54.386Z Reads: 305

```
![IMG_20180225_202222|666x500](upload://pwux8ajvyZBLq4xtdqel8WWFg66.jpg)

Receiver on right connected to master focbox uart. Canbus cable from master to slave focbox. Uart on slave connected to Bluetooth module for Android app. 

PPM cables not connected

There's no split from the receiver.
```

---
## \#603 Posted by: uigiroux Posted at: 2018-02-26T01:28:44.328Z Reads: 291

```
What Android app are you referring too?
Also what are the PPM wires for?
```

---
## \#604 Posted by: Deckoz Posted at: 2018-02-26T01:29:52.180Z Reads: 291

```
Um anything like metr or ackmaniac firmware? So you can change settings on the go?

Or wirelessly change settings from your computer?  The Bluetooth has nothing to do with the remote
```

---
## \#605 Posted by: uigiroux Posted at: 2018-02-26T01:31:14.517Z Reads: 287

```
I thought we were able to change settings over the remote also..
```

---
## \#606 Posted by: GrecoMan Posted at: 2018-02-26T01:32:25.133Z Reads: 285

```
you can change remote settings with the remote...
```

---
## \#607 Posted by: Sender Posted at: 2018-02-26T01:32:42.278Z Reads: 284

```
That picture is infinitely useful to me, lol. THANKS
```

---
## \#608 Posted by: Deckoz Posted at: 2018-02-26T01:33:05.041Z Reads: 285

```
The remote let's you change settings important to the remote. Like your drive ratio...and things like that


You cannot setup a motor or change wattage or amperage n the remote you need bldc/vesc tool, metr or ackmaniac firmware, or metr Bluetooth as a tcp bridge to vesc tool to do configuration without a usb cable
```

---
## \#609 Posted by: uigiroux Posted at: 2018-02-26T01:37:19.066Z Reads: 284

```
Oh that's freaking sweet!  And you can access both VESC this way, or does it just make the settings apply for both VESC as you change them?  That's too bad we can't access that app over the remote so you could change things both for the remote, and the VESC as well.

Also, sorry to keep asking,  but what are the PPM cables for?
```

---
## \#610 Posted by: Deckoz Posted at: 2018-02-26T01:40:11.660Z Reads: 297

```
You just enable CAN FWD with the numerical ID of the ESC that you set (ie master = 0, slave = 1... You have to set this as default is 0 on all esc, don't expect this to magically work)

So can fwd = 1 would show me the settings of the slave....

Ppm is the servo leads in my picture that aren't connected (redblackwhite)
```

---
## \#611 Posted by: uigiroux Posted at: 2018-02-26T01:43:18.366Z Reads: 292

```
Yeah I know what they are in the pic, but what does a servo lead do is what I'm trying to find out.
```

---
## \#612 Posted by: Deckoz Posted at: 2018-02-26T01:50:04.141Z Reads: 298

```
Regular remotes use PPM......
```

---
## \#613 Posted by: Scoo_B_SK8 Posted at: 2018-02-26T02:06:49.595Z Reads: 303

```
https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTuFDMBbnvktPiYqm6emEu5gKTdgiC6yv_Oe6dIrMnqHgGUTkYSVA

![image|600x194](upload://zcrePNqVkidZbNGkM2ZasE4RqI2.jpg)
```

---
## \#614 Posted by: Clonkex Posted at: 2018-02-26T02:07:22.461Z Reads: 294

```
The PPM wires connect to a normal RC receiver. That's how most people send their throttle/brake signals to the VESC. They're also called servo leads because a) PPM signals are what you control servos with (though technically it's a form of PWM), b) servos use the same three wires (power, ground, signal) and c) servos use the same type of plug.
```

---
## \#615 Posted by: Wajdi Posted at: 2018-02-26T02:11:19.924Z Reads: 297

```
@JasperM I have been fulfilling many pre-orders last week, and yours is coming up shortly.
@uigiroux I'm doing my best to get done with pre-orders soon, every time I try to have some in stock, they sell quickly. I have a new batch in progress with approximately 12 openings right now, for a wait time of about 1 week.

@LEE Pm me your order number, I recently sent tracking numbers for a large portion of pre-orders queue. Yes the combined max output should not exceed 1A, they are 5V. It is recommended to run your own power supply for the LEDs tho.

@Darklinks Sorry I have been very busy last week. I fulfilled several orders, and yours should be ready tomorrow and shipped on Wednesday.

@uigiroux I didn't get the chance yet to test the new VESC6 clone, but chances are you still need the Photon receiver. Photon connection uses FHSS, the receiver has the sync algorithm in place to resolve it.
About the double VESC setup, it is easier to just use CAN bus, I didn't test connecting the receiver to two ESCs at the same time. The remote however does support multiple receivers, so you can do that as well.
```

---
## \#616 Posted by: Jc06505n Posted at: 2018-02-26T02:24:34.831Z Reads: 285

```
Zip ties on the Bluetooth 🧐 shoulda thought of that.
```

---
## \#617 Posted by: JasperM Posted at: 2018-02-26T06:17:30.087Z Reads: 289

```
Cheers mate,

Thanks for the update.
```

---
## \#618 Posted by: Deckoz Posted at: 2018-02-26T15:51:40.839Z Reads: 289

```
@Wajdi any update or communication with @Ackmaniac to get the photon working on 3.100?
```

---
## \#619 Posted by: Darklinks Posted at: 2018-02-26T16:31:53.723Z Reads: 288

```
Cool hope to get it soon 😬
```

---
## \#620 Posted by: Wajdi Posted at: 2018-02-27T15:19:01.804Z Reads: 287

```
Not yet. I'm testing all official FW versions today.
```

---
## \#621 Posted by: Zigm4 Posted at: 2018-03-01T16:42:49.902Z Reads: 292

```
Hi,

It's not easy to get in touch with you :stuck_out_tongue:
I never got the confirmation email for my order (#248). Seems your system don't like .at domain names :slight_smile:
Is it possible to get an update on my order and update the email address (see my message on messenger)

Anyway, congrats for yur incredible job. I'm pretty sure there is a huge potential for electric engines remotes !

Thanks,
Zigm4
```

---
## \#622 Posted by: ElskerShadow Posted at: 2018-03-01T18:52:57.915Z Reads: 281

```
I had the same problem when I ordered I couldn’t see my order and had no confirmation mail either 
But the order was there so don’t worry too much I think
```

---
## \#623 Posted by: Zigm4 Posted at: 2018-03-02T09:15:13.661Z Reads: 288

```
@ElskerShadow : I not worrying, he already confirmed my order is processing :slight_smile:
But that's the last part i need to finish my build with @Riako :smiley:
I have few questions :
* When did you placed your order and how long it took to receive it ?
* What do you think about this remote (vs. a GT2B, R1/R2, ...)

@Wajdi : Still no emails even with the other email... Maybe your system is not working :thinking:
I also saw you might plan to change the design, will it be possible to order just the printed box ?

Have a great day !
```

---
## \#624 Posted by: NAF Posted at: 2018-03-02T09:21:28.227Z Reads: 278

```
Damn I wish @Wajdi could design a second version of his remote with two separate buttons like this.  
That Evolve R2 is great ..and feels great. Having two buttons was a very clever idea.
```

---
## \#625 Posted by: Wajdi Posted at: 2018-03-02T21:59:11.950Z Reads: 273

```
@Zigm4 I tried to send you the order confirmation manually right now, let me know if you still don't receive it.
I'm not changing the design any time soon, perhaps in the future I will work on an additional version.
```

---
## \#626 Posted by: treenutter Posted at: 2018-03-02T22:03:55.386Z Reads: 282

```
[quote="PredatorBoards, post:383, topic:24654"]
Dont bother with board-mounted data clusters
[/quote]

I agree w this.. the concept of having a "dashboard" is cool but on a board (moreso than on a bike or a car) you really need all your focus on the road so you can react to what is happening.The data available isn't really helpful unless you are prototyping/testing electronics. I passed on a coulometer for this reason.
```

---
## \#627 Posted by: Zigm4 Posted at: 2018-03-02T22:18:23.681Z Reads: 286

```
[quote="Wajdi, post:625, topic:24654"]
I tried to send you the order confirmation manually right now, let me know if you still don’t receive it.
[/quote]

I got it :smiley:
But still no information on the expected shipping date and tracking code, normal ? :)
```

---
## \#628 Posted by: Wajdi Posted at: 2018-03-02T22:21:38.713Z Reads: 275

```
Yes, you will receive an email with tracking information once it is shipped. Expected in about 10 days.
```

---
## \#629 Posted by: Zigm4 Posted at: 2018-03-02T22:42:23.930Z Reads: 276

```
Thanks a lot !
Please don't forget to send the email directly to my email address (not with you mailing tool)
```

---
## \#630 Posted by: lazerusrm Posted at: 2018-03-04T08:20:10.803Z Reads: 283

```
Wajdi,

    I'm so excited for this combo! I purchased the remote and the receiver off your website on Feb 26 Using paypal.

Do you have an ETA for future remotes?  Order ES-252. This remote is very desirable for me, as my current setup is a bit too touchy.

I have dual 80MM 6kw motors running 12s.  need a better controller. :) Mostly for brake ramp and initial startup smoothing. I will have questions too on how to hook to dual VESC and also dual BL-Control 9120 150A Esc's.

I just realized i may need two receivers for dual motor. Is this the case? can you invoice me for another one through paypal or something so i can make sure i have what i need? Thanks -- _*

*EDIT: ElskerShadow answered this Question ^^^
```

---
## \#631 Posted by: ElskerShadow Posted at: 2018-03-04T10:13:17.269Z Reads: 273

```
[quote="lazerusrm, post:630, topic:24654"]
need two receivers for dual motor. Is this the case?
[/quote]
No you just need canBUS and enable in the VESCtool the can FWD
```

---
## \#632 Posted by: lazerusrm Posted at: 2018-03-04T10:20:45.493Z Reads: 266

```
Thanks! I've been reading a few hours on vesc and software and all that. makes sense ;)
```

---
## \#633 Posted by: Dizzee Posted at: 2018-03-06T06:39:25.717Z Reads: 274

```
I got my remote today so I immediately set everything else aside and got to work on swapping remotes thinking I could knock it out quick and go for a short ride. I was wrong and I hate software sometimes. So I have tried Ackmaniak's V3.10, stock V3.35, stock V3.31 and stock V3.29 firmwares. I realize some of the firmware versions aren't supported but I was just giving it all I had available at the time.I have the TX and RX bound with green lights on both plus I have telemetry coming through just fine on the remote. I have the baud rate set and I've tried setting it to UART as well as Nunchuck (not nrf) and selected current in the nunchuck menu. The remote button up front is set to cruise. However I am unable to get any throttle response from the motors and I can't see any indications of stick movement in the VESC Tool with any of the firmware versions I have available to me. Unfortunately I can not find any past releases of the VESC Tool for Windows other than what I have previously downloaded. My other remote works if I set it to PPM and reconnect the servo connector so the other settings seem fine. I may be skipping something simple out of frustration but I've done everything I can think of and I'm not getting anywhere. Does anyone have any ideas or know what I may be overlooking?
```

---
## \#634 Posted by: ElskerShadow Posted at: 2018-03-06T06:56:47.123Z Reads: 264

```
Can’t really help but the struggle can be hard for this remote. 
I recieved mine 2 month ago never used it because I could never bind it. Apparently @Wajdi sent me a new RX to try but been waiting for week. 
Since early January i’m the happy owner of a 170 € brick remote
```

---
## \#635 Posted by: Wajdi Posted at: 2018-03-06T20:11:59.069Z Reads: 269

```
@Dizzee I have been looking into this for the past few days, and I found the problem. I forked the bldc source code and applied necessary changes to get this working again. I will release a modified FW 3.34 tonight that should get cruise control, reverse, and nunchuck controls back on UART.
```

---
## \#636 Posted by: Dizzee Posted at: 2018-03-08T03:03:13.934Z Reads: 281

```
I can understand your frustration. It's a lot of money to have sitting around. To Wajdi's credit he's taken responsibility for the original receivers and he seems be doing what he can to get it working as intended. I'm more frustrated with the state of the VESC project. There is no reason given for the changes effecting products that do nothing but add value. For me the fact that there's no repository containing past releases of software and firmware is beyond frustrating. All I could find was a forked GitHub project containing previous releases for MAC OS. I don't want to muddy the thread with VESC frustration. I just wanted to state what effects this project directly though. Especially if a specific range of firmware is necessary for the time being.

For those that need it and can make use of it, here's a link to the previous releases of VESC Tool for MAC OS. [MAC VESC Tool Releases](https://github.com/rpasichnyk/vesc_tool/releases)
```

---
## \#637 Posted by: Wajdi Posted at: 2018-03-08T03:08:12.403Z Reads: 282

```
I just managed to have the controls compatibility issue fixed. The modified version is FW 3.35, thats the latest release, I made changes to fix nunchuck compatibility issues with the Photon receiver. 
You can download the FW from my GitHub here https://github.com/wajdib/bldc/tree/master/build_all
Make sure to choose the correct hardware version, and the default FW available.

For this you will need the latest version of the VESC TOOL as well, V0.88. 

This also applies to anyone that wants to update to latest vesc versions and have problems with controls or telemetry, this should fix it for the old Photon receivers.

Let me know if this works for you.
```

---
## \#638 Posted by: SkaterBoy58 Posted at: 2018-03-08T13:37:21.280Z Reads: 300

```
Hi Wadji 

I have tried your modified 3.35FW  VESC firmware with a focbox 4.12HW and vesc tool 0.88 with following results:

* modified 3.35 FW loaded into VESC OK

* Cannot get FOC motor detection to work at all ( does nothing) but BLDC motor detection works OK

* No telemetry at all on photon remote - still shows 255.2 as FW on remote

* Any throttle command from remote brings up vesc tool error "Serial  Port Error- Ä device attached to the system is not functional"- only way this can be cleared is by re-booting vesc ( power-down and re-power)

* Throttle command on remote spins motor OK on BLDC only ( with current - no reverse on Nunchuk ) even if VESC tool error is present ( as above) but no FOC at all

* Installing this modified firmware appears to remove any VESC PPM control via RC remote if ÜART and PPM" is selected from App Settings/General

* Cruise control seems to work OK

Any-one else tried this??

Cheers
```

---
## \#639 Posted by: Wajdi Posted at: 2018-03-09T16:28:56.215Z Reads: 285

```
Hmm, thats weird, I will look into this. BTW for anyone wondering, all new receivers are compatible with latest vesc firmwares out of the box.
```

---
## \#640 Posted by: Mattmccrary8 Posted at: 2018-03-09T22:03:05.913Z Reads: 297

```
Can anyone tell me which to area to short so I can bind this bad boy ![image|375x500](upload://e1TeTiMTgyhaBVfSEyEdTSAjNqt.jpg)
```

---
## \#641 Posted by: Slak Posted at: 2018-03-09T22:12:47.231Z Reads: 292

```
Can't tell you exactly but if you use the "search on this topic" feature with" short" or "bind"  keywords, you'll find hints. It seems to you need to read around post #498 on this topic. There's a picture, read around.

Hope this helps
```

---
## \#642 Posted by: Wajdi Posted at: 2018-03-09T22:19:43.772Z Reads: 297

```
![image|666x500](upload://8Z2TCwCSoYmG4B73BNp35vF0TrU.jpeg)
Here you go
```

---
## \#643 Posted by: JasperM Posted at: 2018-03-10T04:15:07.997Z Reads: 288

```
If I have the remote plugged in to a single focbox, can I have a Bluetooth module plugged in somewhere?
```

---
## \#644 Posted by: Deckoz Posted at: 2018-03-10T09:10:25.738Z Reads: 286

```
Not on a single focbox...

@Wajdi ... I had to install my nano remote today as I cannot get 3.100 or your 3.35 working properly. And cannot bring myself to go back to 2.54 with USB... 

I hope you can get this working soon. Without custom firmware.
```

---
## \#645 Posted by: scepterr Posted at: 2018-03-10T10:55:05.017Z Reads: 276

```
Mine should be coming today/tomorrow I'll be using it on ESCape on 3.1 but I'll test it out on a focbox as well.
```

---
## \#646 Posted by: ElskerShadow Posted at: 2018-03-10T11:52:47.517Z Reads: 277

```
Share your results when you have them !
```

---
## \#647 Posted by: SkaterBoy58 Posted at: 2018-03-10T12:06:59.830Z Reads: 277

```
@Deckoz  What worked and didnt work for you on modified 3.35 FW?
Cheers
```

---
## \#648 Posted by: Wajdi Posted at: 2018-03-10T14:36:55.305Z Reads: 280

```
@Deckoz I will be looking into this again today, to go back to 2.54 just unplug the receiver before turning on your VESC.
It is working without any custom firmware, but only on the newer receiver versions.

@scepterr Yours have the latest receiver version, which should work out of the box with the new firmwares. The new receivers support fw from 3.24 and up.

@JasperM You can't plug them both at the same with what we have so far, because they both need UART port, and only one can be connected at the time.
```

---
## \#649 Posted by: Deckoz Posted at: 2018-03-10T16:10:58.187Z Reads: 279

```
Basically everything you said

I run FOC sensored. And couldn't get foc detection working on his 3.35. still see 255.2 and no telemetry. 

I have these issues, as well Im really not one to ride untested firmware so even if this was working there is very little chance I would run this firmware over Ackmaniac 3.100

So there's two sides of the fence...I could go back to 2.54 and be perfectly fine with this remote. But I cannot wirelessly configure the vescs over a tcp bridge.

As simple as this argument sounds.. having a enclosure that is bolted up and I can configure everything from is better then going back to 2.54 trying to setup the escs with the board half disassembled make shift wires and such just to run the remote.
```

---
## \#650 Posted by: Wajdi Posted at: 2018-03-10T16:42:38.395Z Reads: 273

```
I think it is best to stick with 2.54 for now since it’s tested and fully compatible with older receivers.
```

---
## \#651 Posted by: scepterr Posted at: 2018-03-10T19:25:15.172Z Reads: 290

```
Photon arrived just now, charging it up 😋
![IMG_20180310_132242__01|320x500](upload://tTdpTHvneZZovrSk5b4c06WS7yJ.jpg)

@Wajdi is the remote PCB coated? Noticed the receiver wasn't, already coated that with polyurethane 😉
```

---
## \#652 Posted by: Wajdi Posted at: 2018-03-10T20:14:53.006Z Reads: 283

```
Nice! Pcbs are not coated, so you might wanna be careful with water exposure.
```

---
## \#653 Posted by: scepterr Posted at: 2018-03-10T20:16:33.790Z Reads: 289

```
No worries, I coat every pcb with this
![IMG_20180228_165237|375x500](upload://9LxIVZhcbPWhpuFLtHNLscSppIH.jpg)
```

---
## \#654 Posted by: DanSkates Posted at: 2018-03-10T20:55:47.951Z Reads: 288

```
Nice - hey would you use this on the pcb of your esc too? Thinking my FOCBOXs might benefit from a couple of blasts of this!
```

---
## \#655 Posted by: scepterr Posted at: 2018-03-10T21:00:47.818Z Reads: 289

```
Yep first thing I do
![IMG_20180228_164054__01|690x475](upload://aLAZUA3iPOx67Uq67ByqfGyClv8.jpg)
```

---
## \#656 Posted by: MannyM0E Posted at: 2018-03-10T21:02:26.231Z Reads: 286

```
You just straight up spray over all that and no damage is made to the esc ?
```

---
## \#657 Posted by: scepterr Posted at: 2018-03-10T21:03:01.448Z Reads: 285

```
Lol it's made to protect and insulate the electronics, so no 😋

All my BMS, receivers, remotes, voltage indicators, leds
```

---
## \#658 Posted by: MannyM0E Posted at: 2018-03-10T21:04:21.906Z Reads: 281

```
Just got 2 focbox
Might have to do this to them 
Thanks for the tip
```

---
## \#659 Posted by: scepterr Posted at: 2018-03-10T21:07:03.564Z Reads: 278

```
Having that coating could even save you from manufacturer defects that could get worse with vibration since that basically glues everything down
```

---
## \#660 Posted by: fedestanco Posted at: 2018-03-10T21:15:00.735Z Reads: 278

```
 How does it behave when you try to solder over it or to use hot air station? Does it catch fire like standard urethane or it acts like flux?
```

---
## \#661 Posted by: scepterr Posted at: 2018-03-10T21:50:59.330Z Reads: 277

```
Cant really solder over it, gotta scrape it off , never seen it catch fire
```

---
## \#662 Posted by: scepterr Posted at: 2018-03-11T00:41:50.560Z Reads: 283

```
@Wajdi if I want to power the receiver independently how much current can it handle passing to the LEDs, 3-4A total ok? And if I do that do I still need the ground going to the vesc?
```

---
## \#663 Posted by: Wajdi Posted at: 2018-03-11T01:41:53.320Z Reads: 286

```
![10 PM|690x359](upload://poApBfO0GAYXJGYEcCwlhkZVmT7.png)

By powering the receiver independently I assume you mean supplying external power for the LED's but still powering the receiver itself from the VESC, because the receiver needs a regulated 3.3v from the VESC to operate.

(Assuming your are using a WS2812B strip or equivalent)
Now for the LEDs, I suggest you unpin the +5v pin from the UART cable, this will cut +5v supply from the vesc, but leaves the other +3v3 pin to supply the receiver mcu.
Next, from the schematic there are two ports, front light and back light, each has a data pin, power supply and GND. You connect your power supply to +5V, your power supply GND to GND, and data pin to your led strip data pin.

If you are not using individually addressable LEDs, and just want a way to toggle ON/OFF from the remote, then you can use the digital control pin A2, for this you will need a logic level mosfet (N channel for this example) where you feed A2 to it's gate (With a small resistor in series to protect against over current), source to GND and drain connected to your device GND. and use that to switch whatever you want On/Off. 

If its still not clear, just show me what you got and I will help you hook it up.
```

---
## \#664 Posted by: scepterr Posted at: 2018-03-11T01:48:26.499Z Reads: 278

```
Oh ok I didn't realize it was using 3v3, thought it was 5v, yeah I'll just remove the 5v then 👍
```

---
## \#665 Posted by: scepterr Posted at: 2018-03-12T01:43:46.928Z Reads: 293

```
My slight transreceiver mod for min height
![IMG_20180311_214148__01|690x404](upload://aJoBMmJy8W2XmlyvbaGg88zOBGj.jpg)
![IMG_20180311_223406__01|690x435](upload://yRRZGJpGqNAXr3uSXqcQw74Y1bC.jpg)

@Wajdi one thing I noticed while getting everything ready is the remote battery drains while off and drains significantly while on but idle, had it sitting on a counter for 2.5hrs and it dropped 80%.  An auto shutoff in 10min if disconnected and no buttons pushed would be great, I have a feeling I'll be picking up a remote with a dead battery a lot of the time. I would like to be able to charge every 2-3 days atleast, daily is gonna be cumbersome.
Also would a double tap to turn on be possible to prevent accidental turn on
```

---
## \#666 Posted by: Wajdi Posted at: 2018-03-12T02:01:29.108Z Reads: 279

```
@scepterr I'm actually working on a new software update for the remote that has an auto-off function after some inactivity time :slight_smile: 
About the battery life, one way you can extend your runtime by going to menu, and under controls, there is a SGN setting, it can be set to MIN, LOW, HIGH, and MAX. You might want to change that from MAX to HIGH for example. The SGN setting controls the power of transmission, MAX will have the best range but it will also consume a lot of power. Try the other power options and find a balance between range and power usage.
```

---
## \#667 Posted by: scepterr Posted at: 2018-03-12T02:03:42.814Z Reads: 274

```
Yeah I have it set to MIN, and the lowest brightness setting, I'm guessing it's the screen taking most of the juice? Possible for an even lower brightness setting or is that as low as the backlight unit allows?
```

---
## \#668 Posted by: Wajdi Posted at: 2018-03-12T02:06:49.801Z Reads: 277

```
Most if the juice goes into the display, nrf module, and then the MCU. Unlike other remotes on the market, this one uses a 32bit cpu, which is fast and responsive, but consumes more power. The display does drain a significant amount of power as well, mostly in back-lighting. I will try to come up with an option to adjust brightness as well.
```

---
## \#669 Posted by: scepterr Posted at: 2018-03-12T02:08:26.384Z Reads: 264

```
Oh and definitely a screen off while remote on option, if desperate and low on battery or just need the extended range be able to use without screen on

Like triple tap button A turn screen on/off while remote on
```

---
## \#670 Posted by: Wajdi Posted at: 2018-03-12T02:09:32.324Z Reads: 258

```
Good idea, will add that to my TODO list. maybe a fast double click on the joystick can toggle the screen on and off.
```

---
## \#671 Posted by: Colson003 Posted at: 2018-03-12T02:12:35.754Z Reads: 263

```
[quote="Wajdi, post:668, topic:24654"]
mostly in back-lighting
[/quote]

Maybe OLED would be worth it?
```

---
## \#672 Posted by: Wajdi Posted at: 2018-03-12T02:14:14.555Z Reads: 260

```
I initially started by using an OLED display, but it was too small and there isn't many options to choose from when it comes to size.
```

---
## \#673 Posted by: Deckoz Posted at: 2018-03-12T02:17:48.160Z Reads: 271

```
@scepterr

Mine has been charged for over a month in the past and a couple weeks while using it daily... 

you also gotta remember this is a lipo, so the voltage meter isn't quite scaled right. the top of the battery drops off quick but then holds forever..
```

---
## \#674 Posted by: scepterr Posted at: 2018-03-12T02:20:00.723Z Reads: 260

```
Yeah I wasn't too concerned about the top end it was the 80% drop in 2.5hrs sitting on  a counter
```

---
## \#675 Posted by: Wajdi Posted at: 2018-03-12T02:20:56.277Z Reads: 273

```
@Deckoz yes thats actually correct, percentage is not always accurate. One more thing to note is that when charging the remote, there is an orange LED near the charging port, you have to wait until it goes off to make sure the remote was fully charged. The remote will usually display 100% but its not really fully charged until the LED is off.
```

---
## \#676 Posted by: Deckoz Posted at: 2018-03-12T02:21:03.686Z Reads: 269

```
Was it connected to the board? Because searching for a signal is probably in full power mode on the NRF... as it is scanning the channels...

And I mean a green connection to the receiver...as I've had lots of ride hours with it connected, but also had it go dead on me sitting on the counter quickly when the board was unplugged and searching for signal...
```

---
## \#677 Posted by: scepterr Posted at: 2018-03-12T02:22:14.250Z Reads: 262

```
Nope transreceiver isn't connected
@Wajdi another thing to put a timer on 😋
Also when did switch to lcd happen?
```

---
## \#678 Posted by: Wajdi Posted at: 2018-03-12T02:24:09.161Z Reads: 255

```
I switched to lcd early in the development/prototype period, didn't see the daylight :stuck_out_tongue:
```

---
## \#679 Posted by: scepterr Posted at: 2018-03-12T02:25:56.805Z Reads: 249

```
Is it still compatible with an oled screen so if in the future an appropriately sized one becomes available it could be switched?
```

---
## \#680 Posted by: Wajdi Posted at: 2018-03-12T02:28:32.381Z Reads: 268

```
It can be, but depending on the new screen, we might need to change the pcb design a bit to support different pinouts. Software changes are also needed, OLEDs have different drivers than LCDs.
Average current consumption right now is about 110mA. Battery is 900mah, so in average we have around 6 hours continuous runtime, factoring in about 70-80% efficiency due to heat, peak transmission currents and other factors.
```

---
## \#681 Posted by: scepterr Posted at: 2018-03-12T05:11:19.879Z Reads: 283

```
Not sure if this is a known "feature"
You can change throttle direction by doing calibration backwards, push forward for back,pull back for forward
https://youtu.be/itgMpAJNuSQ

Remote coated, ready for use tomorrow 😛
![IMG_20180312_013245__01|690x232](upload://8ZBkckCMba2ZbLhZNapwOZX51N9.jpg)
(Make sure to mask screen if doing this, any fluid in the backlight will leave streaks)
```

---
## \#682 Posted by: ElskerShadow Posted at: 2018-03-12T08:42:55.969Z Reads: 269

```
I never done such a thing, maybe I should do it !
```

---
## \#683 Posted by: Mattmccrary8 Posted at: 2018-03-12T13:03:14.241Z Reads: 267

```
Do you know which one it is? I’m trying to order a pack
```

---
## \#684 Posted by: Mattmccrary8 Posted at: 2018-03-12T13:04:08.850Z Reads: 282

```
If your in a hurry to use it I can’t remember if it’s 2.0mm or 2.54mm

2.0mm 6pin
https://www.ebay.com/i/2628953986463

2.54mm 6pin
eBay4

10 SETS JST XH 2.54MM 6 Pin Female Double Connector with Flat Cable 200MM USA ...

10 SETS JST XH 2.54MM 6 Pin Female & Female Connector plug with Wires Cable 200MM. | eBay!
```

---
## \#685 Posted by: Wajdi Posted at: 2018-03-12T15:50:15.147Z Reads: 281

```
@scepterr Lol, I never thought about that :grin:, you just discovered a hidden feature, never anticipated someone would pull backward when it says push forward haha :smiley:
The coating looks clean!

@Mattmccrary8 the cable is JST PH 2.0 MM 6 Pin Female Double Connector.
```

---
## \#686 Posted by: Deckoz Posted at: 2018-03-12T16:32:46.691Z Reads: 288

```
Hey @Mattmccrary8 sorry man didn't see this. As wajdi said it's 2.0mm pins :)
```

---
## \#687 Posted by: Mattmccrary8 Posted at: 2018-03-14T10:12:01.229Z Reads: 287

```
A little preview for how bad ass this remote is. 

https://youtu.be/WOtFkFxEfj4
```

---
## \#688 Posted by: JasperM Posted at: 2018-03-14T11:46:46.297Z Reads: 285

```
Hey mate, Is there an update?

Not trying to be pushy, I just wanna start tinkering.

Cheers
```

---
## \#689 Posted by: danggilmore Posted at: 2018-03-14T19:45:20.286Z Reads: 289

```
@SkaterBoy58
@Deckoz

Can anyone help me with getting this bad boy to work? I've been working with @Wajdi but we're struggling to figure out why the remote isn't bringing throttle to my board. I'm running dual vesc 6 in foc sensored via canbus. I've attached pics of my vesc settings. The remote binds to the reciever and shows the green dot but won't relay any throttle to my motors nor show telemetry.

Was running 3.34 but updated 3.35 at Wajdi's recommendation. He says everything looks good and should work but it's not. :[

Appreciate any help I can get. 

![IMG_0202|666x500](upload://bClrzaEbXVwc1T7qesvXys9cYIf.JPG)![IMG_0200|666x500](upload://5JJ1fiPHMkuap1ZtlCqfFJsEsfo.JPG)![IMG_0201|666x500](upload://kNFxEIiMDzdgQl93VKdYseS5A7k.JPG)![IMG_0198|666x500](upload://cIfHqcukP9I9SrCz5OTgvav7WKP.JPG)![IMG_0199|666x500]
```

---
## \#690 Posted by: SkaterBoy58 Posted at: 2018-03-14T23:26:47.266Z Reads: 248

```
@danggilmore   both @Deckoz and myself tried the modified vesc 3.35FW with the remote about a week ago with no success - see posts above . Wajdi was going to look into it .

@Wajdi  -  Any update on your findings on your 3.35FW ?
```

---
## \#691 Posted by: Wajdi Posted at: 2018-03-14T23:49:24.557Z Reads: 241

```
He is using stock fw 3.35, not the modified one, because he has an updated receiver.
Regarding the old receivers, I suggest running 2.54, because so much has changed since then, and its hard to keep compatibility, newer receivers support FW 3.3x and up, but not lower.
```

---
## \#692 Posted by: Deckoz Posted at: 2018-03-14T23:53:10.700Z Reads: 248

```
So the real question is 

Post up the receiver firmware so we can update the receivers via AVR or ASP
```

---
## \#693 Posted by: Wajdi Posted at: 2018-03-14T23:56:05.682Z Reads: 245

```
Sure, you can update the firmware if you have a jtag programmer, you will also need atmel studio 7.
```

---
## \#694 Posted by: Deckoz Posted at: 2018-03-14T23:56:49.779Z Reads: 249

```
Have both on ✋
```

---
## \#695 Posted by: Wajdi Posted at: 2018-03-14T23:58:47.917Z Reads: 250

```
The programmer I use is SEGGER 8.08.90 J-LINK, I will post the firmware here shortly http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#696 Posted by: Deckoz Posted at: 2018-03-15T00:17:33.689Z Reads: 273

```
[quote="Wajdi, post:695, topic:24654"]
SEGGER 8.08.90 J-LINK
[/quote]

What chipset adapter are you using and/or the pinout for the jtag block header. I'm guessing the silk 1 is pin one on the right?

![1521072976467929336751|375x500](upload://dFIwNhT2lj25u8jnqiNqOm4JiJV.jpg)
```

---
## \#697 Posted by: Wajdi Posted at: 2018-03-15T00:19:01.506Z Reads: 263

```
Yes, silk 1 indicates pin 1 of the header.
```

---
## \#698 Posted by: Deckoz Posted at: 2018-03-15T00:21:03.212Z Reads: 263

```
[quote="Mattmccrary8, post:687, topic:24654, full:true"]
A little preview for how bad ass this remote is.
[/quote]

Nice dude. :)
```

---
## \#699 Posted by: Wajdi Posted at: 2018-03-15T00:57:09.279Z Reads: 270

```
Btw guys @danggilmore solved his issue, I'm putting this here so anyone with same issue knows the solution, it turned out VESC 6 has TX and RX pins swapped on the UART port, if anyone is using VESC 6 all you need to do is swap those two pins on the UART cable and you are good to go.
```

---
## \#700 Posted by: danggilmore Posted at: 2018-03-15T00:57:40.664Z Reads: 261

```
@Wajdi is the man! spent hours with me working through this. what a boss! :]
```

---
## \#701 Posted by: caustin Posted at: 2018-03-15T03:20:12.454Z Reads: 272

```

http://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483/784
```

---
## \#702 Posted by: ElskerShadow Posted at: 2018-03-15T09:09:20.593Z Reads: 285

```
![image|375x500](upload://plGhL8MnD5yyebXDxE5C0vffuZz.jpg)
After months of struggle the remote works, it worked in 1,5 sec with the new reciever @Wajdi so it was indeed hardware related
```

---
## \#703 Posted by: Wajdi Posted at: 2018-03-15T14:57:42.917Z Reads: 272

```
Glad you got it working finally.
```

---
## \#704 Posted by: scepterr Posted at: 2018-03-17T20:37:03.651Z Reads: 268

```
Wait so we're using tx/rx not sda/scl?
```

---
## \#705 Posted by: banjaxxed Posted at: 2018-03-17T20:58:41.322Z Reads: 274

```
interesting read here on the different types, I like the sound of silicone due to it's ability to handle temps(PU is a heat blocker?) it's ability to keep water out and the lack of any mechanical stress on the pcb

 although must admit no experience with any of these
http://news.ewmfg.com/blog/which-type-conformal-coating-right-my-pcb
```

---
## \#706 Posted by: scepterr Posted at: 2018-03-17T21:08:52.697Z Reads: 262

```
I can't say I've ever observed any noticable heat increases and I don't coat heatsinked components
```

---
## \#707 Posted by: banjaxxed Posted at: 2018-03-17T21:11:03.370Z Reads: 262

```
Yeah see the masking for fets, presumably keep off their pins too which also get hot hot
```

---
## \#708 Posted by: scepterr Posted at: 2018-03-17T21:12:56.901Z Reads: 255

```
Yeah I just try to seal around the fets externally
```

---
## \#709 Posted by: banjaxxed Posted at: 2018-03-17T21:15:04.023Z Reads: 254

```
Looks like a good idea until a pick, scratch and drv change is needed, hopefully these ESCs don't suffer from that, I'm gonna try it thanks for the pics
```

---
## \#710 Posted by: scepterr Posted at: 2018-03-17T21:16:11.359Z Reads: 251

```
Lol well the idea is to give it the best chance of not failing at the start so you won't have to dig into it later 😉
```

---
## \#711 Posted by: DrJeff Posted at: 2018-03-18T02:13:35.084Z Reads: 242

```
I've used silicone conformal spray for other boards that I keep outside!
But just a lacquer would probably work ;)
```

---
## \#712 Posted by: ElskerShadow Posted at: 2018-03-18T09:41:56.511Z Reads: 250

```
To all the owners of the photon, what do you plan to do in terms of lights ?
```

---
## \#713 Posted by: scepterr Posted at: 2018-03-18T10:18:06.362Z Reads: 257

```
Got the 144led/m strip and waterproof connectors, haven't decided exactly what I'm gonna do yet
Oh and 12v to 5v stepdown, already using a battery to 12v3a stepdown
```

---
## \#714 Posted by: ElskerShadow Posted at: 2018-03-18T10:20:59.769Z Reads: 258

```
So you don’t really care of the 1A max of the reciever ? You just use it for data ? And plug the 5v of the led strip directly to the buck converter plugged into the battery right ?
```

---
## \#715 Posted by: scepterr Posted at: 2018-03-18T10:22:35.358Z Reads: 257

```
Yeah don't use the 5v from the vesc, only from converter
```

---
## \#716 Posted by: ElskerShadow Posted at: 2018-03-18T10:24:51.620Z Reads: 259

```
Alright I was plannin to do that as well. Is there’s any buck converter recommended ? I have a 12S battery
My plan is to have front and rear lights + led strip in the middle. All powered thru buck converter and all soldered to reciever for data and turn on/off from remote. 
Making sure I understand everything
```

---
## \#717 Posted by: scepterr Posted at: 2018-03-18T10:30:50.860Z Reads: 278

```
https://www.amazon.com/dp/B016XI9BJS/ref=cm_sw_r_cp_apa_V9JRAb5ABACYH
 
https://www.amazon.com/dp/B00CGV5NT4/ref=cm_sw_r_cp_apa_T8JRAb3PEXRZH
2pin DC for front/rear, 3pin small for ws2812

https://www.amazon.com/dp/B01EMFIW62/ref=cm_sw_r_cp_apa_W6JRAbTQ6TZRK
```

---
## \#718 Posted by: scepterr Posted at: 2018-03-18T22:38:03.156Z Reads: 282

```
So my photon fell off a desk while charging and this happened 😐
![IMG_20180318_183641__01|690x447](upload://km0M1fbTUVtOnIaehnmQJg5Ul5N.jpg)

I notice the rear support pins are not soldered 🤨

@Wajdi you need to update the original post to reflect what's in the remote, the PCBs you have posted at the top, have all the USB support pads, this PCB does not
![IMG_20180318_184651|444x500](upload://70MTh5QfO3Ko9jIletP9GjigVif.jpg)
If it was left with all the pads it wouldn't break with one drop

The current USB port is held on by 2 support pins in front and just the USB pins at the back, that's not acceptable
```

---
## \#719 Posted by: Wajdi Posted at: 2018-03-18T23:50:21.459Z Reads: 263

```
@scepterr Oups, sorry this happened to you :neutral_face: seems like it took a hit at it’s weakest spot. 

That first micro usb on the prototype pcb was unfortunately out of production, the best alternative I could find was this one. If anyone can find a good micro usb with better support pins please let me know.
```

---
## \#720 Posted by: scepterr Posted at: 2018-03-19T00:02:18.444Z Reads: 273

```
This one has support pins and holes they go into, but no pad so can't be soldered
![IMG_20180318_200326__01|601x500](upload://AeD6Ak2KmEy3Drq1S7j7lTyB2tN.jpg)
```

---
## \#721 Posted by: fedestanco Posted at: 2018-03-19T00:04:12.693Z Reads: 265

```
The one on diebiems is very strong. And you can find the footprint ready to go on github
```

---
## \#722 Posted by: scepterr Posted at: 2018-03-19T00:06:04.963Z Reads: 260

```
I'll be able to fix it and epoxy it down myself, but this will be a very common issue if not mitigated
```

---
## \#723 Posted by: Wajdi Posted at: 2018-03-19T00:18:41.045Z Reads: 261

```
@fedestanco I will check it out, thanks.
@scepterr  You are right, I will adjust the footprint to add pads on those rear pins.
```

---
## \#724 Posted by: Darklinks Posted at: 2018-03-19T03:08:25.305Z Reads: 259

```
@Wajdi I finally got the remote last week. So today I go and try to use turn on the remote but it’s stay frozen it does not change menu or anything. I try  powering of the Remote but it’s does not turn off as well
```

---
## \#725 Posted by: Wajdi Posted at: 2018-03-19T03:11:16.059Z Reads: 266

```
You can either unplug the battery and plug it back in again, 
Or download the flash updater from here http://eboardshop.net/product/photon-updater/
and V0.3 firmware from here http://forum.eboardshop.net/t/firmware-update-download/59
And re-flash it.
```

---
## \#726 Posted by: scepterr Posted at: 2018-03-19T03:29:31.131Z Reads: 290

```
Quick support fix using throughhole resistor leg
PCB should still be updated with pad there but this is something existing users could do. 
![IMG_20180318_232226__01|622x499](upload://kH4XIXoBKaAmjgkwvIx0QozTxN2.jpg)
![IMG_20180318_232340__01|573x499](upload://cfGS03RVZySDPtse7BFAS747UiF.jpg)
![IMG_20180318_232626__01|538x500](upload://uZG0iOAzqkvZQ841fob1HraMitd.jpg)

Just need to solder the support pin to the legs and it's secured
![IMG_20180319_000010__01|663x500](upload://bJM5tcn3jEhRTbhkg7dLRbIiqUK.jpg)

Oh and that middle support pin can easily be soldered to the pads right next to it
```

---
## \#727 Posted by: lazerusrm Posted at: 2018-03-21T11:31:13.719Z Reads: 262

```
Is there an ETA on orders? i've placed one late feb just curious. thx
```

---
## \#728 Posted by: Zigm4 Posted at: 2018-03-22T15:43:27.922Z Reads: 262

```
you are not the only one...
ETA should be 10 to 15 days as indicated on the website, but @Wajdi don't communicate a lot...
Mine was ordered on february 18th and still no remote :disappointed_relieved:
```

---
## \#729 Posted by: ElskerShadow Posted at: 2018-03-22T16:10:08.110Z Reads: 259

```
Don't worry mate, I waited like overall 5month for this and in the end it's worth it... It's not like you can't ride meanwhile, GT2B are cheap.
```

---
## \#730 Posted by: Wajdi Posted at: 2018-03-22T16:27:07.401Z Reads: 261

```
@lazerusrm @Zigm4 Sorry guys for the delays, all pending pre-orders will be fulfilled starting on Monday.
```

---
## \#731 Posted by: lazerusrm Posted at: 2018-03-22T17:36:20.178Z Reads: 270

```
yes I am riding anyway! have an alien remote that works great
```

---
## \#732 Posted by: ElskerShadow Posted at: 2018-03-24T11:17:43.191Z Reads: 276

```
![image|382x500](upload://fiAf3QO3DdRxRObEIb15niliMdz.jpeg)

Guys i have a little problem 
The remote is working fine i just can’t get a throttle response, motor don’t spin and no response in the BLDC tool a
But i have all the data on the remote fine
```

---
## \#733 Posted by: JLabs Posted at: 2018-03-24T11:19:40.951Z Reads: 263

```
Let’s see the motor config tab
```

---
## \#734 Posted by: ElskerShadow Posted at: 2018-03-24T11:29:58.251Z Reads: 271

```
![image|677x499](upload://pPxEJxRY211SLrnfoAKnmb23DPA.jpeg)
I typed faults in terminal and nothing 
I hooked up my gt2B as well on both vesc to try and I don’t have pulsewidth or throttle impulse either
```

---
## \#735 Posted by: JLabs Posted at: 2018-03-24T11:44:17.196Z Reads: 262

```
How about the next tab down on the left? I don’t see anything in the other tabs.

Also I did pick up that your cutoff voltages are mixed around. You will want to change them.
```

---
## \#736 Posted by: ElskerShadow Posted at: 2018-03-24T11:48:48.729Z Reads: 266

```
@Wajdi 
I have been riding for 3 consecutive hours and i have a few questions : 
• I have noticed the battery board percentage is not accurate at all, for example when i was at 66 % the remote was showing 7 % 
• the UI is a pain because A button is used for OK and it’s completely not convenient. As we said in PM’s replace the Ok function with the click of the joystick. It will be way quicker like that IMO. 
• i had a problem in the end of the ride, i couldn’t go more than 30 km/h, i checked the menu and the throttle percentage was at 100 % ( i was not overheating ) . Super Weird behavior, went hope checked 2 hours later and I had all the torque back.
```

---
## \#737 Posted by: lazerusrm Posted at: 2018-03-26T05:25:41.761Z Reads: 261

```
Can't Wait!
```

---
## \#738 Posted by: Acidfie Posted at: 2018-03-28T09:59:13.954Z Reads: 260

```
please check your ERPM Limits before frying your VESC
```

---
## \#739 Posted by: Acidfie Posted at: 2018-03-28T17:04:50.985Z Reads: 257

```
Also, anyone in EU up for a group buy? maybe germany?
```

---
## \#740 Posted by: notger Posted at: 2018-03-28T18:21:06.118Z Reads: 260

```
Hi, I'm interested in a group buy depending on the Endprice including toll, tax and shipping.

Greets from Austria

Notger
```

---
## \#741 Posted by: Acidfie Posted at: 2018-03-28T18:40:31.126Z Reads: 253

```
i think we can calculate about 200€ for this fucking toll, vat and shipping costs...
```

---
## \#742 Posted by: Wajdi Posted at: 2018-03-28T19:01:11.267Z Reads: 258

```
I'm offering 10% off for bulk orders of 10+ units, shipping is also flat rate, group orders can save on shipping as well because its one package only. 25$ for international orders. 
Group order of 10 units would save you 15.9$ + 22.5$ = 38.4$ off per remote. Assuming shipping cost will be divided equally.
```

---
## \#743 Posted by: uigiroux Posted at: 2018-03-28T19:50:00.693Z Reads: 263

```
Is it possible to order (for a extra fee) one of your remotes that is totally set up and pretty much plug and play.  Like we could tell you what ESC were going to be using and the details of motor and battery so it could a be properly setup, since I've heard it can be very difficult to not only pair the remote for basic function, but to get all the other benefits, ie telemetry, light switch, etc...?
```

---
## \#744 Posted by: Acidfie Posted at: 2018-03-28T20:07:28.864Z Reads: 252

```
wait, they are not plug and play?
```

---
## \#745 Posted by: uigiroux Posted at: 2018-03-28T20:11:07.239Z Reads: 254

```
Ugh... Well don't quote me, but I believe there is some work to be done to set them up for everything to work properly.  At least I think there used to be, it might have changed?
```

---
## \#746 Posted by: Zigm4 Posted at: 2018-03-28T20:12:33.792Z Reads: 255

```
Hi @Wajdi

Do you have an estimate delivery date for a group command (i might have some friends interested) ? :slight_smile:  
And an estimated delivery date for February commands ?

Thanks
```

---
## \#747 Posted by: uigiroux Posted at: 2018-03-28T20:20:28.807Z Reads: 243

```
Oh I want to get in on that group buy!  When are you guys planning on ordering..?
```

---
## \#748 Posted by: Wajdi Posted at: 2018-03-28T20:20:33.683Z Reads: 249

```
@uigiroux They are already plug and play, all new orders are compatible out of box with latest VESC firmware. The issues you were seeing are older receiver versions that are incompatible with new firmwares.
Also every remote is paired with its receiver before being sent out.
```

---
## \#749 Posted by: uigiroux Posted at: 2018-03-28T20:22:19.848Z Reads: 240

```
Oh ok perfect, glad that got sorted out! :smile:
```

---
## \#750 Posted by: Wajdi Posted at: 2018-03-28T20:22:41.787Z Reads: 247

```
@Zigm4 I'm trying to get all pre orders shipped out by the end of this week. They will have a new firmware v0.4 installed on them, that has new menu option to setup cell count, giving more accurate board percentage reading, and fixing several issues related to random boot up problems.
```

---
## \#751 Posted by: mmaner Posted at: 2018-03-28T20:24:40.531Z Reads: 247

```
Is the new firmware compatible with all VESC firmwares?  Is there a version to version compatibility chart if not?  I've got 1 of the remotes, waiting on the second, I assume that will ship out with this batch...great remote and great work @Wajdi.
```

---
## \#752 Posted by: Wajdi Posted at: 2018-03-28T20:28:46.750Z Reads: 246

```
@mmaner Yes your remote will be shipped out with this batch.
New receivers are compatible with any VESC FW.
```

---
## \#753 Posted by: mmaner Posted at: 2018-03-28T20:29:54.742Z Reads: 240

```
Awesome, glad to hear it.  Im sticking with @Ackmaniac 2.54 on all of my Vesc4's, so just wanted to be sure.
```

---
## \#754 Posted by: JasperM Posted at: 2018-03-28T22:18:01.506Z Reads: 237

```
Hey there @Wajdi, is my remote in that order?
```

---
## \#755 Posted by: Zigm4 Posted at: 2018-03-28T22:21:12.978Z Reads: 239

```
I think all ours will be in that batch, isn't it @Wajdi ?
My address will change end of april, i guess i will got mine before :wink:
```

---
## \#756 Posted by: ElskerShadow Posted at: 2018-03-29T07:22:34.453Z Reads: 259

```
@Wajdi
There’s one thing that is killing the remote for me, the throttle. I’ve been using the remote daily for a week now and I just can’t feel safe with it. ( no disconnections whatsoever ) 
For example when I am 20 km/h I have to push the joystick up and it will not accelerate before The joystick reaches a certain height. The faster you go the furthest you need to accelerate again. IT’S THE MOST DANGEROUS THING EVER EVER EVER ! I almost crashed 3 times in a week ONLY because of that because there’s a delay when you start to push the joystick and the height it will be effective. 
PLEASE @Wajdi fix that or explain me a way if I can change that in the settings because I am not confident at all riding because of that + the deadband is as well too large for me, not responsive enough.
The slightest push should result in acceleration whatever the speed.
I mean on the GT2B for instance even if i’m 60 km/h even the slightest pull on the trigger will make me accelerate when with the photon i would have to push the joystick to at least 90 % throttle to get more acceleration. 
IMHO it’s the nicest feature if you wan’t peoples do die riding with the remote, i remeber evolve had the same system. Haven’t you heard everyone hates evolve remotes ? 
Meanwhile i keep using the old 25 € GT2B.
```

---
## \#757 Posted by: bevilacqua Posted at: 2018-03-29T07:59:03.705Z Reads: 237

```
do you use acks fw on both?
```

---
## \#758 Posted by: ElskerShadow Posted at: 2018-03-29T08:10:31.983Z Reads: 249

```
I don’t use acks 
I’m on 3.55 FW
```

---
## \#759 Posted by: bevilacqua Posted at: 2018-03-29T08:29:00.293Z Reads: 245

```
I thought that it maybe was because of the Watt Control feature... 
Lets hope you can solve it!
```

---
## \#760 Posted by: ElskerShadow Posted at: 2018-03-29T09:12:47.478Z Reads: 247

```
I don’t actually know if throttle curve will change anything 
I will try tho
Other Photon owners have you noticed the same throttle response ? ( at X speed you need to go further X with the joystick before accelerating again, all the way before X will have no effect on throttle )
```

---
## \#761 Posted by: Wajdi Posted at: 2018-03-29T13:44:05.459Z Reads: 244

```
Thats a normal behavior, and I don't see anything wrong with, if not safer.
If even the slightest push to the throttle when at high speeds would increase the speed further, then thats what I see as dangerous. Photon will you a buffer play on the joystick depending on how fast you are going to avoid accidental pushes that will lead to crashes.

I don't really see why the acceleration joystick should be more sensitive at hight speeds because thats not safe at all. When going fast you need more stable control over the acceleration, not a jerky one small touch and you fly.

I'm sorry but your suggestion doesn't make sense to me. You can always adjust the throttle response on the BLDC tool, it should give you the results you are looking for, but that's just not safe in my opinion.
```

---
## \#762 Posted by: Ackmaniac Posted at: 2018-03-29T14:41:33.663Z Reads: 240

```
You mean when you are doing 80% speed then the first 80% of the trigger will be ignored?
```

---
## \#763 Posted by: Wajdi Posted at: 2018-03-29T14:48:16.345Z Reads: 240

```
When doing 80% of speed, the first 80% of throttle doesn't get ignored, it might feel like it, but it's not, it does still deliver current to the motor, but not more than what you are currently using.
If you are doing 80% of speed, and give only 40% throttle, your speed will slowly slow down until you get to cruising speed to 40%.
```

---
## \#764 Posted by: Ackmaniac Posted at: 2018-03-29T14:57:59.747Z Reads: 242

```
Adn what happens when you go 40% speed and give only 40% throttle. Will it keep that speed even when you go up or down a hill?
```

---
## \#765 Posted by: Deckoz Posted at: 2018-03-29T15:06:58.911Z Reads: 238

```
Throttle works/feels the same as my ppm nano remote. So not sure what the fuss is about.
```

---
## \#766 Posted by: Wajdi Posted at: 2018-03-29T15:10:04.113Z Reads: 243

```
If you have cruise control activated then yes, giving 40% throttle will keep you cruising at 40% speed even when going uphill or downhill.
```

---
## \#767 Posted by: Ackmaniac Posted at: 2018-03-29T15:43:31.425Z Reads: 238

```
Not talking about cruise.
Does 40% throttle result in 40% motor amps or 40% speed?
Or in other words, does 40% throttle simulate 40% ppm throttle signal to the vesc or does your remote calculate the ppm signal based on speed?
```

---
## \#768 Posted by: ElskerShadow Posted at: 2018-03-29T18:31:07.236Z Reads: 242

```
[quote="Wajdi, post:763, topic:24654"]
When doing 80% of speed, the first 80% of throttle doesn’t get ignored, it might feel like it, but it’s not,
[/quote]
That’s how I feel, i feel like it’s completely ignored. 
I think it’s not safe because if i need to accelerate i don’t really know at wich point it will push the throttle.  
So it’s hard to anticipate the acceleration. 
For me it’s safer if you can have full control at any speed without any deadzone on the remote except the middle point, at any given time. 

I’m trying to be as clear as possible but my english is limited. What I say is not nonsense
```

---
## \#769 Posted by: mmaner Posted at: 2018-03-30T13:58:01.208Z Reads: 236

```
Every remote I've ever used behaves this way, I really can't figure out what your looking for but I'm fairly certain it doesn't exist.
```

---
## \#770 Posted by: ElskerShadow Posted at: 2018-03-30T14:59:42.226Z Reads: 235

```
The GT2B does not work like that and is kind of the standart for years
Or even the nano remote, or the nano- X
```

---
## \#771 Posted by: Deckoz Posted at: 2018-03-30T15:05:20.428Z Reads: 251

```
Do you have deadband set on both the remote AND the esc?

As I highly recommend turning deadband on the remote off completely, and running max sensitivity - max sensitivity and no deadband on the remote translates to direct input like the nano/mini. I know what you mean..I felt the same at first. But I think I made a post about this delayed engagement feeling Early in this thread.

Setup throttle curves and deadband on the vesc and set the remote to be setup for direct input.

Let me know @ElskerShadow
```

---
## \#772 Posted by: Wajdi Posted at: 2018-03-30T15:11:02.051Z Reads: 239

```
Just to add to what others suggested, sensitivity option was removed in FW 0.2 and up, and input is direct since then.
```

---
## \#773 Posted by: mmaner Posted at: 2018-03-30T15:20:09.770Z Reads: 242

```
I guess I don't understand what you are saying.

On my Nano-X if I am 30% into the throttle and I let off, then re-apply the throttle I have to get back to the speed at which Im currently at before I 'feel' a response from the throttle.  I probably didn't say that very well, but I'm just really having a hard time understanding what your asking.
```

---
## \#774 Posted by: Deckoz Posted at: 2018-03-30T15:21:37.163Z Reads: 245

```
This makes a world of difference.


Now as long as your not double deadbanding you should be fine @ElskerShadow
```

---
## \#775 Posted by: Toughook Posted at: 2018-03-30T15:58:17.655Z Reads: 249

```
Just to ask about pre orders; I only ordered mine about two weeks ago, are you saying that mine might be one of those shipped (to UK) or is there a stepped system of order batches, from certain cut off points? Just asking , I'm patient 😁
```

---
## \#776 Posted by: Wajdi Posted at: 2018-03-30T18:19:17.104Z Reads: 275

```
Yours will probably be included in this batch as well, I have enough parts to cover all current pre orders.

On the same note, check out the new PCBs, this time they are milky white, and they look so cool 

![image|666x500](upload://8GaLUOt3ugVnDyQC5ERLh7n01Dc.jpeg)![image|666x500](upload://lkg6XcjLnSTwP9iCqWaqfCvtsbY.jpeg)![image|666x500](upload://6ln4yqsiYgdfWqfRhSFs7KLHKtU.jpeg)![image|666x500](upload://mdhTR5Pm4iTNkzSi9CjoI5NJ7IL.jpeg)
```

---
## \#777 Posted by: scepterr Posted at: 2018-03-30T19:19:30.637Z Reads: 264

```
Looks nice, though I noticed there's still no pads on the support holes for the microusb
```

---
## \#778 Posted by: Wajdi Posted at: 2018-03-30T19:30:26.990Z Reads: 264

```
Thanks, those pcbs were ordered before we discussed the pads.
```

---
## \#779 Posted by: lazerusrm Posted at: 2018-03-31T03:41:18.724Z Reads: 260

```
no worries anyone can fix! :) I ordered mine late feb.. can't wait!!!!! :)
```

---
## \#780 Posted by: lennylogs Posted at: 2018-03-31T19:28:43.320Z Reads: 260

```
Hey @Wajdi - I tried hooking up the remote last night and it wasnt connecting to the vescs. By “tried hooking up the remote” i mean i literally just plugged it in to the vesc and turned it on. 

So I’m sure I’m just skipping a very basic step(s) of setup, but do you have some sort of a step-by-step setup guide to follow?
```

---
## \#781 Posted by: Wajdi Posted at: 2018-03-31T20:18:48.117Z Reads: 252

```
@lennylogs Can you show me a picture of your connection?
```

---
## \#782 Posted by: RedEagle Posted at: 2018-03-31T23:32:16.351Z Reads: 266

```
https://www.electric-skateboard.builders/t/eu-group-buy-photon-remote/50814/
```

---
## \#783 Posted by: Zigm4 Posted at: 2018-04-03T13:50:10.273Z Reads: 259

```
@Wajdi : Super Painfull guy (me) is back , can i get an update on our batch please ?  :smiley:
```

---
## \#784 Posted by: advongunten Posted at: 2018-04-03T19:16:33.870Z Reads: 272

```
Hi everone!
I've got two photons, one with a quick discharging battery.
I'm charging both of them until orange led went out (both remotes powered off bytheway).
If I power Photon #1 on after a week it says 86%, acceptable.
The second one, after the same one week... the battery discharges down to 6%! :astonished:

Anyone some ideas/same problem? @Wajdi ?

Until now i haven't opened the remotes, because i'm hoping its just some software-related bug.
But meanwhile i think its a) a bad battery or b) the circuit of the photon is sucking too much current while on standby, because the remote is always on standby or on (as i understand it) there is now on/off switch to physicaly disconnect the battery.
Maybe thats an idea for further versions?
If I don't use the remote over the next wintertime, lets say 3-4 month, should it always be plugged in all the time..?

Thanks and have a nice one
```

---
## \#785 Posted by: LEE Posted at: 2018-04-05T04:14:42.521Z Reads: 263

```
I ordered Photon last December.
Will it arrive soon enough?
```

---
## \#786 Posted by: Wajdi Posted at: 2018-04-07T03:20:00.251Z Reads: 260

```
Hey guys, sorry I was away for a couple days, but I'm back now. I'm in the process of shipping out the packages, keep an eye on confirmation emails.
```

---
## \#787 Posted by: SuperBen Posted at: 2018-04-07T23:12:53.348Z Reads: 258

```
If I ordered a Photon today when could I expect it to be delivered? :slight_smile:
```

---
## \#788 Posted by: Minim Posted at: 2018-04-08T06:56:05.311Z Reads: 260

```
What's the lead time if ordering now?
```

---
## \#789 Posted by: lennylogs Posted at: 2018-04-08T19:44:40.328Z Reads: 264

```
Hey @Wajdi sorry for the slow reply - heres a photo of the connection. The green light on the receiver is on but the motors dont spin. They work fine with my maytech remote so i feel like im just not connecting the photon remote properly 

![image|375x500](upload://tbIu3hBdGGDgPQWTqd1u9WhmNsT.jpeg)![image|375x500](upload://yUNyiV5EYBGd3fgeChR0g086vhc.jpeg)
```

---
## \#790 Posted by: Wajdi Posted at: 2018-04-09T16:57:04.803Z Reads: 251

```
@lennylogs
You bought two receivers right? If I remember correctly, I have setup one receiver as master, and the other as slave for your convenience. Please confirm and I will show you how to rebind.

@SuperBen @Minim Lead time right now is less than a week, I just shipped most pre-orders, and still have extra parts.
```

---
## \#791 Posted by: lennylogs Posted at: 2018-04-09T17:01:36.892Z Reads: 245

```
No - just one receiver. Maybe it still needs to be rebinded/rebound?
```

---
## \#792 Posted by: Wajdi Posted at: 2018-04-09T17:06:15.827Z Reads: 241

```
Ok, I sent you a PM.
```

---
## \#793 Posted by: SuperBen Posted at: 2018-04-09T17:37:40.058Z Reads: 247

```
Thanks for getting back to me :) 

One week thats not bad at all. I was interested back in December but waited to start my build. Seeing that guy who posted this week who has been waiting since December was throwing me off.

Order placed!
```

---
## \#794 Posted by: Wajdi Posted at: 2018-04-09T17:58:19.246Z Reads: 242

```
Thanks for your order, Lee’s order was placed in March, I don’t why he said December :smile:
```

---
## \#795 Posted by: SuperBen Posted at: 2018-04-09T18:16:53.728Z Reads: 247

```
Hahaha

Awesome man thanks! The Photon wait had me going down the rabbit hole last night, I was thiiiiis close to investing in a 3D printer and everything lol

Very excited to see this bad boy in action, been following this thread for 4-5 months
```

---
## \#796 Posted by: lazerusrm Posted at: 2018-04-09T18:55:05.200Z Reads: 241

```
Do you have updates for orders placed late February? I'm excited to receive mine Order: ES-252 Date: Feb26 - 2018. 

Thx!
```

---
## \#797 Posted by: Wajdi Posted at: 2018-04-09T19:08:51.042Z Reads: 239

```
I sent you tracking number earlier today, let me know if you have received it.
```

---
## \#798 Posted by: Minim Posted at: 2018-04-09T20:47:45.575Z Reads: 241

```
I see some posts here about weird throttle response. Is this only a minority that are on that side? Any user reviews out there?
```

---
## \#799 Posted by: Toughook Posted at: 2018-04-09T20:53:34.530Z Reads: 244

```
Very much looking forward to receiving mine 😁 My build starts in earnest this week so hoping to bypass installing the Maytech remote that came with my original parts list. Still I can use it for a back up, or second board 😂😂
```

---
## \#800 Posted by: lazerusrm Posted at: 2018-04-09T21:03:18.932Z Reads: 241

```
Wajdi - Did not receive it, i checked my spam folder as well. Dang! Thanks for looking into it.
```

---
## \#801 Posted by: Wajdi Posted at: 2018-04-09T21:10:42.788Z Reads: 247

```
@lazerusrm I sent you PM.
@Minim Throttle works the same as any standard remote, except it has more range, better accuracy, and fast response thanks to it's 32bit MCU.
```

---
## \#802 Posted by: LEE Posted at: 2018-04-10T02:25:52.041Z Reads: 242

```
I received the tracking number.
It is troublesome to check the voltage with the smartphone, but this is also the end.
I am looking forward to it!
```

---
## \#803 Posted by: Jreamer Posted at: 2018-04-10T02:43:28.439Z Reads: 236

```
Invoice ID: ES-232

Been patiently waiting for this remote. Whats going on?
```

---
## \#804 Posted by: Wajdi Posted at: 2018-04-10T02:46:58.618Z Reads: 232

```
@Jreamer I sent you tracking number today along others, let me know if you didn't receive it.
```

---
## \#805 Posted by: Jreamer Posted at: 2018-04-10T02:47:52.586Z Reads: 231

```
Ah it was in the spam.
```

---
## \#806 Posted by: Wajdi Posted at: 2018-04-10T02:48:21.359Z Reads: 234

```
Yep, this happens a lot :smile:
```

---
## \#807 Posted by: lazerusrm Posted at: 2018-04-10T03:14:01.912Z Reads: 233

```
Thanks Wajdi, can't wait to try it out, though i'm a bit scared, as my board is very very powerful. Will have to detune for a bit :)
```

---
## \#808 Posted by: Toughook Posted at: 2018-04-10T10:44:44.814Z Reads: 249

```
just went onto your website, logged on with my username and PW and then to My Orders. It shows that I don't have any order history yet I did purchase on 14th March @ 20:20:57 GMT Paypal Transaction ID :  5NE830395T766474W  	

Is there a problem with the account history on your site? Hopefully I shouldn't be too concerned, but could you please PM me with confirmation that you actually received my order. The money has definitely left my Paypal account !! 

Cheers
Tony
```

---
## \#809 Posted by: Wajdi Posted at: 2018-04-10T12:59:30.251Z Reads: 247

```
Hi Tony,

Your order was received, I replied to your email with details, let me know if you still have a question.
```

---
## \#810 Posted by: Zigm4 Posted at: 2018-04-11T16:18:54.696Z Reads: 255

```
Hi @Wajdi,

The tracking code is still in "Pre-Shipment" status (since two days). I've called the transporter and they told me they don't have the package yet... i'm pretty confused... :confused:
When do you plan to send them ?

Thanks ! :)
```

---
## \#811 Posted by: Wajdi Posted at: 2018-04-13T22:19:01.513Z Reads: 256

```
Packages were sent today.
They have the new Photon v0.4 firmware with the following new features:

* Added auto off option - can choose a timeout in minutes of inactivity before the remote self shutdown.
* Display brightness control - can be used to increase or decrease the display brightness, useful if you are riding at night and want to save battery.
* Power save mode - Can be tuned on and programmed to a certain percentage, if its set to 30% for example, once the remote reaches 30% of battery, it will automatically dim the display.
* Menu interactions are now done using the middle joystick button, Button A now only opens and closes menu.
* Improved power consumption during sleep.
```

---
## \#812 Posted by: lazerusrm Posted at: 2018-04-14T00:49:16.458Z Reads: 239

```
Confirmed, mine shows up monday, wahoo!
```

---
## \#813 Posted by: lazerusrm Posted at: 2018-04-16T18:43:06.974Z Reads: 245

```
Recieved my remote.

Tried to power it on and am stuck with a blank white screen. what gives? I'll try updating the firmware tonight

edit: cant find .4 firmware.  ugh

Edit edit: Tried .3 .. FW updatet worked, screen is blank. gonna have to send it back, unless I can fix it? PM sent. :(
```

---
## \#814 Posted by: Wajdi Posted at: 2018-04-18T00:48:33.685Z Reads: 238

```
I replied to your PM, sorry this is happening to you. I would be happy to take it back and replace it asap.
```

---
## \#815 Posted by: lazerusrm Posted at: 2018-04-18T01:18:30.039Z Reads: 237

```
Thanks wadji for getting back to me quick 👍
```

---
## \#816 Posted by: lazerusrm Posted at: 2018-04-18T03:55:25.391Z Reads: 238

```
UPDATE:  I was able to repair the remote myself. The pin header on the display to the main PCB needed a bit more flux and solder, and came right on. YAY

I also added a bit of double sided tape to the other end of the display to reduce vibration fatigue on the pin header. perhaps a suggestion for future remotes.
```

---
## \#817 Posted by: quack3r Posted at: 2018-04-18T04:29:28.111Z Reads: 245

```
I'm having the same no throttle response issue you had. What did you do to fix it?
```

---
## \#818 Posted by: lazerusrm Posted at: 2018-04-18T12:14:44.589Z Reads: 255

```
Okay, i'm stuck again.

Setup:
12S
Dual Vesc6
Ackmaniac 3.1 Firmware

Finally found pins for binding after messing with firmware. 

Remote is on .4 now (verified in settings)
Reciever is connected to bottom pins of VESC6 (top two adc pins left disconnected)
baud rate set to 115200, all control modes removed, control mode set to uart and nunchuck set to "Current"

reciever has a solid orange light, nothing else
controller shows no data.

i tried swapping the rx/tx pins on the cable, nothing. i tried the slave vesc6 with the same settings, nothing

do i have a bad receiver too? I've streamed data to my phone using uart and a bluetooth module, so i know the serial port works when set properly.

It'd be nice to have a reference what the LED's mean, and an updated pinout on the website for the different receiver revisions.

thanks!
```

---
## \#819 Posted by: Wajdi Posted at: 2018-04-18T13:40:56.373Z Reads: 243

```
[quote="lazerusrm, post:818, topic:24654"]
Ackmaniac 3.1
[/quote]

Ackmaniac Fw is unfortunately not supported :slightly_frowning_face: You can use the latest official vesc firmware to get it working.
```

---
## \#820 Posted by: lazerusrm Posted at: 2018-04-18T14:24:51.667Z Reads: 232

```
Ah. Ok. Will try this and report back.
```

---
## \#822 Posted by: lazerusrm Posted at: 2018-04-18T14:40:19.575Z Reads: 253

```
it's not working for me, i'm getting no data to the remote, and an solid orange led.

EDIT: Vesc6 works with the .91 firmware from vesc-project.com  - I also looked through this thread again, and noticed this is posted earlier in the thread. Perhaps this info could be added to the main website for reference?

Steps for resolution:

Follow all original instructions for connecting the remote.

Swap the RX and TX pins on one side of the JST Connecttor using a tool (or a small knife or screwdriver) to lift the plastic retaining tabs.

Finally :)
```

---
## \#823 Posted by: lazerusrm Posted at: 2018-04-18T20:42:42.997Z Reads: 246

```
So, I have another issue. I have an orange light when I plug the remote in, and while it was charged, it would say charging... but... its not charging and now it's dead. what would cause it not to charge? I plugged it in overnight when I first got it.. once I fixed the screen, it only showed 9% charged, I figured it might be a big or something... not sure where to look now :confused:
```

---
## \#824 Posted by: LEE Posted at: 2018-04-18T21:16:12.562Z Reads: 244

```
Hi @Wajdi,

The tracking code is still in “Pre-Shipment” status. 
I’ve called the transporter and they told me they don’t have the package yet… i’m pretty confused… :confused:

When do you plan to send them ?

Thanks ! :slight_smile:
```

---
## \#825 Posted by: Wajdi Posted at: 2018-04-18T21:31:05.825Z Reads: 243

```
@lazerusrm When you unplug the remote from charge, what percentage does it display? 
@LEE Tracking shows that it was delivered yesterday, can you PM me what tracking you have?
```

---
## \#826 Posted by: lazerusrm Posted at: 2018-04-18T22:27:24.560Z Reads: 247

```
Got it sorted. I left it plugged in, and it fully charged. The problem was the remote battery got low, and i think the mcu browned out, and got stuck, and would not turn on.

I had to desolder the battery from the remote and resolder it. It's working now and showing 100% battery, so it did charge it all the way. 

Just a bad set of circumstances. :slight_smile:
```

---
## \#827 Posted by: lazerusrm Posted at: 2018-04-18T23:54:47.323Z Reads: 242

```
So i guess i must be getting super unlucky or something. I got stranded 10 miles up a canyon after i took a break, and the remote auto powered off... Then when i turned it on again, it started to turn on, and then the screen went blank. It wont turn on now, i'm thinking i'm going to have to de-solder the battery again... seems to me like this thing really needs a hard power on-off switch. I'm gonna have to wire one in, that sucked!
```

---
## \#828 Posted by: Zigm4 Posted at: 2018-04-19T06:26:03.908Z Reads: 261

```
@LEE  Is it a copy/past of my previous comment ? ;)
@Wajdi : My package is marked as delivered (in the US) but i got nothing and i live in France. Could you tell me if it's normal ?

![Colis|230x500](upload://brnX8f4pLahU8W05p2q3q5yXzrU.jpg)
```

---
## \#829 Posted by: LEE Posted at: 2018-04-19T06:42:42.577Z Reads: 262

```
![image|295x500](upload://3Gk05gOL1yMNbxPy7VYa3ogWInK.jpeg)
It is still in this state...
```

---
## \#830 Posted by: lazerusrm Posted at: 2018-04-19T15:05:03.464Z Reads: 236

```
Mine was like that for a little while. I think Wadji is very busy, give him some time, I'm sure he will take care of you.
```

---
## \#831 Posted by: Wajdi Posted at: 2018-04-19T15:30:23.270Z Reads: 241

```
@Zigm4 For some reason they returned two of the international packages back to me. This is the first time this happens, I still don't know whats the reason, but I suspect a USPS error.
I will bring them back again to the post office and see what the fuss is all  about.

@LEE Can you PM your order number?

@lazerusrm I think I will start using hard switches as well on future models, sleeping mode isn't really cutting it on this remote.
```

---
## \#832 Posted by: Zigm4 Posted at: 2018-04-19T15:32:22.554Z Reads: 245

```
[quote="Wajdi, post:831, topic:24654"]
I will bring them back again to the post office and see what the fuss is all  about.
[/quote]

When will you be able to send it back ? :frowning:
And how long should it take to arrive at my place ?
```

---
## \#833 Posted by: Wajdi Posted at: 2018-04-19T15:33:30.086Z Reads: 247

```
I will drop them off today. I will update you about the estimated delivery date.
```

---
## \#834 Posted by: Zigm4 Posted at: 2018-04-21T17:25:27.830Z Reads: 250

```
Hi @Wajdi,
Tell me you sent the package yesterday/the day before as planned.
I can't believe i didn't reveive it yet...
```

---
## \#835 Posted by: Wajdi Posted at: 2018-04-21T19:49:43.839Z Reads: 249

```
@Zigm4 I dropped the box at USPS for the second time, they told me they forgot to stamp it that's why it was returned back to me.
This morning it was delivered to me AGAIN. I can't believe this, I'm going to take it back to USPS for the THIRD time, and see what went wrong. This is frustrating.
```

---
## \#836 Posted by: Zigm4 Posted at: 2018-04-21T20:09:56.302Z Reads: 244

```
Yes it's really frustrating.
I need this remote... If the next shipment is failing again, i'll cancel this order.
I'm waiting for news from you on tuesday please.

Thanks !
```

---
## \#837 Posted by: webst Posted at: 2018-04-22T05:36:51.826Z Reads: 244

```
[quote="Zigm4, post:836, topic:24654"]
I need this remote… If the next shipment is failing again, i’ll cancel this order.
[/quote]

:face_with_raised_eyebrow:
```

---
## \#838 Posted by: Mobutusan Posted at: 2018-04-22T22:23:33.375Z Reads: 252

```
@wajdi, I'm hoping you can help me. I picked up @deckoz remote, but I can’t seem to get this to bind. I updated the remote to the latest V.4 firmware, with the V.2 receiver connected to my single TB 4.12 VESC via UART, running Ackmaniac 2.54. In the BLDC tool I have UART app selected, baud rate at 115200 and current control selected in Nunchuk tab. I first set the remote to binding/searching, then short the two binding pads on the receiver, power up the board, get the blinking orange light, and no connection; just endless “searching” on the remote and the blinking orange light on the receiver. Even if I power up the VESC and remote in binding mode first, then bind/search on the remote, still no connection. I rebooted the VESC when I changed from PPM to UART, and wrote all my settings to the VESC. Any idea what I might be missing or doing wrong?
```

---
## \#839 Posted by: Wajdi Posted at: 2018-04-22T22:58:10.005Z Reads: 251

```
@Mobutusan I just added V0.4 for old HW http://forum.eboardshop.net/t/firmware-update-download/59
Let me know if it works for you.
```

---
## \#840 Posted by: Mobutusan Posted at: 2018-04-22T23:10:15.452Z Reads: 252

```
Cool, thanks! And just so I'm clear, is the V.2 receiver considered "old" hardware in this case? And is the V.1 receiver useable at all, or is it just vintage DIY paperweight status now?
```

---
## \#841 Posted by: Wajdi Posted at: 2018-04-23T00:07:38.086Z Reads: 253

```
The only difference between old and new receivers is the Fw they support. Old receivers will support vesc fw2.x while new ones support fw 3.x.
```

---
## \#842 Posted by: mmaner Posted at: 2018-04-23T01:13:49.655Z Reads: 259

```
Do the new ones support v2 FW as well or only v3?
```

---
## \#843 Posted by: zyphaz Posted at: 2018-04-23T19:13:09.276Z Reads: 266

```
What is considered "old hw", how do we identify?  I assume the 0.1 screen printing on the back of the remote's PCB?  

![image|480x500](upload://36XSHMi0xR1siDXBGQIgbrFZAIB.jpg)
```

---
## \#844 Posted by: lazerusrm Posted at: 2018-04-24T23:31:44.746Z Reads: 262

```
EDIT: Post updated to be more kind to Wadji's hard work. I Originally wrote a post after a near accident which could have ended my life. (Remote lost connection during braking coming to a 45mph street)

So after having this remote for a week... I don't want to make it sound terrible

I think it needs a bit more work before it should be considered ready for most people.

Mine arrived broken, i had to take it apart and re-solder it to get it to work. It constantly disconnects, screen still intermittently works, it constantly drops connection so i can't trust it.. Had to routinely take it apart to disconnect the battery and reconnect it for it to turn on... ugh. Also the receiver came with no case? I saw pictures of a 3d printed one. Perhaps publish your stl so we can print our own?

It is a cool concept but definitely going on the shelf until i can work with Wadji, and some revisions done to it.

Test your remote VERY VERY THOROUGHLY. An improperly working remote can KILL you.

I seriously want it to work so bad too. i love the concept, and it's probably 90% there.. It's just that last 10% that makes it completely worthless to me unfortunately.
```

---
## \#846 Posted by: lazerusrm Posted at: 2018-04-25T02:18:11.078Z Reads: 246

```
good for you, not everyone has had your experiences. I'm not slamming wadji or the project, but I am providing some warnings and criticism, which I think is fair.

there are others from my batch having some of the same issues., I hope it gets worked out.

And my warnings are real. An inconsistently working remote will kill you. I almost couldn't brake the other day and nearly went right out into a busy intersection
```

---
## \#848 Posted by: Deckoz Posted at: 2018-04-25T03:20:58.392Z Reads: 256

```
I wouldn't go that far either, mine was amazing on my vanguard. I just skate to fast and my thumb would get disoriented with the joystick going above 30 on the evo, since I'm mostly focused on the road. I'd end up pushing sideways instead of up and down lol. 

But on my vanguard that topped out at 31, and mostly was 18-25mph, it was the best thing ever. I didn't have to worry about Bluetooth connected to my phone to watch speed or mileage etc. 

It really has promise... If I was to suggest anything at all, it would be to change the joystick to a hall sensor lever(up and down only) with a left and right button to the sides of the lever for adjustment of settings.

And add a microusb port to the receivers, to make receiver updates, as vesc firmware matures, the ability for a user to plug in. A USB vs jtag would be 🤸

Wajdi has done a fantastic job so far. I know some user experience is gonna vary..but man, I never had a single drop out, even on the original receivers(no antenna).
```

---
## \#849 Posted by: lrdesigns Posted at: 2018-04-25T03:30:44.767Z Reads: 252

```
Nice to see some of the experienced guys coming to its defense.  

[quote="Deckoz, post:848, topic:24654"]
it would be to change the joystick to a hall sensor lever(up and down only) with a left and right button to the sides
[/quote]

This would make it safer in those oh shit situations. The 4 way throttle is one thing that weirded me out and kept my wallet from feeling lighter.
```

---
## \#850 Posted by: Deckoz Posted at: 2018-04-25T03:38:11.879Z Reads: 263

```
[quote="lrdesigns, post:849, topic:24654"]
oh shit situation
[/quote]

Haha might not even be oh shit. I like to ride with my hands behind my back, my arms don't extend for balance 97% of the time. My videos might not show it, Because I have to hold the GoPro stick.. but, anyway once I start getting above 30mph when I'm tucking, back of hands on my butt, I'm fine when standing, but as soon as my upper torso levers over into a tuck my thumb is just trying to move forward or backwards, which ends up being sideways 😂 lol. It's that thing where your brain thinks it's doing something but you can't see, it so it's all "feel". Not sure how to explain it. 

Tldr my thumb is dumb when I can't see it so when I go fast I need a fixed axis, because I have no self control.
```

---
## \#852 Posted by: zyphaz Posted at: 2018-04-25T12:50:42.863Z Reads: 270

```
It's quite possible there was a bad batch.  FWIW, I received mine about a week ago as well, and I've had the two of issues @lazerusrm mentioned in the thread.  

A) White screen, which we were told was due to bad connections cold joints to the display
B) Sleep bug requiring a disconnect/reconnect of the battery to power on

Total disclosure, I did reheat/wick/flux/resolder the display on Monday night after @Wajdi suggested to do so to fix A). Bench tested that night and Tuesday morning with no issues, it sat on my desk all day.

Tuesday night, I wrap up my day and think about going for a spin? Nope, won't boot.

C) Total non-boot/power-on condition even after removing the battery
D) Charging LED will not illuminate (running a meter to the battery shows there is voltage in the batt so it's not completely dead, so it could be just not charging if the batt is full?)

On the plus side, when it did power-on I had zero disconnect issues and having the telemetry on hand was beyond slick.  I still ran metr to my tablet for the historical telemetry, but leave the tablet in my backpack and rely on auto-start/stop.  That's another big plus since my phone runs > Android 8.0.
```

---
## \#853 Posted by: mmaner Posted at: 2018-04-25T13:01:37.692Z Reads: 254

```
:arrow_up: That's how you write a critique on new hardware...
```

---
## \#854 Posted by: Toughook Posted at: 2018-04-25T13:21:35.329Z Reads: 257

```
hi Wajdi,

there seems to be an issue with my account and the way I created one on your site. I created one with the _tony@_ address, but checked out and paid with Paypal with the _sales@_ address of same domain. When I log into My Account, which is the _tony@_ it shows no orders, but we both know, and I have the confirmation of purchase email from my _sales@_ address......... !!!

So, please could you tell me the current situation. I have no way of knowing when'if it's been shipped, and trying to log in your site with _sales@_ says 'no known account with this address'

Soz to be a pain, but I wouldn't ask if I could find the info myself :slight_smile:
Thanks
```

---
## \#860 Posted by: SuperBen Posted at: 2018-04-25T17:42:05.049Z Reads: 255

```
Well shit lol

Hopefully with this feedback the next batch can have these issues checked/tested before they go out. That's the beauty of feedback with new product designs that are being improved as they are built, the things going wrong get brought up and then fixes are implemented. 

@Wajdi I'd like to request my remote be checked for this stuff before it gets sent out please, as I do not think my order has shipped yet. Still excited to try out this remote, thanks :)
```

---
## \#861 Posted by: lazerusrm Posted at: 2018-04-25T17:43:46.845Z Reads: 255

```
I agree. I would recommend Wadji suspend orders untill he can look into the issues a bit and get them sorted.

I'm sure he is under immense pressure from people to get their remotes out asap, but i'm sure people will wholeheartedly understand that there might be a delay due to a few critical bugs.
```

---
## \#862 Posted by: zyphaz Posted at: 2018-04-26T02:28:47.562Z Reads: 275

```
[quote="zyphaz, post:852, topic:24654, full:true"]
Tuesday night, I wrap up my day and think about going for a spin? Nope, won't boot.

C) Total non-boot/power-on condition even after removing the battery
D) Charging LED will not illuminate (running a meter to the battery shows there is voltage in the batt so it's not completely dead, so it could be just not charging if the batt is full?)
[/quote]
Welp, the saga continues. Just got home from work and decided to try to power on my Photon and.... it powers on.  No changes, no fixes attempted, no putting it on the charger, just pushed the power button and it turned on.  

One odd thing happened though, the batt level on the top right keeps going from ~29% to ~74%, accompanied by the screen flashing on/off/on.
https://www.youtube.com/watch?v=eLboUol4xo4
```

---
## \#863 Posted by: lazerusrm Posted at: 2018-04-29T00:58:08.092Z Reads: 270

```
Mine does similar things, except my battery percentage worked correctly. (unit won't boot anymore, just get a white screen 99% of the time)

I'd put it on a shelf and wait for wadji to get some time for us
```

---
## \#864 Posted by: Zigm4 Posted at: 2018-04-29T08:03:59.638Z Reads: 283

```
Hi @Wajdi,

I’am completely dedicated to helping individuals build their businesses (by ordering innovative products), evolve the e-Sk8 community, and innovate regularly. But i really think you are facing problems and don’t want to communicate about them.

I ordered the “Universal Advanced VESC Remote Control (Photon)” remote on **February 18th, 2018**. On the website, it’s indicated the expected shipping date should be arount **2 or 3 week** after ordering. (Note : even today it’s indicated : “PRE-ORDER All Pre-order reservations are expected to ship in 2-3 weeks”).

On **April 29th, i still have no news about my order** or any problem you could face actually. If you need more time to send something that works (strong welds, no blank screen, no battery problems, ...), if you have problems that prevent you from working on orders or other things, tell us.

When you start an e-commerce, you must respect deadlines or communicate clearly if necessary.
In case you do not understand my impatience or annoyance, below you can see each communication we had.
<ul>
 	<li>On March 1st asks for news on the forum</li>
 	<li>On March 2nd asks for news on the forum
<ul>
 	<li>On March 2 messaged me back stating that this would be sent within 10 days</li>
</ul>
</li>
 	<li>On March 9th asks for news via PM
<ul>
 	<li>On March 9th messaged me back saying he was doing his best and that he planned to send it on Monday March 12th</li>
</ul>
</li>
 	<li>On March 12th asks for news via PM
<ul>
 	<li>On March 13th messaged me back stating that he is still working on</li>
</ul>
</li>
 	<li>On March 18th asks for news via PM
<ul>
 	<li>On March 19th messaged me back stating that he has just finished assembling it and that he only has a flash</li>
</ul>
</li>
 	<li>On March 22nd asks for news on the forum
<ul>
 	<li>On March 22nd messaged me back telling me that it would leave from Monday, March 26</li>
</ul>
</li>
 	<li>On March 28th ask for news via PM
<ul>
 	<li>On March 29th messaged me back via PM indicating that it's almost ready</li>
</ul>
</li>
 	<li>On March 28th asks for news on the forum
<ul>
 	<li>On March 28th messaged me back stating that this would be sent before April 1st</li>
</ul>
</li>
 	<li>On April 3rd asks for news on the forum
<ul>
 	<li>On April 7th messages me back indicating that a tracking code would arrive and that the packages were going to leave</li>
</ul>
</li>
 	<li>On April 6th raise via PM indicating that it starts to be long and not normal
<ul>
 	<li>On April 7th message back via PM stating that he had taken some day off and that it was almost ready</li>
</ul>
</li>
 	<li>On April 9th Tracking code reveived</li>
 	<li>On April 11th asks for news on the forum indicating that the tracking code is still in "Pre-Shipping" status
<ul>
 	<li>On April 14th messaged me back indicating that the parcels left the same day</li>
</ul>
</li>
 	<li>On April 19th asks for news on the forum indicating that my package is shown as delivered in the US but I live in France...
<ul>
 	<li>On April 19th messaged me back indicating that the package had returned home and that he would return it the same day</li>
</ul>
</li>
 	<li>On April 21st asks for news on the forum
<ul>
 	<li>On April 21st messaged me back indicating that he had sent it again and that he had still returned home</li>
</ul>
</li>
 	<li>On April 21st asks for news indicating that if I did not receive my order quickly I would cancel my order</li>
 	<li>On April 24th asks for news on the forum</li>
</ul>

**I reiterate my confidence and appreciation for your work.**
Thank you for taking the time to communicate clearly on the various problems and to give us fixing and shipping date.
```

---
## \#865 Posted by: LEE Posted at: 2018-04-30T22:03:36.528Z Reads: 266

```
If you change the item of A.OFF in the remote control setting menu, the power will turn off and the power will not turn on.
In my Photon the buttery wiring is soldered directly to the board.
```

---
## \#866 Posted by: Chase Posted at: 2018-05-02T22:39:31.290Z Reads: 265

```
Who has the company email for this? I have tried asking for a refund for weeks through wadji’s profile on here. Everything I send has been ignored. Every time he has responded it has been a lie. I can’t find an email on the site. Several days ago I received a tracking number despite asking several times for a refund. It still says it is in preshipment, so I would like to find a way to contact Wadji before this gets in route.
```

---
## \#867 Posted by: LEE Posted at: 2018-05-02T23:53:19.536Z Reads: 258

```
The concept is advanced and wonderful.
Please somehow fix the problem.
I will wait for that day.
```

---
## \#868 Posted by: Knives186 Posted at: 2018-05-03T02:43:55.268Z Reads: 261

```
contact@eboardshop.net
```

---
## \#869 Posted by: Chase Posted at: 2018-05-03T03:46:57.953Z Reads: 263

```
Thanks a lot. Got a refund within seconds. I guess for those of you that still have orders, use the email above to contact wadji.
```

---
## \#870 Posted by: Zigm4 Posted at: 2018-05-03T10:24:07.137Z Reads: 260

```
I sent an email earlier today, hopefully he will refund me as well...
@Chase, Wajdi sent you an email to confirm the refund ?
```

---
## \#871 Posted by: Chase Posted at: 2018-05-03T21:53:13.508Z Reads: 261

```
PayPal sent the refund almost instantly after I sent the email. I sent it to the email given above and 
eminentsoftworks@gmail.com
```

---
## \#872 Posted by: SuperBen Posted at: 2018-05-03T22:10:48.551Z Reads: 265

```
I got tracking info on the 30th but its still in pre-shipment.

I hope mine got checked for the issues others have been having. That would be a good thing to do before dropping the package off lol Very excited
```

---
## \#873 Posted by: Linny Posted at: 2018-05-04T02:50:42.521Z Reads: 263

```
Yep, i ordered around the same time as you. I wonder how long it'll actually take to the doorstep, my board is all ready and is just missing a remote!
```

---
## \#874 Posted by: LEE Posted at: 2018-05-05T01:33:42.563Z Reads: 266

```
I think that it is better to ship after resolving the problem firmly.
It is meaningless to receive the product in the condition of a defect.
There is no choice but to wait for Wajdi's correspondence.
```

---
## \#875 Posted by: Zigm4 Posted at: 2018-05-05T08:28:42.653Z Reads: 270

```
I got him by email. He told me he is busy actually and he don’t have time to connect on the forum. You should send him an email (he is replying quite fast).

Hopefully i’ll Get my remote one day (seems he sent it for the third time last week)...
```

---
## \#876 Posted by: Wajdi Posted at: 2018-05-09T23:53:53.417Z Reads: 274

```
Hey guys,
Sorry I was away for a while,
I didn't catch up on all inquiries yet, but I have an update to announce.
FW0.41 is now released

* Fixes White/Black screen problems
*  Permanently fixing boot up issues. 

I completely removed MCU sleep mode, and instead reducing power by putting the display and nrf modules to sleep. This fixes the boot up problem, at a slight cost of more power consumption during Off mode. The White/black screen issue was introduced on FW 0.4, it is now fixed on 0.41.

V0.41 is also release for older HW. Older HW is any PCB other than white color.
Firmware can be found here http://forum.eboardshop.net/t/firmware-update-download/59

Also All orders that received confirmation last week, will have this firmware already installed. I shipped some today and will ship the rest in the next few days.
```

---
## \#877 Posted by: LEE Posted at: 2018-05-10T08:30:47.607Z Reads: 257

```
Remote control has been restored by Ver 0.41.
good job!
```

---
## \#880 Posted by: craigthemachine Posted at: 2018-05-16T19:23:50.686Z Reads: 256

```
Well, I'm closely watching this product. It looks promising, once they comb out the few bugs and obviously improve the delivery timeframe.
```

---
## \#881 Posted by: alexmarin99 Posted at: 2018-05-19T19:29:34.787Z Reads: 265

```
Is there a link with a BOM and PCB design files?

I would like to build it myself, thanks.
```

---
## \#882 Posted by: Jps224psu Posted at: 2018-05-20T02:08:07.915Z Reads: 279

```
Ok so ive lost my mind. Spent like 4hrs trying to get remote to work w vesc6. Photon FW .4 vesc6 FW 3.38. Followed all the directions, when u say switch rx/tx pins assuming the cables which was done then switched back then back again. Binded and rebinded multipe times. Then the black screen issue. Took remote apart removed battery plugged back in and it booted. Then tried again and it didnt work. Decided to update to FW .41 on photon got that to work however it is no longer binded after update so i tried that and after FW upgrade it will no longer bind. Here is set up. Any help would be appreciated. ![image|281x500](upload://ptXDEw81nqheyv0Nne5ksH5NORA.jpg)![image|281x500](upload://egpQKCwqB8Lhu7Wm7Wi71KIDuRn.jpg)
```

---
## \#883 Posted by: timbo_1233 Posted at: 2018-05-20T02:46:58.634Z Reads: 260

```
Oh yeah na that aligator clip you are using to hold the receiver is probebly shorting a couple components out ://
```

---
## \#884 Posted by: Jps224psu Posted at: 2018-05-20T02:53:41.311Z Reads: 263

```
It doesnt clamp very well and its only touching the 2 pins i used it on fw .4 and it worked 3x successfully.
```

---
## \#885 Posted by: Wajdi Posted at: 2018-05-20T03:06:22.675Z Reads: 270

```
Here is what you need to do to get this working:
1.Swap Tx and Rx pins on one end only of the cable
2. Use PhotonFW4.1r.bin  http://forum.eboardshop.net/t/firmware-update-download/59
3. Everything should work fine.
```

---
## \#886 Posted by: Jps224psu Posted at: 2018-05-24T01:47:19.261Z Reads: 265

```
Hey wajdi,

Last night remote was at ~93%. I turned it off and unplugged it from usb. Wnent out to garage today to grab and take a spin it was at ~9%. I plugged in it jumped to ~22% immediately....went on a 2 mile ride came back it was at ~17%. Any idea whats going on there? 

Thanks
```

---
## \#887 Posted by: Wajdi Posted at: 2018-05-24T02:33:14.264Z Reads: 263

```
Hey Jps224psu,
Battery lifetime will be improved in V0.42, I temporarily disabled sleep mode to fix some boot up issues, however I will restore it soon and battery lifetime will be extended.
```

---
## \#888 Posted by: Wajdi Posted at: 2018-05-25T18:47:53.232Z Reads: 255

```
New FW update 0.42 now available. Restored sleep mode, reducing power consumption significantly. http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#889 Posted by: JasperM Posted at: 2018-06-12T02:19:23.457Z Reads: 245

```
Hi guys,

I am finnaly trying to use my Photon that arrived a little while back.
I have downloaded the updater but when I try to run the .exe it says that I am missing VCRUNTIME140.dll and MSVCP140.dll. My computer runs these two error messages twice and says that reinstalling the program may help.
I just extracted the folder to my desktop. Where can I get these two .dll files?
```

---
## \#890 Posted by: Wajdi Posted at: 2018-06-12T02:31:09.144Z Reads: 243

```
What Ver. does it show on the remote menu? Chances are you already have the latest firmware.
If not, to solve your problem you need to download the Visual C++ Redistributable for Visual Studio 2015 from here https://www.microsoft.com/en-us/download/details.aspx?id=48145
```

---
## \#891 Posted by: JasperM Posted at: 2018-06-12T02:48:53.881Z Reads: 246

```
It says Ver. 4.

Also I seem to have flicked something in the menu and now the screen is black when plugged into my computer, I have not yet powered on my board with the receiver.
```

---
## \#892 Posted by: Wajdi Posted at: 2018-06-12T02:50:53.654Z Reads: 244

```
Update to v0.42 and let me know if you encounter any difficulties.
```

---
## \#893 Posted by: JasperM Posted at: 2018-06-12T02:56:56.934Z Reads: 243

```
I downloaded it but it says I already have it and that I should remove the old version, I did a search and have 16 visual C++ from 2005 through to 20015.
should I remove all of them and install the one that you lined to?
```

---
## \#894 Posted by: Wajdi Posted at: 2018-06-12T03:00:06.519Z Reads: 238

```
You don't necessarily need to remove all of them, just install the 2015 one, also make sure you select the 32bit version "vc_redist.x86.exe"
```

---
## \#895 Posted by: JasperM Posted at: 2018-06-12T03:01:56.260Z Reads: 234

```
Cheers that worked, I selected the x64 one.

Thanks for your help
```

---
## \#896 Posted by: JasperM Posted at: 2018-06-12T04:11:07.857Z Reads: 247

```
Hey mate, I have updated the firmware and done the binding.
I have changed the app to UART, set the Baud rate to 115200, and set Nunchuck to current with reverse.
when I push the joystick forward there is a signal on the remote but no spinning of wheels.
I am however receiving data from the board.

Any ideas?
```

---
## \#897 Posted by: JasperM Posted at: 2018-06-12T04:58:33.248Z Reads: 262

```
This is how I have it connected and I am running FW2.18 on my Focbox.
![15287794265127228989143820376719|243x500](upload://9ZzU8x0sp30I6ZLEfPXA29GF87l.jpg)
```

---
## \#898 Posted by: Wajdi Posted at: 2018-06-12T05:25:50.282Z Reads: 256

```
Hi Jasper, this is because you are running an older FW, update to a latest Vesc firmware and you should be ready to go.
```

---
## \#899 Posted by: JasperM Posted at: 2018-06-12T06:20:07.910Z Reads: 246

```
I remember seeing somewhere that the photon doesn't work with Ackermaniac's FW, what firmware would you recommend, I'm just after ridability, nothing too crazy.
```

---
## \#900 Posted by: Wajdi Posted at: 2018-06-12T06:33:16.269Z Reads: 247

```
3.35 is working fine on my testing units.
```

---
## \#901 Posted by: JasperM Posted at: 2018-06-12T06:55:59.647Z Reads: 256

```
I'll try it tonight. 

Cheers for your help.
```

---
## \#902 Posted by: JasperM Posted at: 2018-06-12T09:55:30.360Z Reads: 280

```
I finaly figured out how to update the FW to 3.35, but VESC Tool is still saying that the FW is too old and I need to update to be able to use all of the program.

So i updated to 3.38 and I am no longer receiving board bat%, Voltage and distance is in the neg as per pic.

On the up side the remote now spins the wheels :grinning:

![20180612_195415|243x500](upload://xFA9kzOnqsIAeCidZCmmxzcfjq.jpg)
```

---
## \#903 Posted by: JasperM Posted at: 2018-06-12T10:48:31.068Z Reads: 284

```
Ok I tried the motor detection in VESC Tool and it failed, but everything else seemed to work so I powered on.

I just applied full throttle on my workbench and the speedo went from 0 to 61 instantly.

When I then brake it slows the motor but just before it stops there is a chunk sound and the fault light flashes briefly.
```

---
## \#904 Posted by: i2oadsweepei2 Posted at: 2018-06-12T11:28:32.216Z Reads: 278

```
I don’t want to derail too much. But is this something that we can use without the photon remote? Stats visible on the board while using our own remotes? Sorry if I missed this somewhere just curious. Thanks

Continuing the discussion from [No words...just pictures delete words! Use pm!](http://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5570):
```

---
## \#905 Posted by: Wajdi Posted at: 2018-06-12T14:09:33.034Z Reads: 277

```
Hi Jasper, You need to get the motor detection working first. Disconnect the receiver from your Vesc and try the motor detection again.
For the board battery voltage to be correct on your remote, make sure to go Photon settings and set the right number of cells of your board.
```

---
## \#906 Posted by: Wajdi Posted at: 2018-06-12T14:10:38.819Z Reads: 282

```
@i2oadsweepei2 That's a full control panel I'm working on right now and will post a proper thread about soon. It is standalone and does work with any remote.
```

---
## \#907 Posted by: Wajdi Posted at: 2018-06-12T14:32:07.201Z Reads: 299

```
@JasperM I just updated to Fw 3.38 and it works perfectly. Make sure you do motor detection without the receiver connected and it passes.
![image|375x500](upload://dN5ceyUC8jnIgRcDubKIcqYYXj7.jpeg)
```

---
## \#908 Posted by: Deckoz Posted at: 2018-06-12T15:46:09.696Z Reads: 287

```
@Wajdi saw the truck mounted screen. 

When can get it? It is uart telemetry device only correct? Or does it require a photon receiver? 

I am hoping it connects directly to the vesc and processes telemetry and isn't wireless...
```

---
## \#909 Posted by: Wajdi Posted at: 2018-06-12T15:57:48.966Z Reads: 278

```
@Deckoz It's a standalone control panel and telemetry device, with its own hardware and software, does not require a photon. I will be posting a more detailed thread soon.
```

---
## \#910 Posted by: JasperM Posted at: 2018-06-13T09:04:48.969Z Reads: 298

```
I have unplugged the receiver and attempted to detect the motor again and it failed again.

Below are the settings I put into the wizzard and my set up.

The motor spins then stops and then slowly chuggs around like it wants to spin but cant quite get there.

![15288802534281414388086010989455|243x500](upload://2kZgwo7WfBqXz6JAb75O9vJvsFJ.jpg)

![15288802956927221875757986533526|243x500](upload://pPRbLumICQ7RuDN9mk15BUuYpT.jpg)

![15288803346518742486440039133640|243x500](upload://Acotqo954wrmjHQQw9C30UYzwuh.jpg)

![15288803728867952028298326940901|690x335](upload://q7JjKtbfRktNNzdCe0X6Grlrtn6.jpg)
```

---
## \#911 Posted by: meesie Posted at: 2018-06-13T09:14:32.431Z Reads: 279

```
try increasing the amps and/or ERPM in the motor detection a bit. there's also a nifty little question mark button that will tell you how to fix certain detection problems
```

---
## \#912 Posted by: SeanHacker Posted at: 2018-06-13T11:04:32.196Z Reads: 282

```
Increase duty to .15 then see how it does.
```

---
## \#913 Posted by: JasperM Posted at: 2018-06-13T11:05:39.110Z Reads: 313

```
OK...I fixed the detection problemby increasing the duty to .07, thanks meesie.

I went for a ride and my board pulls like crazy now and it's nice having all of the data on the remote in your hand.

But the first thing to happen was the brakes stopped working, they felt like they were trying to engage every second or so but couldn't. but a little latter kicked in.

Then the acceleration stopped working. The remote still showed a signal for everything but the Temp on the remote showed 57 degrees, is this high, I could also smell burning plastic but I could not feel any warmth from the motor or the enclosure at all and the ambient temp here is around 15 degrees. In my garage 10 minutes later the temp was in the 30s again and the board works. I have pulled my Focbox open and taken pictures, the only thing I can see is the negative wire looks kinked? :thinking:

I realise this might be getting off track for this thread but I am not all over Vesc settings and don't want to brick my Focbox. Any settings that I may have stuffed?

![15288888491848208166471231976181|243x500](upload://4zDQ60SOfUjfJFhwAfPcL2ThnsL.jpg)

![15288888887935108277629264901585|243x500](upload://uO4LFxblPhcr4PbuNcIIAqWCyZb.jpg)
```

---
## \#916 Posted by: isaacmedford Posted at: 2018-07-30T12:51:50.566Z Reads: 288

```
@Wajdi with .42 photon firmware on new style receiver with whip antenna and using Acks 3.38 firmware I am unable to perform a ppm pulselength map.  I can see the green graph raise up and down as the joystick is moved but not in the input setup wizzard app.  I am receiving data on the remote such as V, A, P, ect.

Also, with the A.Off setting on the remote turned on , after the set time is reached it turns off as designed.  Then when trying to turn back on it will flash the screen and not turn back on until the battery plug connection is reset.

Any ideas?
```

---
## \#917 Posted by: Wajdi Posted at: 2018-08-01T15:32:34.507Z Reads: 285

```
It is recommended to use UART control, if you still want to use the PPM port, set control to ADC.
```

---
## \#918 Posted by: Linny Posted at: 2018-08-06T15:39:25.702Z Reads: 278

```
With some elbow grease and effort, the casing can be made to look like an injection molded piece. ![20180617_135832|690x388](upload://jfEerudnT7l7FlMl45ovCAlVeGC.jpg)
```

---
## \#919 Posted by: mishrasubhransu Posted at: 2018-08-06T17:41:29.509Z Reads: 264

```
How did you give it a matte finish?
```

---
## \#920 Posted by: uigiroux Posted at: 2018-08-07T02:31:40.077Z Reads: 265

```
He said 'elbow greese', lol :wink:
```

---
## \#921 Posted by: Linny Posted at: 2018-08-07T05:36:40.225Z Reads: 276

```
Take a look at my thread on how to smooth out 3D prints. 
https://www.electric-skateboard.builders/t/how-to-make-your-3d-printed-remote-part-look-hella-pro/63931
```

---
## \#922 Posted by: skatardude10 Posted at: 2018-08-08T02:41:39.347Z Reads: 269

```
Is this remote still not compatible with @Ackmaniac's firmware v3.101? 

I'd love to get this remote for the turn signal functionality, but only if I can still use ESC Monitor with BT on the slave to change settings on the go like I do with acks firmware.

@Deckoz mentioned using ackmaniacs firmware with this remote... Any update from you by chance?
```

---
## \#923 Posted by: Wajdi Posted at: 2018-08-08T17:06:04.074Z Reads: 269

```
@skatardude10 I have seen several using Ack firmware successfully with Photon remote  however I did not test it personally. Maybe someone who is using Ack Fw can confirm.
```

---
## \#924 Posted by: skatardude10 Posted at: 2018-08-08T18:11:23.487Z Reads: 269

```
Good to know, thanks man!
```

---
## \#925 Posted by: Jansen Posted at: 2018-08-10T04:07:40.673Z Reads: 269

```
When is the new casing for the photon going to be coming out, If i pre-order now will I get the new one you posted a while back?
```

---
## \#926 Posted by: Wajdi Posted at: 2018-08-10T09:35:49.127Z Reads: 272

```
[quote="Wajdi, post:909, topic:24654"]
It’s a standalone control panel and telemetry device, with its own hardware and software, does not require a photon. I will be posting a more detailed thread soon.
[/quote]

If you are referring to this, it’s a new control panel, unrelated to the Photon remote, more information about it here https://www.electric-skateboard.builders/t/proton-digital-instrument-and-control-panel-touch-screen/58664/95
```

---
## \#927 Posted by: JasperM Posted at: 2018-08-17T09:04:18.418Z Reads: 260

```
Does anyone else have a problem with the remote taking a long time to pair with the board when turning on, if I take the enclosure off and short the bind pins it works but that is a dick around.

If I leave the remote sitting on the board for a while I'll come back and it will be connected, shouldn't it connect straight away?
```

---
## \#928 Posted by: Wajdi Posted at: 2018-08-17T09:16:47.655Z Reads: 260

```
@JasperM
It should auto pair right away every time you power on the board. What version are you running on the remote?
```

---
## \#929 Posted by: JasperM Posted at: 2018-08-17T10:00:28.159Z Reads: 276

```
Im running the latest FW.

I just came back from a ride where it stoppped working half way through, before my ride I had to remove the enclosure and bind again.

Ive just removed the enclosure to investigate and have found that the antenna square thingy has fallen off the receiver. 
How is it secured to the pcb, it almost looks it was only held on by the hot glue gun glue.
![15344999042286063617919371833600|243x500](upload://q1cUcGEdQaD3jjqzQ96rDvJpSpZ.jpg)
![1534499951658121047470031952701|243x500](upload://y6baSAmS6F2WZ80ZmzwkV9zJoHU.jpg)
```

---
## \#930 Posted by: Wajdi Posted at: 2018-08-17T10:15:07.199Z Reads: 255

```
That explains the pairing issues, seems like a bad solder joints. I will receive a new version of the receiver by the end of this month, and I will send you a new replacement.
```

---
## \#931 Posted by: JasperM Posted at: 2018-08-17T10:17:04.307Z Reads: 264

```
Cool, is the silver square thingy only held down on one side?
If so can it be secured all round?
```

---
## \#932 Posted by: Wajdi Posted at: 2018-08-17T10:18:02.175Z Reads: 263

```
Yes currently only held on one side, new versions will have it secured from the sides also.
```

---
## \#933 Posted by: Giba Posted at: 2018-08-18T00:54:43.276Z Reads: 265

```
@Wajdi g’day mate hope you count my remote and receiver on these batch as I cannot wait no more to use these highly demanding awesome remote 🙂
See my last email just to remind you![image|323x500](upload://k1ck0KX03EGOjq1X9Op2uooQfpN.jpeg)
```

---
## \#934 Posted by: Wajdi Posted at: 2018-08-18T10:58:15.289Z Reads: 257

```
@Giba Yes yours is in it.
```

---
## \#935 Posted by: Wajdi Posted at: 2018-08-29T20:03:12.811Z Reads: 258

```
Hey guys,
Just a quick update, a newer version of the Photon is currently in production. 
Improved receiver design, now with micro USB to update software.
New NRF modules with FCC certification.
Binding using a micro button instead of jumper.
Hardware improvement of the remote, now with hard reset function.

**Receiver**

![18%20PM|580x302](upload://avVpiirVITC7MR36ysXkmCjLBxq.png)

**Remote**

![39%20PM|690x208](upload://f3tS6J7J6EgQ3SVS24yfcplQKpI.png)

For everyone that has a preorder pending, you will get the latest version shipped in about 8-10 business days.
```

---
## \#936 Posted by: lockeboss Posted at: 2018-09-02T17:05:00.072Z Reads: 253

```
Hi,

I have just read on the Homepage for the single receiver that  its ideal if you want to run two receivers at the same time for a dual setup. 

Right now im planning my first build so im still in the "learn everything about the eskate technic". my question is,what are the differnces from a dual setup with 2 receivers to one with a single receiver.since its ther first time i have read about that.

when i make a pre order now will i already get the new version withe the Improved receiver design?

im looking forward to holding one in my hands :smiley:
```

---
## \#937 Posted by: Wajdi Posted at: 2018-09-02T17:33:54.950Z Reads: 241

```
@lockeboss Yes, if you order now you will get the updated version.
For a dual setup, if you have your Vescs connected using CAN bus, then 1 receiver connected to the master Vesc is enough. If you plan to keep both Vescs separated, then one receiver per Vesc would be needed in this case.
```

---
## \#938 Posted by: lockeboss Posted at: 2018-09-02T17:56:21.826Z Reads: 243

```
Perfect!
Thanks for the quick response. Going to order soon :slight_smile:
```

---
## \#939 Posted by: Jansen Posted at: 2018-09-06T21:59:31.347Z Reads: 243

```
[quote="Wajdi, post:937, topic:24654"]
Yes, if you order now you will get the updated version.
For a dual setup, if you have your Vescs connected using CAN bus, then 1 receiver connected to the master Vesc is enough. If you plan to keep both Vescs separated, then one receiver per Vesc would be needed in this case.
[/quote]

Couple quick questions I wanted to know and/or confirm before putting my order in right if you could let me know when you have time @Wajdi

- Any discount for buying both the photon and proton at the same time? 
- Lead time for shipment to go out and/or arrive to me (SoCal USA) for each product if ordered by tomorrow?
- I see you updated the design on the improved receiver, are you still planning to make the photon with the newer more sleek \ smaller casing you posted a 3d print sample of earlier in the thread or is that on the back burner for now?
- I believe I've read the answer to this already but the photon does work with the ackmaniac FW right?
- If I am running my dual FOCbox set up via PPM instead of CANbus I would need to buy an extra receiver to work properly it looks like, am I understanding that correctly?
- To use the photon once received, what steps need to be taken at this point besides the typical plugging the receiver in the VESC's and pairing, is that all right now or are there any extra steps (not super technical in this matter so hoping it's as easy as using any new remote, or not too much more if there are extra steps)

Thanks so much in advance and keep up the excellent hard work as it all looks amazing and the ESK8 com has been lacking a remote like this. Can't wait to have it hand and be using it. Been wanting cruise control for ages now!!!!

Appreciate your quick response in advance @Wajdi
```

---
## \#940 Posted by: Wajdi Posted at: 2018-09-06T23:37:16.219Z Reads: 248

```
The new Photon remotes will be even more powerful than ever. To answer your questions:

[quote="Jansen, post:939, topic:24654"]
Any discount for buying both the photon and proton at the same time?
[/quote]
Normally not, but PM me once you are ready, I might add a discount for you  :wink:

[quote="Jansen, post:939, topic:24654"]
Lead time for shipment to go out and/or arrive to me (SoCal USA) for each product if ordered by tomorrow?
[/quote]

I was just contacted by the fab today confirming the status update for the new Photon PCBs, I should have them in hand in about 9 business days, and shipped to you in about 2 more days.
Regarding the Proton control panel, it will take about 25 days before I have the first batch ready to be shipped out.

[quote="Jansen, post:939, topic:24654"]
I see you updated the design on the improved receiver, are you still planning to make the photon with the newer more sleek \ smaller casing you posted a 3d print sample of earlier in the thread or is that on the back burner for now?
[/quote]

Are you referring to the casing of the receiver? I stopped printing the receiver casing due to the extra delay it adds for it to be printed out. I will provide the 3D files so you can print a casing for it. I might add that as an add-on option.

[quote="Jansen, post:939, topic:24654"]
I believe I’ve read the answer to this already but the photon does work with the ackmaniac FW right?
[/quote]

It should be, I didn't officially test it. If I have the chance, I might confirm that soon.

[quote="Jansen, post:939, topic:24654"]
If I am running my dual FOCbox set up via PPM instead of CANbus I would need to buy an extra receiver to work properly it looks like, am I understanding that correctly?
[/quote]

If your Vescs are not connected through CAN, you will need a receiver for each Vesc.

[quote="Jansen, post:939, topic:24654"]
* To use the photon once received, what steps need to be taken at this point besides the typical plugging the receiver in the VESC’s and pairing, is that all right now or are there any extra steps (not super technical in this matter so hoping it’s as easy as using any new remote, or not too much more if there are extra steps)

No extra steps are required. Remotes are shipped already paired to their receivers. One thing you need to do is to set the app to UART, and make sure the baud rate is at 115200.
[/quote]
```

---
## \#941 Posted by: JasperM Posted at: 2018-09-07T01:21:11.755Z Reads: 220

```
[quote="Wajdi, post:940, topic:24654"]
I was just contacted by the fab today confirming the status update for the new Photon PCBs, I should have them in hand in about 9 business days, and shipped to you in about 2 more days.
[/quote]

Does that include the new reciever that you are sending me?
```

---
## \#942 Posted by: Wajdi Posted at: 2018-09-07T04:31:31.407Z Reads: 220

```
@JasperM  Yes.
```

---
## \#943 Posted by: Jreamer Posted at: 2018-09-18T21:35:25.359Z Reads: 221

```
So I'm not sure where to look for this but I could use a tutorial on how to set this remote up. I have only every used Nano remotes so this is all new to me. Thanks!
```

---
## \#944 Posted by: JasperM Posted at: 2018-09-18T22:13:47.517Z Reads: 219

```
Go to @Wajdi website and sign in to the forum there. There is a mega thread there that goes through stuff from memory.
```

---
## \#945 Posted by: Jreamer Posted at: 2018-09-18T22:17:25.148Z Reads: 225

```
Exactly what I was looking for! Thanks.
```

---
## \#946 Posted by: Nedtrampz Posted at: 2018-09-19T00:56:54.608Z Reads: 231

```
does the speed show in kmph or mph? both?
```

---
## \#947 Posted by: Jreamer Posted at: 2018-09-19T01:52:04.337Z Reads: 230

```
You can choose in the remote menu screen. @Nedtrampz
```

---
## \#948 Posted by: Wajdi Posted at: 2018-09-22T20:27:19.618Z Reads: 237

```
Just received the new batch of the Photon remotes, they look so fresh!
![IMG_1188|375x500](upload://4sBdXY7rJqO5xssKFuC8DcxpM7R.jpeg) ![IMG_1190|375x500](upload://oVFFRmBANIogIk8VnK560t3rnJJ.jpeg) ![IMG_1189|375x500](upload://5XQHjWMT186k9DT60Zu1sUDeWJd.jpeg) 

Receiver now has a push button for binding, and a micro usb port to easily update its firmware.
I still need to solder the push buttons on the remote, joystick and screen, but its almost ready.
```

---
## \#949 Posted by: Wajdi Posted at: 2018-09-23T00:34:51.576Z Reads: 239

```
Half way through, adding displays and testing tomorrow.

![IMG_1192|666x500](upload://mr7JAgOS0emDaIyUYHk2hkY0Kan.jpeg) ![IMG_1195|375x500](upload://gR9SAAzr4EztLhhkhHcTyJLCe2X.jpeg)
```

---
## \#950 Posted by: JasperM Posted at: 2018-09-23T00:38:46.263Z Reads: 228

```
Can you send me the shipping number when you send the receiver to me, do you need my address again or have you still got it?
```

---
## \#951 Posted by: Wajdi Posted at: 2018-09-23T00:39:29.959Z Reads: 226

```
Just send me a pm with your previous order number and I will find it.
```

---
## \#952 Posted by: JasperM Posted at: 2018-09-23T00:46:43.634Z Reads: 226

```
PM sent

10 char
```

---
## \#953 Posted by: Acidfie Posted at: 2018-09-29T20:13:16.796Z Reads: 218

```
Anyone want to say something about the reliability of the connection?
```

---
## \#954 Posted by: JasperM Posted at: 2018-09-29T20:31:43.966Z Reads: 224

```
I must admit I haven't used mine much when I had it working but I never had any problems with the connection once paired.
```

---
## \#955 Posted by: Giba Posted at: 2018-09-29T23:49:03.732Z Reads: 224

```
I believe mine is in this batch? Or is it already on its way, am I right? @Wajdi
```

---
## \#956 Posted by: Jansen Posted at: 2018-09-30T00:50:34.293Z Reads: 233

```
Thanks for all of the info, really appreciate it. The only thing that you didn't answer for me that maybe I just didn't explain properly based on how you answered it..... on the casing question, I wasn't asking about a casing for the receiver (even though I would love to have one for it as well if possible) but I was asking if and when you are going to be switching the change the casing on the actual remote to the slimmer / sleeker looking one that I have seen on a couple threads as well as a random website or two.... I've includeda pic just in case I'm still not making sense....

LMK when you can and thanks so much again for all your help. Depending on what your answer is I could be ready as soon as my next reply back to you.

Thanks in advance and Talk soon brotha, 


 ![Photon|690x311](upload://rJHPPSBt0UWuTEx1aPLDkEHGndt.jpeg)
```

---
## \#957 Posted by: Schulerbible Posted at: 2018-09-30T00:57:06.568Z Reads: 225

```
It would be great to do a complete makeover of the casing such that it looks like the Evolve R2 remote ....
```

---
## \#958 Posted by: Wajdi Posted at: 2018-09-30T15:49:46.464Z Reads: 242

```
@Giba Yes it's in this batch, I'm currently finishing up some testing and then it will be ready for shipping. I also got new antennas, smaller and compact 
![IMG_1224|375x500](upload://q3jrwTQhmWXQZreHiwxLBITMDkI.jpeg) ![IMG_1235|375x500](upload://r0cqvDfP8nWwKZ3yzJgfluqzL3d.jpeg) 

@Jansen I see now what you meant. The current version of the Photon is at it's smallest form. There is a slight difference in the design but the remote overall is very thin and small
![47%20AM|689x281](upload://d7I7gTdqiPaw3gvUGJSyDJQ5mRs.jpeg) 
![IMG_1236|375x500](upload://6G6ix8BqMfXDsoVwFJCyj75teRM.jpeg) 

@Schulerbible Oh man, the Evolve R2 design is just awful :laughing: I never liked it.
```

---
## \#959 Posted by: Jansen Posted at: 2018-09-30T20:51:36.212Z Reads: 240

```
[quote="Wajdi, post:958, topic:24654"]
@Jansen I see now what you meant. The current version of the Photon is at it’s smallest form. There is a slight difference in the design but the remote overall is very thin and small
[/quote]

Niiiice! That does look really good, thanks for the clarification. I think I'm sold. Have any / most of the bugs (if any) been worked out of the OS and/or how is it running / how d
o you like the final product. 

If I order today like Im thinking whats the lead time to get to me in Southern California USA? 92807

Thanks for your replies brotha, really appreciate it
```

---
## \#960 Posted by: Wajdi Posted at: 2018-09-30T21:57:01.486Z Reads: 234

```
Glad to hear that! 
Most of the bugs have been fixed, software has been highly optimized throughout the year, most of the receiver flaws have also been addressed, and I can say the hardware is at its final version right now. 
Lead time is about 2 weeks, all current units that I have right now are sold, but I have another batch already in production and should be received is 2 weeks or less.
```

---
## \#961 Posted by: 701Superjet Posted at: 2018-10-01T19:17:46.231Z Reads: 235

```
Any plans of making a trigger style version?
```

---
## \#962 Posted by: Wajdi Posted at: 2018-10-03T01:46:25.886Z Reads: 254

```
Remotes are ready, the only thing taking time right now is 3D printing...
![IMG_1256|375x500](upload://hbLPQ7BRKLNLDuFw6GuufgHNj3a.jpeg) ![IMG_1257|375x500](upload://bk7AJPkoEX4XpYhCnbwn311kHyD.jpeg) ![IMG_1255|375x500](upload://vBflKeiPeMQDPSDqkgv08pJrsqX.jpeg) ![IMG_1254|375x500](upload://3eLwVpDuRPpn5QrzVqAy9SMfN7U.jpeg) 

If you have pre-ordered, and can access a 3D printer, and don't want to wait for the covers to be 3D printed, PM me or send me an email and I will send you the electronics and .STL files.
```

---
## \#963 Posted by: JasperM Posted at: 2018-10-03T10:53:23.655Z Reads: 244

```
@Wajdi, is my reciever coming soon?
```

---
## \#964 Posted by: Wajdi Posted at: 2018-10-04T14:54:11.612Z Reads: 245

```
Yes, should be ready this week.
I also published the .stl files for the Photon casing on thingiverse :+1:
https://www.thingiverse.com/thing:3133640
And also on my website:
https://eboardshop.net/product/photon-casing-stl-files/
```

---
## \#965 Posted by: ricardo Posted at: 2018-10-12T15:25:44.139Z Reads: 237

```
Hi,

Do you have any updates on the cases and shipping? Can't wait to get this on my hands... All the rest of my build is ready!

Congrats for the great work btw! 

Cheers, 
Ricardo
```

---
## \#966 Posted by: jadatmag Posted at: 2018-10-14T21:19:34.863Z Reads: 235

```
Does anyone know if this remote will work with the Raptor 2?

@Mickyboy have you tested? As changing the firmware on the Raptor 2 is no option.

Reverse function, cruise control, out-of-the-box? Just switching the receiver? Sounds to good to be true!

Will changing between FOC and BLDC be possible (in the future). Changing Amp settings etc? Removing the need for a smartphone!!
```

---
## \#967 Posted by: Wajdi Posted at: 2018-10-14T21:42:19.175Z Reads: 239

```
Currently packing up the remotes, all done.

![IMG_1362|375x500](upload://hsjNQtZVv72jC7Ff2nX1ojOVvca.jpeg) ![IMG_1368|375x500](upload://5xXm9Kbz7Nsm7fR9D4dM4WNDKsF.jpeg) 

@jadatmag Yes it should work with the Raptor 2, just plug the receiver, its that simple.
[quote="jadatmag, post:966, topic:24654"]
Will changing between FOC and BLDC be possible (in the future). Changing Amp settings etc? Removing the need for a smartphone!!
[/quote]
Probably in the future I will introduce those features as a software update.
```

---
## \#968 Posted by: jadatmag Posted at: 2018-10-14T21:43:50.054Z Reads: 228

```
OMG do you have a spare one in this batch?????
```

---
## \#969 Posted by: Wajdi Posted at: 2018-10-14T21:44:54.798Z Reads: 230

```
I have a new batch coming up in about a week.
```

---
## \#970 Posted by: jadatmag Posted at: 2018-10-14T21:45:41.583Z Reads: 238

```
NONONONONONO kick someone from the que, I don't care. I'm ordering RIGHT NOW

edit:
Might be a stupid question to ask after ordering, but will this work with the Focbox unity? @Wajdi
Because I'm planning to upgrade as I'm going to be receiving it for free.
```

---
## \#971 Posted by: Wajdi Posted at: 2018-10-14T21:52:08.729Z Reads: 234

```
:joy: Thank you for your order :+1:
Yes its compatible with Focbox unity because it uses the same open source firmware by Vedder.
```

---
## \#972 Posted by: totalgeek9224 Posted at: 2018-10-14T22:05:02.720Z Reads: 231

```
Share your secret.... :joy:
how does one receive a unity for free?:thinking:
```

---
## \#973 Posted by: SkaterBoy58 Posted at: 2018-10-14T22:58:54.051Z Reads: 232

```
Probably ordered a Rapter and built up store credit of $100 per month for delayed shipment!
```

---
## \#974 Posted by: jadatmag Posted at: 2018-10-14T23:20:09.091Z Reads: 231

```
I was getting a warranty replacement. It got stuck at customs in The Czech Republic for 3 months along with 37 other boards (mostly normal orders). So they decided to send us free Unity's.

People who ordered way later then the people with a board in the stuck batch were already receiving their Raptor 2's.

In the end my warranty replacement took 5 months. And I had to put serious effort in to get those 5 months waiting time compensated with extra warranty. (It isn't standard practice for Enertion to compensate waiting time for warranty repairs and replacements. Even if that means u lose 5 months of your 12 months warranty period.
```

---
## \#975 Posted by: JasperM Posted at: 2018-10-20T10:48:36.758Z Reads: 230

```
Update on shipping?
```

---
## \#976 Posted by: Wajdi Posted at: 2018-10-23T02:15:55.646Z Reads: 239

```
@JasperM Getting there! 
![IMG_1384|666x500](upload://9xsyYkentBguT2jOtEPOX1H21nz.jpeg) 

I'm writing an updated tutorial on how to use the remote as things have changed considerably.
Also v0.5 is going to be released in a few hours, contains major fixed and recommended.
```

---
## \#977 Posted by: JasperM Posted at: 2018-10-23T02:29:37.467Z Reads: 232

```
All good,

I'm just over my GT2B. 😁
```

---
## \#978 Posted by: Wajdi Posted at: 2018-10-23T05:13:54.064Z Reads: 237

```
V0.5 of the Photon remote is released.

* Major bug fixes
* Optimized power consumption
* Fixed instances of random boot up due an RTC bug

Available for download here http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#979 Posted by: jadatmag Posted at: 2018-10-23T15:02:41.049Z Reads: 233

```
I'm sorry brah, your order got delayed because he's sending your remote to me instead.
```

---
## \#980 Posted by: JasperM Posted at: 2018-10-23T20:07:18.578Z Reads: 232

```
All good, I'm just getting the receiver.
```

---
## \#981 Posted by: Wajdi Posted at: 2018-10-25T04:49:54.838Z Reads: 240

```
Receiver V0.2 firmware update is out!

It fixes a common problem related to antenna power overload. 
By default the receiver is programmed to MAX radio power, this causes problems in some instances where it overloads itself and results in intermittent connectivity.

This updates adds a new functionality to the push button, allowing to change the radio power level by a short press.

**Short press** = change power level
**Long press ( 4 seconds )** = Enter binding mode

Power change blink code:
* 1 blink = Min level
* 2 blinks = Low level
* 3 blinks = High level
* 4 blinks = Max level

If you are experiencing intermittent connectivity, go through the different power levels until you find the best setting for your environment.
Also don't forget that there is a similar option on the remote itself, under Control->sig. 

Update is available to download here http://forum.eboardshop.net/t/firmware-update-download/59
And the updater tool is available here https://eboardshop.net/product/photon-updater/
```

---
## \#982 Posted by: Giba Posted at: 2018-10-26T01:40:36.451Z Reads: 227

```
Can’t wait anymore to get my hands on with this thing. Have you shipped mine yet @Wajdi?
```

---
## \#983 Posted by: Floyd650 Posted at: 2018-10-28T01:50:44.529Z Reads: 229

```
I got my remote in the mail a few days ago.  I can't tell you how stoked I am.  I just need to get a few kinks worked out.  I am having two issues.  

The first is with intermittent connectivity.  If I go to the binding mode in the remote and push the button on the receiver it typically binds and seems to work flawlessly.  But if I goof around with it for more than a few minutes I lose connection.  If I enter the binding mode again, it won't reconnect without pushing the button on the receiver again, which of course would be a real hassle if the remote was tucked away in the enclosure.  

The second issue is that the Photon Updater doesn't recognize the remote when I pug it into my computer's USB.  I can tell it's connected because it's charging, but no matter how many times I hit "Refresh" it never populates the Port.

If I could get the remote to connect with the updater, maybe I could update the software regarding antenna overload...
```

---
## \#984 Posted by: Wajdi Posted at: 2018-10-28T01:54:41.756Z Reads: 215

```
@Floyd650 Connect the receiver to your computer, not the remote. Also make sure that the receiver is powered on. Let me know if this makes it recognizable.
```

---
## \#985 Posted by: Floyd650 Posted at: 2018-10-28T01:59:17.435Z Reads: 219

```
Wow.  That was the fastest response in the world.  Thanks, and yes that worked perfectly.  Now I'm in the updater.  I'll see if I can get my connectivity sorted out.  Thanks again for making such an amazing tool!
```

---
## \#986 Posted by: Wajdi Posted at: 2018-10-29T01:10:29.987Z Reads: 224

```
New remote version 0.51 is released, I discovered a bug when canceling a binding process using the home button instead of the joystick push button, causing the binding loop to not cancel properly and keeps running even when at the main screen. 
This results in poor connectivity and power on issues.

Update is available for download here http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#987 Posted by: Volts Posted at: 2018-10-29T12:40:58.505Z Reads: 220

```
Hi Wajdi, been 2 weeks since perchance any updates?
```

---
## \#988 Posted by: Wajdi Posted at: 2018-10-29T14:20:59.955Z Reads: 215

```
Hi Volts, please PM your order number. Thanks!
```

---
## \#989 Posted by: Giba Posted at: 2018-10-30T15:42:42.079Z Reads: 209

```
@Wajdi any update on shipping?
```

---
## \#990 Posted by: Wajdi Posted at: 2018-10-31T02:34:22.742Z Reads: 222

```
@Giba I created shipping labels for most orders today, let me know if you didn't receive yours.

Update: I improved the overall response time by optimizing the FHSS synchronization between the remote and receiver. This increased the response time by almost 200%, telemetry now has a higher refresh rate due to less missed packets, and commands are more instantaneous. 

* V0.52 (remote) is released
*Improved FHSS (Frequency Hopping Spread Spectrum) synchronization. Response time is improved by 200%.  **V0.3 is mandatory on the receiver for this to work.**

* V0.3 (Receiver) is released
*Improved FHSS (Frequency Hopping Spread Spectrum) synchronization. Response time is improved by 200%.  **V0.52 is mandatory on the remote for this to work.**

Download as usual is available here http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#991 Posted by: Giba Posted at: 2018-10-31T10:45:12.054Z Reads: 215

```
@Wajdi No, I didn’t received any mate. Checked all my emails folders including spam and junk mail folder, there’s nothing
```

---
## \#992 Posted by: JasperM Posted at: 2018-11-01T11:14:36.227Z Reads: 210

```
I also have no shipping info in my emails.
```

---
## \#993 Posted by: Volts Posted at: 2018-11-01T12:51:30.713Z Reads: 208

```
Look at your promotion box I found mine in there
```

---
## \#994 Posted by: JasperM Posted at: 2018-11-01T23:17:58.001Z Reads: 206

```
Promotion box?
```

---
## \#995 Posted by: ethel Posted at: 2018-11-01T23:50:30.619Z Reads: 206

```
Junk box maybe?
```

---
## \#996 Posted by: JasperM Posted at: 2018-11-02T02:47:06.319Z Reads: 200

```
I've checked all the boxes.......all of them. :yum:
```

---
## \#997 Posted by: PickSix24 Posted at: 2018-11-04T16:26:35.375Z Reads: 200

```
What’s the shipping time if I ordered today ?
```

---
## \#998 Posted by: Wajdi Posted at: 2018-11-05T21:17:44.404Z Reads: 202

```
Sorry guys for the delays, 
I have printed the shipping labels, and will be dropping off the packages during the next 2-3 days. Antennas were delayed.
@PickSix24 I would say current tentative shipping time is about a week.
```

---
## \#999 Posted by: Holyman92 Posted at: 2018-11-05T21:50:47.264Z Reads: 203

```
@Wajdi would i happen to be ont he orders going out? #416
```

---
## \#1000 Posted by: Giba Posted at: 2018-11-09T19:59:04.372Z Reads: 196

```
4days fast since your last update any good news to deliver @Wajdi
```

---
## \#1001 Posted by: JasperM Posted at: 2018-11-10T04:14:25.124Z Reads: 198

```
@Wajdi is there any update on shipping?
```

---
## \#1002 Posted by: Volts Posted at: 2018-11-11T11:58:51.771Z Reads: 194

```
Mines on the way YAY!
```

---
## \#1003 Posted by: City-Blade-101 Posted at: 2018-11-13T18:26:29.073Z Reads: 191

```
AWESOME AS FUCK!
...no use for a name, but I would call it "ALPHA ONE" :sunglasses:
because its the beginning of a new remote century.
Edit: just one question that i could not figure out in this threat: Is the button on top a dead mans switch? (HOPEFULLY NOT! AHHHHHHHHH!)
```

---
## \#1004 Posted by: Linny Posted at: 2018-11-13T18:52:34.707Z Reads: 187

```
It can be a reverse, cruise control or deadman. Pretty neat to have different choices for the button
```

---
## \#1005 Posted by: City-Blade-101 Posted at: 2018-11-13T22:21:54.791Z Reads: 192

```
WOW sounds good,very impressive.:thinking:
speechless  at this point:no_mouth:
```

---
## \#1006 Posted by: MiniChopper4Me Posted at: 2018-11-18T02:24:34.666Z Reads: 193

```
What material is the remote printed with? I want to smooth it out like @linny did, but considering the acetone vapor bath (if its in fact made with ABS) or I'll order some of that gloop if its made using PLA.
```

---
## \#1007 Posted by: Linny Posted at: 2018-11-18T02:37:48.928Z Reads: 194

```
I think it's printed in PLA. For the photon I'd suggest filler primer and wet sanding after 4 or 5 heavy coats to fill up the lines
```

---
## \#1008 Posted by: MiniChopper4Me Posted at: 2018-11-18T02:51:08.119Z Reads: 188

```
Thanks, I'll give that a try!
```

---
## \#1009 Posted by: Giba Posted at: 2018-11-19T06:25:17.124Z Reads: 190

```
@Wajdi you know I paid money for this thing and that is my hard earned money to fund my project to enjoy what I work hard for! I bought it last March received the remote defective! You said you going to replaced it you even mentioned it many tmes here in the forum! And I am patiently waited to replace your defective remote and until now it seems that you are just ignoring all my messages! Is this how you do bussiness?
```

---
## \#1010 Posted by: Wajdi Posted at: 2018-11-20T04:10:17.561Z Reads: 196

```
@Giba Sorry man, but I'm not sure what you are talking about. I never received any messages regarding your issue and I honestly have no idea what's going on. If you can PM me your order number and what issue you are having I might be able to help.
```

---
## \#1011 Posted by: Giba Posted at: 2018-11-20T06:04:24.802Z Reads: 221

```
@Wajdi ![image|281x500](upload://6iJiRyhsGo2O5JsCbPXUbWYrTuD.png)  ![image|281x500](upload://j3fw0BELDVCxwsMajMh8KcluEFc.png) ![image|281x500](upload://zQ3b8i4mDe4I8twmFCscH0RniU0.png) that screenshot should be enough to refresh your memory mate. And if you can back read to these forum I always doing a follow up about the shipment
```

---
## \#1012 Posted by: Wajdi Posted at: 2018-11-20T06:20:06.911Z Reads: 202

```
@Giba Gotcha, didn’t recognize your forum name.
```

---
## \#1013 Posted by: Volts Posted at: 2018-11-21T06:28:58.163Z Reads: 209

```
Anyone else having trouble logging into the firmware update page, also has anyone use the photon remote and reciever setup with a VESC 6 from Trampa Boards, if so can they post a pic of their receiver to controller wiring please.
```

---
## \#1014 Posted by: Wajdi Posted at: 2018-11-22T00:57:44.882Z Reads: 202

```
I sent you an email on how to connect it. If you have any questions let me know.
```

---
## \#1016 Posted by: Volts Posted at: 2018-11-22T07:26:22.453Z Reads: 202

```
Got to say this is one hell of a setup, makes the long ass wait time worth it, for future buyers, get two recievers if you are running vedders VESC 6 cause Can bus doesn't work over UART, but also from some tests with ppm can bus has impedance miss match or delay which will fuck things up at some point
```

---
## \#1017 Posted by: Giba Posted at: 2018-11-26T16:27:12.238Z Reads: 193

```
@Wajdi any update on sending me the remote man?
```

---
## \#1018 Posted by: Gaz Posted at: 2018-12-07T03:01:08.977Z Reads: 188

```
Hi @Wajdi 

Any thoughts as to when you may have more in stock?  Thank you. WiIl you be offering a kit deal, remote, Receiver and display. Cheers.  LOVE THE DISPLAY.
```

---
## \#1019 Posted by: jadatmag Posted at: 2018-12-07T15:01:03.175Z Reads: 189

```
Took me a few hours to set this up but I now have bluetooth via my slave, photon receiver on the master with according baudrates, canbus forward, motor directions, multiple esc's settings in the Nunchuck tab (REALLY WTF????) And all kinds of other settings that I changed and changed back that I don't understand shit from. I don't know where I would be without this community and forum.

I had to throw out 3 laptops, eat up 6 fingers and punch 6 holes in every wall that's surrounding me. But it's all working now. I can now ride backwards with my Photon remote while I'm checking my speed on my Apple watch while changing my power settings on my phone. I'm so happy that I'm blowing a rape whistle right now.
```

---
## \#1020 Posted by: Gerrycorrado Posted at: 2018-12-07T15:08:54.477Z Reads: 185

```
I might need to pay you a visit in the future then :stuck_out_tongue:
```

---
## \#1021 Posted by: jadatmag Posted at: 2018-12-07T16:33:09.643Z Reads: 184

```
You bought the Photon remote and have  2 vesc's?
```

---
## \#1022 Posted by: Gerrycorrado Posted at: 2018-12-08T13:22:27.597Z Reads: 188

```
2 maytechs
```

---
## \#1023 Posted by: Chupacabra Posted at: 2018-12-09T03:08:03.263Z Reads: 197

```
Hi What's the latest on the delivery times. I want this remote but don't wanna wait to long as i don't have a replacement and need a remote for my build.
```

---
## \#1024 Posted by: Holyman92 Posted at: 2018-12-12T07:16:40.843Z Reads: 196

```
![jpg_1544598655793|281x500](upload://xD7QrH44AIFXW38h4CCA4E0gWsh.jpeg) 

@Chupacabra here's my order... I hate to do it, but come Monday I'll most likely be doing a charge back a month and a half is a crazy long wait time for processing. Sadly I missed out on the hoyt discount because I was torn between this remote and hoyt and now I wish I'd have gone with hoyt
```

---
## \#1025 Posted by: danggilmore Posted at: 2018-12-12T07:35:57.389Z Reads: 192

```
I'm sure if you just ask for your money back, he'll refund you. He's hella nice and logical.
```

---
## \#1026 Posted by: Holyman92 Posted at: 2018-12-12T07:45:31.774Z Reads: 194

```
![Screenshot_20181212-014448|690x297](upload://rnYL09Z76FqlFpX2QHmouti5hlz.jpeg)

I sent him an email a week ago w/ no reply (as of an hr ago when i checked) and the last message I received was 22 day ago on here that is why I'm resorting to a charge back... it's never my 1st go to and i like to think I'm fairly reasonable when it comes to waiting for a product
```

---
## \#1027 Posted by: visnu777 Posted at: 2018-12-12T17:17:24.993Z Reads: 179

```
I hope he is well. I'm waiting for a photon too (for over one month without notice). He was helpful and communicative before so I hope everything is alright for him :)
```

---
## \#1028 Posted by: Brianr058 Posted at: 2018-12-12T19:24:10.226Z Reads: 171

```
Great innovator, not so much the business man
```

---
## \#1029 Posted by: jadatmag Posted at: 2018-12-12T20:38:12.750Z Reads: 177

```
Placed order on Oktober 14th. I asked him where my order was by personal message on this forum on November 29th and he hasn't answered since.

Received it on November 30th though.

He seems to be MIA...
```

---
## \#1030 Posted by: JasperM Posted at: 2018-12-13T00:30:05.922Z Reads: 183

```
My receiver broke due to bad soldering and he said that the would replace it for me, that was in September.

Every time I contact him he constantly says 'it will be posted in the next couple of days.'

Then I said that its becoming a bit ridiculous, he said he would send it the next day. I asked him for a tracking number two days later and he supplied one, the problem is it still says that USPS has not actualy received the package yet. The shipping label was created on 22 Nov.

Great remote, really bad warranty. I essentially have a really expensive paper weight at the moment.:triumph:
```

---
## \#1031 Posted by: ElectricCoast Posted at: 2018-12-13T18:07:50.718Z Reads: 177

```
I thought this remote was cool but accountability is everything to me.  Just my 2 cents.
```

---
## \#1032 Posted by: Giba Posted at: 2018-12-13T18:25:09.401Z Reads: 181

```
@JasperM hey mate have you got your sorted? I also have a warranty issue on my remote purchased last March’18 and since then I haven’t actually used it. I got a defective one 😤 He keep saying it will be replaced I lost count how many times I gave him my order number but still waiting until now and he doesn’t respond at all. @Wajdi whatever you doing now mate, I don’t know how you able to sleep giving that you left some people waiting who payed you our hard earned money for a product that supposedly a satisfying not a nightmare!
```

---
## \#1033 Posted by: visnu777 Posted at: 2018-12-13T19:45:09.940Z Reads: 175

```
After reading all this I opened a dispute on PayPal. I'm a bit sad since I wanted that remote badly but 184 dollars is too much for not getting any response but instead reading about these issues :(
```

---
## \#1034 Posted by: JasperM Posted at: 2018-12-13T21:31:38.911Z Reads: 181

```
No I still don't have a receiver, just a tracking number for a non existent package.

Its really anoying because the hand full of times that I did get to use the photon, it was great.

I also gave hime my address and order number multiple times.
```

---
## \#1035 Posted by: jadatmag Posted at: 2018-12-15T00:42:52.984Z Reads: 182

```
I have received and installed the receiver but started getting cut-outs.

I made sure I updated the firmware on the remote and receiver.

It works and does everything I want it to do. Except that it's loses connection every few seconds. I can see the connection being lost because the signal lights on both my focboxes turn off (with throttle pinned) everytime the connection is lost. When it loses connection the board shortly does not respond to throttle or braking.

I tried doing the pairing process a few times, reflashing firmware a few times, trying out all signal strenght combinations on the remote and receiver (on high and max settings on the remote the remote doesn't even connect) and nothing gives me a solid connection.

I emailed @Wadjia and hope he will be here to help me (us) out.
```

---
## \#1036 Posted by: Wajdi Posted at: 2018-12-15T01:14:15.453Z Reads: 186

```
Sorry guys I was away from the forums for a while, I was extremely busy. I always answer emails at contact@eboardshop.net tho if Im not on the forums. Let the reply marathon begins :smiley:

@Holyman92 I sent your package yesterday, I hope you received your tracking number/
@JasperM @Giba really sorry guys, I didn't forget about you. Will be sending out your replacements this week, I was very short on components lately.

@visnu777 Sorry to see you go, I saw your Paypal claim and refunded you right away. Should of just emailed me :smile: 

@jadatmag I just published an update, Remote V0.54 and receiver V0.4.

**-Photon Receiver: V0.4**
* **Remote has to be updated to V0.53 for this to work.**
*Fixes and improves connectivity

**-Photon Remote: V0.53**

* Fixes several software issues.
* Improves connectivity
* **Receiver has to be V0.4**    

Download here http://forum.eboardshop.net/t/firmware-update-download/59

Just FYI guys, Photon remote is now out of stock and unavailable for purchase, I don't know when I will bring it back, but I will figure something out.
```

---
## \#1037 Posted by: visnu777 Posted at: 2018-12-15T11:01:36.755Z Reads: 180

```
[quote="Wajdi, post:1036, topic:24654"]
Just FYI guys, Photon remote is now out of stock and unavailable for purchase, I don’t know when I will bring it back, but I will figure something out.
[/quote]
Hi Wajdi, thats what I was hoping for, information :D Actually if you had written that before I wouldn't have wanted the refund. The lack of communication, the sudden "out of stock" on the website and the negative feedback from others had driven me there :) And yes, I should have written you a direct email first but since you advertised on this forum and used it for documentation of progress it was my first thought to contact you here. I still believe that your remote is the ultimate one, so see that you restock and I'll be the first one in line :D I even got some led strip for it in addition to my regular headlights.
```

---
## \#1038 Posted by: jadatmag Posted at: 2018-12-15T15:57:22.338Z Reads: 181

```
In bench testing the connection seems to be solid now!

But now the reverse function doesn't work anymore.

When pressing the top button and full throttle at the same time the wheels start gaining speed really slowly, but not in reverse.

It seems Rev. does the same as Cruise. But Cruise doesn't let you lower the speed while holding the button. Rev. does let you lower your speed while pressing the button.
```

---
## \#1039 Posted by: jadatmag Posted at: 2018-12-15T16:25:27.199Z Reads: 183

```
I think I found a bug;

With V.max @ 4.20 and V.min @ 3.00 the battery percentage according to the board @ 33.00 V is 5%. Which is quite different from what the Android Ackmaniac monitoring tool gives me and my board itself says on it's display.

Changing V.min to 2.00 with 33.00 V gives me 8% battery, which is still less then what my board itself and the Android Ackmaniac monitoring tool gives me.

Something isn't right with the formula or calculation.
```

---
## \#1040 Posted by: Wajdi Posted at: 2018-12-15T16:55:51.585Z Reads: 188

```
I just tested both cruise and reverse functions, they work fine. When you have the trigger set to reverse, you only press it once to change direction, when set to cruise, you keep holding the button to maintain speed, push throttle up to increase speed, and down to decrease speed.

Regarding the battery percentage, what the Photon is telling you is the closest to reality. The Photon uses typical li-ion cell discharge curve to estimate your percentage left.
The curve is similar to this
http://siliconlightworks.com/image/data/Info_Pages/Li-ion%20Discharge%20Voltage%20Curve%20Typical.jpg 

Which neither your battery monitor nor the app I believe do.
```

---
## \#1041 Posted by: bevilacqua Posted at: 2018-12-15T17:18:38.983Z Reads: 179

```
that discharge curve looks a bit too exagerated // Rather +2C discharging or even a LiFepo cell

Look for a dischrage chart for a lipo cell that fits your C—rating
```

---
## \#1042 Posted by: Wajdi Posted at: 2018-12-15T18:10:34.349Z Reads: 176

```
Im not using that one, just an example image I quickly found online.
```

---
## \#1043 Posted by: jadatmag Posted at: 2018-12-16T22:58:33.257Z Reads: 177

```
I've tested the remote under normal riding conditions today and the update seemed to have done the trick, not a single disconnect or hickup!

The reverse function still acts exactly like 'cruise'. I'm able to slowly ramp up or ramp down my speed in Rev.  When switching to 'Cruise' it won't let me decellarate though. Maybe it's something in my focbox settings. I'll look into it the next time I open up my board.

**V0.53** + **V0.4**
```

---
## \#1044 Posted by: Wajdi Posted at: 2018-12-17T17:07:38.284Z Reads: 173

```
Sweet, glad the update fixed the connection issues. 
And yes I agree, perhaps a configuration issue with the reverse, check your nunchuck control and see if its set to current control without reverse.
```

---
## \#1045 Posted by: DAddYE Posted at: 2018-12-17T18:23:14.926Z Reads: 170

```
Hey sir! Since you’re planning on stopping the development on this remote did you think about open sourcing the firmware?
```

---
## \#1046 Posted by: jadatmag Posted at: 2018-12-17T21:10:02.909Z Reads: 173

```
Setting 'control Type' to 'Current' in the Nunchuk tab did the trick!

The mode 'Cruise'  on the remote now also ramps up and down fine.
```

---
## \#1047 Posted by: Goonman Posted at: 2018-12-18T05:06:24.298Z Reads: 179

```
I am about to throw this thing in to a low earth orbit. I am trying to update the firmware to .53 and .4(both downloaded) has dropped out and frozen up multiple times. So far I have downloaded windows x64  and x86 and Arduino adafruit etc. I have found the device in device manager. Uninstalled and reinstalled via browse file and finding the Arduino file. But windows saying no can do because it's not x64 file. I guess that's why I have already downloaded and setup x86. Not that I know what any of this shit means anyway. Not interested in coding Arduino and com port BS just wanted to ride my F&$@ing Esk8!
Can someone help?
```

---
## \#1048 Posted by: visnu777 Posted at: 2018-12-18T05:55:44.841Z Reads: 174

```
I'll give you 50$ for it ;)
```

---
## \#1049 Posted by: jadatmag Posted at: 2018-12-18T09:57:06.124Z Reads: 185

```
Have you tried running windows update? Let it go through all update cycles. It should find the correct drivers itself.
```

---
## \#1050 Posted by: JasperM Posted at: 2018-12-18T11:36:15.980Z Reads: 185

```
Ill give you $30 for your receiver.:rofl:
```

---
## \#1051 Posted by: Mich21050 Posted at: 2018-12-18T11:52:16.671Z Reads: 181

```
I would give you 60$ for it :slight_smile:
```

---
## \#1052 Posted by: visnu777 Posted at: 2018-12-18T12:26:21.427Z Reads: 176

```
65 dollars 😜
```

---
## \#1053 Posted by: Mich21050 Posted at: 2018-12-18T12:27:13.726Z Reads: 174

```
65,99$ :joy:
```

---
## \#1054 Posted by: Wajdi Posted at: 2018-12-18T15:37:17.941Z Reads: 178

```
@Goonman Can you please post what error you are getting? Does the Photon updater executes and run?

@DAddYE I never said I'm stopping development, heck Im just getting started :wink:
```

---
## \#1055 Posted by: DAddYE Posted at: 2018-12-18T15:38:43.845Z Reads: 180

```
I tried 😂 would be really neat tho 😇
```

---
## \#1056 Posted by: Goonman Posted at: 2018-12-19T01:20:02.698Z Reads: 179

```
It's saying that the file should be x64 to run. The remote was working yesterday. So I will try and sort some other time. Or when it stops working again
```

---
## \#1057 Posted by: uigiroux Posted at: 2018-12-19T04:20:51.526Z Reads: 178

```
Lol I'm so glad to hear that!  I was just reading the thread trying to catch up and saw the post saying you were stopping so I just started speed reading trying to find out more, haha.  Glad your keeping at it!  Will be ordering from you soon :slight_smile:
```

---
## \#1058 Posted by: Goonman Posted at: 2018-12-19T06:38:45.735Z Reads: 174

```
Thanks yeah I did that.
```

---
## \#1059 Posted by: Giba Posted at: 2018-12-19T09:47:49.949Z Reads: 184

```
[quote="Wajdi, post:1036, topic:24654"]
@JasperM @Giba really sorry guys, I didn’t forget about you. Will be sending out your replacements this week, I was very short on components lately.
[/quote]
@Wajdi hey mate! any news about the replacements of our remote?
```

---
## \#1060 Posted by: JasperM Posted at: 2018-12-20T10:19:43.174Z Reads: 181

```
The tracking number that @Wajdi gave me still says that USPS still have not received the package since 22 Nov 18, almost a month. 

Its starting to feel like he is not interested in replacing expensive defective parts. Just stringing us along.
```

---
## \#1061 Posted by: jadatmag Posted at: 2018-12-23T02:59:32.582Z Reads: 179

```
Can I connect the Photon receiver on my Slave focbox?

My bluetooth receiver for the phone apps seems to read settings fine but isn't able to write settings while connected through the Slave Focbox.

I'm on Ackmaniac firmware
```

---
## \#1062 Posted by: hoeksame1 Posted at: 2018-12-23T17:04:46.321Z Reads: 180

```
Needatmagniet
```

---
## \#1063 Posted by: DAddYE Posted at: 2018-12-23T19:57:53.531Z Reads: 188

```
Yup you can however see my comments. It appears that on some Vesc (mine are Focboxes) either the Bluetooth module or the receiver causes reset issues
```

---
## \#1064 Posted by: Wajdi Posted at: 2018-12-28T03:35:03.337Z Reads: 193

```
![IMG_1685|666x500](upload://zPxTb6ebGXy0IUNqfJP3B5oIfhe.jpeg) 
@JasperM @Giba I finally received the batch today, it took forever to be done for some reason. :tired_face:
```

---
## \#1065 Posted by: JasperM Posted at: 2018-12-28T22:47:01.914Z Reads: 192

```
@Wajdi - Mate, some communication would be nice. In your last messages you said you would be sending it in the next couple of days, that was almost a month ago.

I you were waiting for parts to be made I would have  been a bit more understanding.
```

---
## \#1066 Posted by: Minim Posted at: 2018-12-28T23:18:20.249Z Reads: 191

```
Are you going to get them back in stock soon?
```

---
## \#1067 Posted by: unityserpentw Posted at: 2018-12-29T00:14:21.605Z Reads: 194

```
@Wajdi - Ive got the Photon connected with the Focbox Unity. Have a question, Im trying to wire my own existing binding button to the receiver board. Now that you've added the micro switch, is it still possible to add the wiring and if so where? I've circled one spot where the pinout shows it may be possible. If so, can you explain how? I![RECEIVER|580x302](upload://umenDWtqX0d9Y5FHx612aJYHw5A.png)
```

---
## \#1068 Posted by: Holyman92 Posted at: 2018-12-29T01:13:42.184Z Reads: 189

```
Anyone else have an issue with acceleration? It seems that take off and accelerating are causing cogging and it seems like it just loses power momentarily while trying to accelerate unless holding the cruise button and accelerating while cruise is pressed. 

I tested to see if it was the controller by using my regular rc remote and the rc remote works fine
```

---
## \#1069 Posted by: JasperM Posted at: 2018-12-30T09:54:23.475Z Reads: 184

```
I have emailed you through your website not too long ago, no reply there either, the shipping label you printed on 22 Nov has not been updated.

Are you sending this receiver soon? Is there a different tracking number?
```

---
## \#1070 Posted by: FredXanadu Posted at: 2019-01-05T20:42:54.239Z Reads: 180

```
Hello @Wajdi,  any update concerning the compatibility with the unity ?
```

---
## \#1071 Posted by: JasperM Posted at: 2019-01-06T02:49:32.325Z Reads: 196

```
Still no update. Just continuous excuses of being busy.

![Screenshot_20190106-124722_17TRACK|243x500](upload://mhP7V3Cn1teYhsYiD9iHVAahePt.jpeg)
```

---
## \#1072 Posted by: FredXanadu Posted at: 2019-01-09T16:49:11.958Z Reads: 185

```
Hello @Wajdi, cool you please answer me concerning the compatibility problem between the Unity and the Photon ? Any update on this ?
```

---
## \#1073 Posted by: Wajdi Posted at: 2019-01-09T21:05:04.451Z Reads: 193

```
Hi @JasperM, your package was sent out a couple days ago
![53%20PM|690x214](upload://qfqR40kNzGblQAAqln730o2EzO8.png) 

@FredXanadu I'm working on an update to make it compatible with Unity, I still don't have access to that Esc, only the source code at the moment, but I should be able to get it working pretty soon.
```

---
## \#1074 Posted by: Komamtb Posted at: 2019-01-16T08:40:47.054Z Reads: 182

```
So how people are finding the remotes? Worth the buck?
```

---
## \#1075 Posted by: Bikekrazy Posted at: 2019-01-22T15:01:12.650Z Reads: 178

```
I like the idea of controlling board functions from the remote and not being locked into an OEM remote control.
```

---
## \#1076 Posted by: Volts Posted at: 2019-01-24T03:01:10.057Z Reads: 181

```
Its a very good product, but expect to wait 2-3 months for the goods
```

---
## \#1077 Posted by: FredXanadu Posted at: 2019-01-24T11:15:02.840Z Reads: 179

```
Any update concerning the Unity compatibility ?
```

---
## \#1078 Posted by: Wajdi Posted at: 2019-01-24T15:11:08.226Z Reads: 177

```
I managed to update the compatibility, I will be posting the receiver firmware update today.
```

---
## \#1079 Posted by: unityserpentw Posted at: 2019-01-25T03:33:18.736Z Reads: 182

```
Awesome,  been patiently waiting for this update.  Photon been working great otherwise.  With this update it will be the best and most advanced universal remote....
```

---
## \#1080 Posted by: Wajdi Posted at: 2019-01-25T05:04:06.262Z Reads: 187

```
Receiver V0.41 FW released.
* Compatible with remote FW 0.53 and up.
* Adds support for Unity

Please give me feedback if this works, I cannot test it as I don't have the hardware.

Download here http://forum.eboardshop.net/t/firmware-update-download/59
```

---
## \#1081 Posted by: Volts Posted at: 2019-01-26T06:50:54.131Z Reads: 175

```
just tryed to update my remote failed for some reason and now it wont turn on, anyone know how to fix this problem?
```

---
## \#1082 Posted by: Volts Posted at: 2019-01-26T06:53:54.909Z Reads: 177

```
did you have your remote turned on when you updated?
```

---
## \#1083 Posted by: ricardo Posted at: 2019-01-26T11:44:59.425Z Reads: 174

```
@Wajdi, can't seem to find out how to change sensitivity of the remote? At the moment the remote seems a bit slow to respond/have to move the throttle a bit before it responds... is there a guide or a video for this?

Cheers,
Ricardo
```

---
## \#1084 Posted by: Wajdi Posted at: 2019-01-26T15:39:00.116Z Reads: 178

```
Did you double check that you have put the remote firmware on the remote and not the receiver one? They are different and can’t be mixed up. Try again following this tutorial http://forum.eboardshop.net/t/photon-updater-guide/55 make sure you select the correct COM port.

@ricardo there is a bit of a dead band at the beginning and end, which is normal.
```

---
## \#1085 Posted by: Wajdi Posted at: 2019-01-26T15:53:52.079Z Reads: 178

```
Also if you had the correct firmware the first time, it means that your remote is in boot loader mode right now, that's why its not turning on, following this steps to get the drivers and finish the setup https://www.electric-skateboard.builders/t/universal-advanced-vesc-remote-control-photon-custom-design/24654/581
```

---
## \#1086 Posted by: Volts Posted at: 2019-01-27T06:07:29.074Z Reads: 180

```
I have duel vecs setup, just tryed running two recievers to one remote and now i have a controller that wont turn on, did i just brick my controller? help
```

---
## \#1087 Posted by: ricardo Posted at: 2019-01-27T07:53:48.723Z Reads: 181

```
Is there a way of eliminating that dead band? it accounts for about 30% of the total trigger travel and, as a result, can be really annoying/dangerous if i want to make a fast start...
```

---
## \#1088 Posted by: Chupacabra Posted at: 2019-02-05T16:36:45.203Z Reads: 176

```
@Wajdi Did you just make the remote available on the website again? It says there’s one unit available. Dibs!
```

---
## \#1089 Posted by: Chupacabra Posted at: 2019-02-05T21:07:48.499Z Reads: 178

```
WTF Who bought the remote? Its gone!!
Damn no respect for dibs at all. What has this world come to?
```

---
## \#1090 Posted by: Wajdi Posted at: 2019-02-05T23:49:37.694Z Reads: 174

```
@Chupacabra Sorry about that man :laughing: I made a couple lately and they are already gone. I will be making some more units by the end of the week, I will let you know once I have them ready.
```

---
## \#1091 Posted by: Chupacabra Posted at: 2019-02-05T23:57:45.836Z Reads: 173

```
@Wajdi That'll be super dope man :fire: :fire:. Please keep one remote aside for me. I can pay you a deposit to secure my place if needed.
```

---
## \#1092 Posted by: sodniwe Posted at: 2019-02-22T23:19:26.825Z Reads: 160

```
@Wajdi Any remotes available?  Mine just broke and i'm looking to buy a new one.
```

---
## \#1093 Posted by: StefanMe Posted at: 2019-02-22T23:39:11.497Z Reads: 158

```
I guess eskating.eu are selling them in the future...
```

---
## \#1094 Posted by: Wajdi Posted at: 2019-02-23T00:10:09.529Z Reads: 159

```
I received parts today, I should have them ready for shipping next week.
```

---
## \#1095 Posted by: Chupacabra Posted at: 2019-03-02T04:12:56.099Z Reads: 159

```
Hi @Wajdi Just got your remote today and oh man is it good. I am using Flipsky VESC 6.6 that has 1.5A 5V rated port. I was wondering if I could hook up 14  led lights to the back light port and would that still work in the ratio 4:6:4 or 5:4:5 for reactive lights?
```

---
## \#1096 Posted by: bevilacqua Posted at: 2019-03-02T08:57:23.311Z Reads: 156

```
I would avoid that port for stability/security reasons. Some guys had problems on 4.12 HW (1A rated) I wouldt play with fire even on 6.X HW and 1.5A

Better use a DCDC step down
```

---
## \#1097 Posted by: Chupacabra Posted at: 2019-03-02T14:41:50.051Z Reads: 150

```
Thanks. But even with 10 lights I wasn’t able to make the led lights work. I tried with both the front and back led light post but no success.
```

---
## \#1098 Posted by: Floyd650 Posted at: 2019-03-03T06:43:05.406Z Reads: 144

```
Up and running!  Love it!
```

---
## \#1099 Posted by: atlasdev Posted at: 2019-03-03T22:27:28.901Z Reads: 146

```
Hi, This looks amazing and would love to buy one!

Just one question. I want to customize my lights, while using the remote. Is it possible to read the values from the remote? The values I'm interested are the following:

 - Speed & brake (Y-axis of the joystick)
 - Left & right indicators (X-axis of the joystick)
 - The button to change light modes

I would be using a arduino nano for it, so I can use any ports on there.

Thanks!
```

---
## \#1100 Posted by: Wajdi Posted at: 2019-03-03T22:57:38.032Z Reads: 149

```
@Chupacabra What leds are you using? are they WS2812B? 
Recently I discovered that they don't work well when the data input is at 3v3 while supply is at 5v.
I made a post about it here https://www.electric-skateboard.builders/t/photon-addressable-leds/74309/10?u=wajdi
Also to activate the leds you have to press the b button on the remote. Reactive brake lights work with 10 leds, 3 for left, 3 for right, and 4 for middle. This number is fixed at the moment.
Also as @bevilacqua suggested, it is better to use a step down converter to stay in the safe side.

@atlasdev Currently you can read the joystick middle push button from the control port on the receiver here https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/2/0/2052bf4ecb4502018af76502b464cf4ac0f919d9_2_690x359.png

You can use that for anything you want to control using the remote.
Regarding the joystick reading values and the b button, those are sent to the receiver and embedded into the RF packets, they are used internally. There are currently no easy way to get those values, but with some work you can extract the joystick values from the UART port by having an arduino in between, assuming your arduino has at least two uart ports. For example connect the receiver uart port to an arduino port 1, unpack the data, extract the joystick values, and forward the original packet to the vesc through port 2.
```

---
## \#1101 Posted by: atlasdev Posted at: 2019-03-03T23:52:03.616Z Reads: 150

```
Thanks for the reply. That's a shame really. Correct me if I'm wrong but isn't Uart a really simple protocol? Can't I just hook up an arduino serial read pin to the TX of the Photon? This means I don't have to create a proxy between the remote and the VESC and as it's read only means I can't even interfere with the connection. The only thing I think is missing is the indicator, or do you send that to the VESC as well?
```

---
## \#1102 Posted by: Wajdi Posted at: 2019-03-04T01:00:12.892Z Reads: 152

```
That actually might work, you can parallel read the serial data coming out of the tx pin of the receiver to your arduino, and extract the joystick values.The values you would get are up/down, since those are sent to the vesc for acceleration/braking. The left/right are still not accessible.
One more button you can read from the communication is the trigger button. So in total you have up/down, trigger button and joystick push button.
It is possible to read the indicator (left/right) but it requires a custom firmware, seeing that you won't be using the led ports on the receiver, they can be remapped to reflect that. If you are interested in that I can definitely enable it for you.
```

---
## \#1103 Posted by: atlasdev Posted at: 2019-03-04T07:41:52.744Z Reads: 153

```
Thanks! I'll definitly take you up on that offer! You should have received my order :)
```

---
## \#1104 Posted by: Chupacabra Posted at: 2019-03-21T18:09:09.475Z Reads: 161

```
Hi @Wajdi

I am having trouble connecting my receiver to the flipsky Vesc 6.6 plus and need help. 

Is the light supposed to be green or orange? Initially I was able to get my remote to work but somehow this time I cannot. 

I am connecting it here by switching the TX and RX wires. I am also noticing that my VESC keeps turning on and off when the receiver is connected. I must tell you that I have soldered 10 leds to the remote based upon your earlier response. 

![V6_2beee7c4-4918-4bd4-b92e-746d2a67755b_2048x2048|553x499](upload://m404Lu9TeV7uoWDmqpwOMJpElJv.jpeg) 

Can you please help!
```

---
## \#1105 Posted by: Chupacabra Posted at: 2019-03-22T20:23:04.857Z Reads: 152

```
Just to update I'm getting the orange light and am running the Ackmaniac 3.103. I was able to run it on this setup before no problem. I am unable to do so this time.
```

---
## \#1106 Posted by: Chupacabra Posted at: 2019-03-22T21:19:40.682Z Reads: 151

```
@Wajdi I am also unable to download any update file from your website. Its not allowing me to create a user id. Everytime I try, i get a message saying email already in use.
```

---
## \#1107 Posted by: Komamtb Posted at: 2019-03-25T13:45:22.023Z Reads: 149

```
@Wajdi I also have an orange light instead of green, what does this mean? the data is flowing.
at the moment my remote does'nt conect to the receiver anymore. No idea how that happened.
The remotes battery % keeps changing from 0 to 90% 5 times per second all the time, teli data sometimes also does that. From my testing, accelaration comand gets stuck for a few seconds in cruise control mode, very bad and expensive experience I had. So at the moment the remote is not even usable.
```

---
## \#1108 Posted by: Wajdi Posted at: 2019-03-28T18:58:00.001Z Reads: 150

```
@Chupacabra I suggest you remove the LEDs and see if the problem is solved. All the latest receivers have orange LED indicating power on. Green led is only on when pairing.

@Komamtb Orange light means it's powered on, there is an option to change signal power level on the remote and receiver, make sure you have it set to min or low on the remote, also on the receiver press the button once to cycle through the signal modes. Blinking led will tell what power you are on, 1 blink is min, and 4 blinks are max, set the receiver to min or low power as well and see if this improves the signal quality.

Regarding the battery percentage, does that happen when charging?
```

---
## \#1109 Posted by: sginthelbt Posted at: 2019-04-01T21:07:38.668Z Reads: 148

```
What version of firmware are you running on what vesc?  I can't get any telemetry on the photon but the remote will spin the wheels.  I also have an issue with cruise control only working on a single vesc... thinking maybe your multiple esc on the nunchuuk tab might do the trick.

The rape whistle comment made me laugh...
```

---
## \#1110 Posted by: Aries Posted at: 2019-04-02T23:20:24.399Z Reads: 144

```
@Wajdi 
 Hi,
I just received the focbox unity and came across this remote, would this be compatible with the unity since it only uses a ppm port for connecting the receiver?

Also does the remote have a vibration function?
```

---
## \#1111 Posted by: ricardo Posted at: 2019-04-03T13:00:00.246Z Reads: 150

```
Hi guys, 

Just wondering if anyone has the same issue as mine with the Photon remote: the dead band is enormous (about a 1/3 of the total possible travel) and no matter what I do in calibration nothing seems to change (whether the dead band setting is on 0 or 5 it makes absolutely no difference). This irritates me royally, as I'm always a bit afraid of when the remote is going to kick in...!

@Wajdi is there a work around this, or is it a known issue and we just have to learn to live with it?
```

---
## \#1112 Posted by: yousefnjr Posted at: 2019-04-08T19:07:28.921Z Reads: 137

```
^^ dead band on mine feels OK

Have mine hooked up to a Unity and it’s mostly working great. All telemetry is showing on the display (voltage, distance, etc.) except the speed (big red number). Sometimes I’ll see it lock-in a non-zero value, but it doesn’t update in real time at least. Any ideas? Using UART cable, and I think settings in Focbox UI were 11500 baud 

I also can’t get the focbox UI to detect the throttle for remote calibration. I’m able to get the wheels moving when riding, just can’t get Focbox UI to recognize it.
```

---
## \#1113 Posted by: Chupacabra Posted at: 2019-04-08T22:44:11.252Z Reads: 133

```
Try using the FOCBOX tool. I had a similar issue that I was able to solve with the tool
```

---
## \#1114 Posted by: atlasdev Posted at: 2019-04-15T20:49:59.619Z Reads: 146

```
Hi,

I just received my unit, and tried it out for a little bit. It seemed to work, but I had to go before I could play around with it more. After I came back the battery seemed dead, so I charged it. Now the backlight of the screen does not work. It flashes when I start it (so it does work), but then it's very dim and most of the time it doesn't seem to be on. What could this be caused by? I've tried updating the firmware and reseating the battery connector (to powercycle it), but this does not change it.

Thanks!
```

---
## \#1115 Posted by: Komamtb Posted at: 2019-04-22T06:35:26.596Z Reads: 141

```
https://youtu.be/pnZQzGx-xmw
Anyone else had is having some of the same issues? I can't get the to work with Wajdi.
```

---
## \#1116 Posted by: esk81 Posted at: 2019-04-24T09:19:38.536Z Reads: 136

```
Just some curiosity, what is the function of the failsafe on the transceiver? 
If no signal, the motor and ESC stop working immediately. Why a failsafe needed?
```

---
## \#1117 Posted by: mmaner Posted at: 2019-04-24T12:48:23.722Z Reads: 135

```
[quote="esk81, post:1116, topic:24654"]
If no signal, the motor and ESC stop working immediately.
[/quote]

Incorrect.  Sometimes it will go full throttle, depending on out of the box settings.  You have to set the function of the ESC after PPM drop.
```

---
## \#1118 Posted by: Hardwiring Posted at: 2019-04-30T21:52:02.743Z Reads: 135

```
hi, after an update this is all i get. 
https://youtu.be/hmrL4nqF6TM
windows 10, arduino drivers installed and official update tool... tried different cables.... tried everything..... top to bottom of the thread...
have I killed it? suggestions please
```

---
## \#1119 Posted by: Guz Posted at: 2019-05-03T03:27:48.033Z Reads: 127

```
hey guys whats the lead time on one of these if we order today?
```

---
## \#1120 Posted by: Hardwiring Posted at: 2019-05-03T20:56:12.024Z Reads: 126

```
@MiniChopper4Me ..... This Guy :clap::clap::clap::clap:

https://www.electric-skateboard.builders/t/how-to-guide-photon-remote-initial-setup/72139/17?u=hardwiring
```

---
## \#1121 Posted by: Scoo_B_SK8 Posted at: 2019-05-09T17:24:51.788Z Reads: 117

```
@Wajdi

Just busted open the box 📦 with the photon injection molds (moved to new location, travel for work, new baby #4 has had my head spinning for awhile). 

To all that have had to wait for “shells”... that is on me.  I told wajdi i was going to, but as described above it got pushed to the side. 

My very very bad😖!

So gonna try and knock a bunch out in the next week or 2 and get em into wajdi’s hands. (First few batches on me wajdi, sorry bro!).
```

---
## \#1122 Posted by: Komamtb Posted at: 2019-05-10T11:34:54.966Z Reads: 111

```
Is @Wajdi gone from the forum again?
```

---
## \#1123 Posted by: Flasher Posted at: 2019-06-05T02:58:10.024Z Reads: 96

```
anyone can help me out? im trying to update the remote but my computer doesnt recognize it.... i tried installing arduino ide and using its driver folder as a reference for the windows installer but i am still unable to find a driver for it
```

---
## \#1124 Posted by: Wajdi Posted at: 2019-06-05T04:32:12.254Z Reads: 101

```
Try this steps https://www.electric-skateboard.builders/t/universal-advanced-vesc-remote-control-photon-custom-design/24654/581
```

---
## \#1125 Posted by: ricardo Posted at: 2019-07-22T08:15:14.811Z Reads: 84

```
would you be able to run be through the steps on it? Really at a loss here, and it annoys the hell out of me... :-/ also tagging @Wajdi just in case...
```

---
## \#1126 Posted by: Brobert Posted at: 2019-12-31T17:30:45.579Z Reads: 56

```
I cant seem to download the photon updater every link of it you made does not work
```

---
## \#1127 Posted by: Wizeartz Posted at: 2020-01-06T09:04:09.716Z Reads: 48

```
Hi, is the Photon still available? Thanks
```

---
## \#1128 Posted by: Mainsedora Posted at: 2020-01-06T18:18:58.732Z Reads: 48

```
just get a vesc wand
```

---
## \#1129 Posted by: solid_37 Posted at: 2020-01-08T21:28:34.548Z Reads: 43

```
another thing can just vaste my time and money.
I have wait it several month. 
They respond last time 30 day ago. your remote is ready for shipment.
now the eboardshop.net it's offline.
Another 200€ vasted in a trash tech.
good work scammers!!
```

---
## \#1130 Posted by: Darren_Banana Posted at: 2020-01-12T08:04:08.921Z Reads: 43

```
Same here. I have waited for my photon remote for a good 2 months and nothing has arrived. Not even a tracking code. I want my money back!!! @Wajdi
```

---
## \#1131 Posted by: RyEnd Posted at: 2020-01-12T15:54:56.157Z Reads: 43

```
This is why Paypal's 180 day dispute window is great.

I'm at least glad I was waiting on the Photon when the Wand came out, and that stopped me from buying that trainwreck...
Now I'm just waiting for the OSRR while vx2s tide me over...
```

---
## \#1132 Posted by: solid_37 Posted at: 2020-01-12T21:10:46.266Z Reads: 40

```
buy color version of the vx2, if u want use it on focbox.
```

---
## \#1133 Posted by: solid_37 Posted at: 2020-01-12T21:13:08.425Z Reads: 41

```
if u find a way.... these guys escaped with all the money. they selling a photo not a remote ;)
```

---
## \#1134 Posted by: Brobert Posted at: 2020-01-13T13:00:38.328Z Reads: 36

```
I got mine about 7 months ago first purchase starting my evo build the seller does never reply on my messages i gues im one of the last that received a photon remote 
I do know some 3rd partys also sell them maybe they have in stock on their website they are more expensive tho
```

---
## \#1135 Posted by: Brobert Posted at: 2020-01-25T18:37:04.773Z Reads: 26

```
Anyone got the speed meter on the display working With focbox unity?
```

---
## \#1136 Posted by: yousefnjr Posted at: 2020-01-25T19:01:28.924Z Reads: 26

```
Nope. Sometimes it’ll change to something non-zero for a few seconds though. I spent a few weeks fiddling with all the settings I could find before I gave up
```

---
