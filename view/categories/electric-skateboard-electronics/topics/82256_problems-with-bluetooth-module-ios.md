# Problems with Bluetooth Module (iOS)

### Replies: 11 Views: 309

## \#1 Posted by: Muffe Posted at: 2019-01-27T12:24:29.334Z Reads: 74

```
I am currently having issues connecting my focbox to my hm-10 module. 

My wiring is like this:
VCC-5v
GND-GND
TX-RX
RX-TX

I am using the Xmatic app and I am on iOS, the module just flashes red and doesn’t show up in the app or the Bluetooth settings. It does however show up on my Laptop for some reason. Any suggestions on how to fix this?
```

---
## \#2 Posted by: pjotr47 Posted at: 2019-01-27T12:34:44.649Z Reads: 67

```
Baud rate correct? + on what vesc are you using it?
```

---
## \#3 Posted by: LEE Posted at: 2019-01-27T12:46:28.045Z Reads: 63

```
Try baud rate 9600or 115200.
Try BLE Scanner App.
In my case, iOS recognized BT by using BLE Scanner App.
```

---
## \#4 Posted by: Muffe Posted at: 2019-01-27T16:14:02.290Z Reads: 54

```
The BLE app recognizes it and I am able to connect it to my phone, however, it still says Searching for device even though it is connected in my Bluetooth settings.
UPDATE: Status is now ''Connecting to vesc''
```

---
## \#5 Posted by: Andy87 Posted at: 2019-01-27T17:19:13.941Z Reads: 45

```
Do you have a second app using for Esk8 data on your phone?
I had issues once as the bt signal was used by an other app.
```

---
## \#6 Posted by: Muffe Posted at: 2019-01-27T17:36:47.563Z Reads: 43

```
I only have one app that that uses the Bluetooth signal.
```

---
## \#7 Posted by: LEE Posted at: 2019-01-27T19:26:45.474Z Reads: 39

```
https://www.electric-skateboard.builders/t/vesc-ios-bluetooth-app/53479/350

Did you try this?
```

---
## \#8 Posted by: Nubasaurus Posted at: 2019-01-27T21:56:34.798Z Reads: 31

```
> 
I had to use the BLE app to find mine also. Make sure connect and select it under settings in Xmatic afterwards.
```

---
## \#9 Posted by: Muffe Posted at: 2019-01-28T09:17:56.765Z Reads: 26

```
Yeah that was my problem, after playing around with the app for like 30min I realized that the Bluetooth module had unselected itself in the BLE app. After i selected it and played around some more with the Baud Rate it works!
```

---
## \#10 Posted by: Nubasaurus Posted at: 2019-01-28T09:22:16.091Z Reads: 22

```
Awesome. Glad you got it sorted out. Took me a while but it was a relief when I figured it out. It’s odd that iOS doesn’t list BLE devices under settings and we have to use a 3rd party app.
```

---
## \#11 Posted by: Muffe Posted at: 2019-01-28T09:26:13.655Z Reads: 22

```
Yeah, sometimes I really want to change to android just because of such small inconveniences.
Btw the reason that it was important to figure out the Bluetooth module is s that I can limit the speed. I have been invited by these people https://www.kongsberg.com/ More specifically to the weapon factory to present my board for the public and I don't really want anyone to hurt themselves. Here are some pics of my board. 
I want to somehow represent the Esk8 community but i don't know how, should i give out business cards? I don't know why i am asking for your help but you seem knowledgeable.
![IMG-6898|375x500](upload://z7rYTKiexJDeqSSMpzQ7waL0AIJ.jpeg) ![56971137511__2D7819AE-F429-46D0-9794-C21B85DD91CE|374x500](upload://dOchPcJhk2T3Z2SrKBSXQMsuucx.jpeg)
```

---
