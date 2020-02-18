# Maytech vesc help Please

### Replies: 44 Views: 3079

## \#1 Posted by: Tampaesk8er Posted at: 2017-05-09T21:24:05.598Z Reads: 211

```
I'm having a slight issue with my (Maytech) vesc remote settings, ( 2.4 Ghz remote).
When my board is connected to computer and I use the keyboard, the throttle and coasting works good.
 But when i use remote controller, the speed at max is slower and when i realease throttle, it slams the brakes. No coasting when throttle released on remote controller, I appreciate all the help from all you talented eboarders, thank you all.
```

---
## \#2 Posted by: Tampaesk8er Posted at: 2017-05-09T21:25:01.318Z Reads: 211

```
Here are my current vesc settings.<img src="/uploads/db1493/original/3X/c/6/c6b1666a4da1a88378c9fee22009dae4e550a41a.JPG" width="669" height="499"><img src="/uploads/db1493/original/3X/e/c/ec6b5170baf2bc72fab55c7c82a434519061f44e.JPG" width="669" height="499">
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-09T21:36:17.712Z Reads: 192

```
Did you set the PPM min/max? First disable your control mode, then go to PPM tab and check the "display" box. Turn on your remote and throttle all the way down and look at the PWM value, then input that value in Min Pulse width, do the same thing with max pulse width at full throttle.

Then turn on your control mode and try again. Also, what control mode are you using? PID speed control and duty cycle will brake at neutral
```

---
## \#4 Posted by: Tampaesk8er Posted at: 2017-05-09T21:43:03.065Z Reads: 188

```
(current, no reverse with brake)
```

---
## \#5 Posted by: Tampaesk8er Posted at: 2017-05-09T21:44:42.128Z Reads: 187

```
Heres my remote and PPM settings.
<img src="/uploads/db1493/original/3X/a/c/ac26f8f802236eab80a09e561f622d111ce4566b.JPG" width="669" height="499"><img src="/uploads/db1493/original/3X/b/9/b98817bbd6521dd3058beecab084cddc9ddab968.JPG" width="669" height="499">
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-09T21:47:28.542Z Reads: 171

```
1.5 minimum is awfully high, did you follow the instructions I gave?
```

---
## \#7 Posted by: Tampaesk8er Posted at: 2017-05-09T21:51:47.343Z Reads: 166

```
yes, what is PWM value and where do i find it?
```

---
## \#8 Posted by: Jinra Posted at: 2017-05-09T21:57:54.238Z Reads: 166

```
It's under the PPM section on the app configuration tab. Follow the instructions I gave above to find your values.
```

---
## \#9 Posted by: Tampaesk8er Posted at: 2017-05-09T22:02:16.323Z Reads: 166

```
this is where im at right now.<img src="/uploads/db1493/original/3X/8/e/8e11baa48a49d181e393b9831bef106f86b7f474.JPG" width="669" height="499">
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-09T22:03:52.842Z Reads: 152

```
PPM section, not ADC
```

---
## \#11 Posted by: Tampaesk8er Posted at: 2017-05-09T22:07:08.327Z Reads: 153

```
oh, my bad.<img src="/uploads/db1493/original/3X/a/b/ab18e218425ae15de09bb1ff4216a37f0c579725.JPG" width="669" height="499">
```

---
## \#12 Posted by: Jinra Posted at: 2017-05-09T22:09:54.150Z Reads: 148

```
Yea now check the "display" box and turn on your controller. Throttle all the way down and record the pulsewidth on the box to the right, and put that number for "minimum pulse width". Do the same for "maximum pulsewidth" at full throttle.
```

---
## \#13 Posted by: Tampaesk8er Posted at: 2017-05-09T22:27:27.632Z Reads: 148

```
i followed the instructions but my numbers arent changing when i hit throttle. I cant find where you tell me to record max number and min number, im so confused. 
im running firmware 2.18 just incase.<img src="/uploads/db1493/original/3X/4/e/4ed0bdb22f274bb3f74742c031e6c23f0d1fd304.JPG" width="669" height="499">
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-09T22:31:51.690Z Reads: 146

```
Check the box in the left circle, and check the PWM signal on the right circle
<img src="/uploads/db1493/original/3X/c/5/c54d6b78a2b8e29722def392dec1a58d8c7be24f.png" width="689" height="217">
```

