# Simple Esk8 remote from SolidGeek in a smaller version with bigger screen - my journey

### Replies: 1 Views: 189

## \#1 Posted by: StefanMe Posted at: 2018-10-16T18:32:57.691Z Reads: 90

```
Hi guys!

At first I wanna thank u all for the great content in this forum. Didn't expect to waist so much time here :stuck_out_tongue:

I use the remote from @solidgeek for a while and its awesome. I love to check my battery or currents all the time without  pulling out my phone from the pocket while riding. I design a PCB in the last weeks, but was still not happy with the huge amount of complications with wiring and soldering... my PCB is work out ok, but I still have an issue with the power supply and and space inside. Was a cool silent project for me. The feather m0 didn't get out of my head, so I decided to order one and take a closer look. Its an awesome package with nearly everything build in... M0 Cortex Chip, IOs, USB for charge and programming, ON/OFF function with simply pulling an input to ground... cool piece of electronic. I never went deep into programming except of my work where I programmed a lot od PLC stuff (Beckhoff and Siemens), but I tried...

And no proudly... I can say IT WORKS! I ported all the code by nearly writing the lot of new code to the Feather M0. I designed the case a little bit shorter and it looks fantastic with the new bigger display.

The milestone for me, why I now publish this piece of art, is that I was able to communicate safely with the board with a customised key to make it safe while riding with the same remote next to it. While the remote boots up the first time u power it up, it generates a 16byte encryption key and add a boardID at the byte 16. So in the future u can also ride different boards with unique IDs and be safe. U just change the boardID on the remote and go on.

Everything is still under hard development and definitely not ready to ride, but I am looking forward to realise the code within the next 2 weeks for people who want to experiment with it and give feedback!

A big thanks to @solidgeek for the basic code and the basic idea. Hope u can enjoy my work. If I am finished with this project I ll send u one package to hopefully enjoy it. 


PS: sorry for my incredible good english... I am from germany. And yes... I love beer.

![IMG_6498|375x500](upload://8pRcosH4mCle9TUYpFmWcRLXvK0.jpeg) ![IMG_6495|375x500](upload://oExX2FVAT8wFz8qmJguBcyFRAT6.jpeg)
```

---