---
## \#15 Posted by: Tampaesk8er Posted at: 2017-05-09T22:37:56.430Z Reads: 144

```
ok, min was 1.43

max was 1.8.
```

---
## \#16 Posted by: Jinra Posted at: 2017-05-09T22:39:50.960Z Reads: 142

```
Yep so put those values in the appropriate boxes and write config. Then try your throttle again.
```

---
## \#17 Posted by: Tampaesk8er Posted at: 2017-05-09T22:42:28.018Z Reads: 146

```
I did but still brakes when i release throttle to neutral. SMH, LoL.<img src="/uploads/db1493/original/3X/9/d/9de3e9c0b352a0f309afe34d1237eecbfcce7eed.JPG" width="669" height="499">
```

---
## \#18 Posted by: Jinra Posted at: 2017-05-09T22:44:30.901Z Reads: 138

```
You'll have to adjust the trim on your remote. True neutral is the median between your min/max pulsewidth and if your neutral position doesn't match true neutral, it'll accelerate or brake at neutral. Try to adjust your trim to get min pulsewidth closer to 1.0 and max closer to 2.0 with neutral being 1.5
```

---
## \#19 Posted by: Tampaesk8er Posted at: 2017-05-09T22:54:31.453Z Reads: 149

```
its working at these settings.
<img src="/uploads/db1493/original/3X/0/c/0cff61630d4810a5af7800dfe8d35563ba3b8408.JPG" width="669" height="499">
```

---
## \#20 Posted by: Jinra Posted at: 2017-05-09T22:56:44.995Z Reads: 145

```
You lose a lot of throttle range if the green bar isn't in the middle at neutral, keep that in mind.
```

---
## \#21 Posted by: Tampaesk8er Posted at: 2017-05-09T22:58:46.444Z Reads: 137

```
this is where its at right now.<img src="/uploads/db1493/original/3X/6/0/60dd12cb1861a6e921bd66e584c18e047a4d2584.JPG" width="669" height="499">
```

---
## \#22 Posted by: XIII Posted at: 2017-05-09T23:00:19.813Z Reads: 133

```
it has to become 50% , play with the values
```

---
## \#23 Posted by: Jinra Posted at: 2017-05-09T23:00:49.852Z Reads: 135

```
Looks good, just keep in mind you'll lose the difference of your min/max pulsewidth minus the actual min/max of your throttle.

For example if you set max to 1.9, but your max throttle only goes to 1.8, you lose .1 of your throttle. It's best to set the trim just right.
```

---
## \#24 Posted by: Tampaesk8er Posted at: 2017-05-09T23:06:22.289Z Reads: 136

```
thank you so much for taking the time and having patience for walking me through this, i will play with it and learn it. 
 I hope that someone also learns from this walk through. 👍😎
 Time for me to go study the vesc setup manual again. thanks again. LoL.
```

---
## \#25 Posted by: Tampaesk8er Posted at: 2017-05-09T23:09:05.352Z Reads: 139

```
👍👍👍👍👍👍👍👍👍👍👍<img src="/uploads/db1493/original/3X/6/5/650dc2f445513fdbfbbceccb81992f30cc28e387.JPG" width="669" height="499">
```

---
## \#26 Posted by: Tampaesk8er Posted at: 2017-05-10T22:12:57.418Z Reads: 129

```
Big shoutout to @Jinra for helping me out with the VESC and BLDC tool setting up the remote control.
```

---
## \#27 Posted by: schlub Posted at: 2017-05-11T08:29:22.206Z Reads: 125

```
Is this VESC any good? Thinking about getting it myself, Thanks
```

---
## \#28 Posted by: Tampaesk8er Posted at: 2017-05-11T09:32:10.412Z Reads: 128

```
Yes, it works as good as any other vesc. The only difference is they put the maytech name brand on it. My other board has a non maytech brand vesc, they both work fine. Check out @psychotiller, psycotiller.com, thats where I bought my maytech.
```

---
## \#29 Posted by: Maxid Posted at: 2017-05-11T09:36:37.598Z Reads: 120

```
Not true - don't say that.
Maytech VESCs come without a bootloader which is a significant difference!
```

---
## \#30 Posted by: TarzanHBK Posted at: 2017-05-11T09:37:39.778Z Reads: 118

```
they also work only with the original BOM, not the upgraded one
```

---
## \#31 Posted by: Bataleon Posted at: 2017-05-11T09:49:16.469Z Reads: 116

```
I've been using a Maytech VESC on a single drive for 100 km without any issues. So far so good.
```

---
## \#32 Posted by: Bataleon Posted at: 2017-05-11T09:50:06.312Z Reads: 112

```
Is it not possible to flash a bootloader, if needed?
```

---
## \#33 Posted by: TarzanHBK Posted at: 2017-05-11T09:53:42.849Z Reads: 112

```
They often work fine, but you should know, there are better Vescs available. It´s like you get what you pay for.
Without a bootloader, you have to get a St-Link V2 and upload the bootloader and after that the firmware yourself.
```

---
## \#34 Posted by: Maxid Posted at: 2017-05-11T09:56:31.583Z Reads: 118

```
sure but going online and buying an ST-Link, reading up on how the upload works plus performing the upload just to save like 10 bucks? Plus the chances of inferior quality?
```

---
## \#35 Posted by: Bataleon Posted at: 2017-05-11T10:02:08.956Z Reads: 119

```
@TarzanHBK Ah I had no idea extra HW was needed. I often follow the approach “if it ain’t broke, don’t fix it” so can’t imagine needing to upgrade the firmware. BLDC mode is working well at the moment.

@Maxid  On the quality front, Maytech have years of experience manufacturing ESCs for the RC hobby market. So if anything, I would expect their quality to be higher than the small "VESC-only" suppliers. This is pure speculation though.
```

---
## \#36 Posted by: Maxid Posted at: 2017-05-11T10:26:18.287Z Reads: 118

```
Experience on this forum has shown that these chinese VESCs are inferior to the "established" manufacturers.
Also just because you have the experience to make a good product does not mean you actually do when you use cheap parts of lesser quality to put it together.

I don't want to argue but the heart of your vehicle is in my eyes not the place to cheap out on. Get worse wheels that don't cushion vibrations as good or worse trucks that might make handling a little harder - but the VESC controls the entire thing!

Maytech is fine as long as you don't want to use the latest firmware and cutting edge features like FOC
```

---
## \#37 Posted by: Jammeslu Posted at: 2017-05-11T10:32:10.055Z Reads: 117

```
Can somebody breifly explain the bootloader thing about the maytech Vesc? I got one cant i run inte without doing a bootloader?
```

---
## \#38 Posted by: Maxid Posted at: 2017-05-11T10:49:05.177Z Reads: 124

```
bootloader is necessary if ou want to update your firmware with for example @Ackmaniac's version.
If you are fine with the version it came with there is no need for you to update.
```

---
## \#39 Posted by: TarzanHBK Posted at: 2017-05-11T10:54:00.496Z Reads: 125

```
Some infos on how to handle that:
https://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752
```

---
## \#40 Posted by: psychotiller Posted at: 2017-05-11T16:36:18.139Z Reads: 119

```
I plug mine straight into my computer with no stlink and. It works fine with no firmware update.
```

---
## \#41 Posted by: psychotiller Posted at: 2017-05-11T16:40:40.091Z Reads: 117

```
If you think you always need to do firmware updates fine. Get a boot loader. But give people all the info as to why you think you need it and stop just saying they don't work without it, because it just isn't true.
```

---
## \#42 Posted by: TarzanHBK Posted at: 2017-05-11T18:03:19.504Z Reads: 119

```
Sorry for the confusion, but there are patches of maytech vesc here on the forum without any bootloader and firmware.
```

---
## \#43 Posted by: Jammeslu Posted at: 2017-05-11T19:15:15.115Z Reads: 123

```
oh ok thanks, i got may tech vesc from e-green and people has been saying they come without bootloader that is why i was worried
```

---
## \#44 Posted by: Tampaesk8er Posted at: 2017-05-11T20:32:04.017Z Reads: 116

```
I got mine from @psychotiller and its working great, i just did a few tweaks, thanks to @Jinra, i'm still new learning the VESC, alot of learning still to come but also, i've built 2 eboards in 5 months and so far so good thanks to this forum, i'm learning something new everyday.

https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980/73

https://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419
```

---
