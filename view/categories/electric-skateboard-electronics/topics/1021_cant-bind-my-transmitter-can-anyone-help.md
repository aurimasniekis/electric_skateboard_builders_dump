# Can&rsquo;t bind my transmitter - Can anyone help?

### Replies: 21 Views: 3788

## \#1 Posted by: Turkeybird Posted at: 2016-01-17T04:49:00.490Z Reads: 106

```
I just bought everything but the deck for an AT board from a guy, and I'm wondering if anyone recognizes the brand of controller and remote. I can't get the transmitter to bind with the receiver, and I hope that someone can give me some tips. It's 36v/800watts, and I'm using a 10 s LiPo to power it up. Basically, I've just applied power, I push the button on the controller, two red LED's on the controller come on, I power on the transmitter, the transmitter gun beeps and a red LED comes on, I pull the trigger, and nothing. Anything else that I might try? I really don't know where to look for binding instructions because I don't even know the brand. The only mark that I see is xkate on the rx board, but it doesn't look like an Altered controller/tx. Here are pics
<img src="/uploads/db1493/original/2X/0/010a727bc188694c8bc9fae1956347553b0997fd.jpg" width="375" height="500">
```

---
## \#2 Posted by: cmatson Posted at: 2016-01-17T04:53:04.951Z Reads: 103

```
[quote="Turkeybird, post:1, topic:1021"]
if anyone recognizes the brand of controller and remote
[/quote]

it's one of the ones that come with most generic Chinese boards rebranded by other companies (like Fiik for example). 

Unfortunately, I don't have any experience with one of these remotes, but I am sure someone here on the forum has.
```

---
## \#3 Posted by: Turkeybird Posted at: 2016-01-17T04:54:59.295Z Reads: 103

```
Thanks man. I'm hoping so.
```

---
## \#4 Posted by: mostwanted Posted at: 2016-01-17T05:28:14.562Z Reads: 100

```
see that aluminium thin metal strip at the hand held remote controller ? thats a sensor , if you're not holding it , it wont move . also , theres a close range sensor on the board it self , if you're not standing on it , the motor wont spin . 
in total , if you're  not close enough , it wont move .

or..... try carefully pry open the hand held remote controller , if tiny wire is cut off from the thin alluminium strip , or the strip is peeled off , there's no connection . the remote wont send signal to reciever .
```

---
## \#5 Posted by: Turkeybird Posted at: 2016-01-17T05:39:17.024Z Reads: 90

```
Is the close range sensor something that is built into the receiver? I used my own deck. would it not work if I have the board on its back with the tx right over the rx?
```

---
## \#6 Posted by: Turkeybird Posted at: 2016-01-17T06:17:11.121Z Reads: 87

```
I tried on the board, and checked the wire, and it doesn't work still. I need to find out if the tx/rx is bad, or the speed controller. Are these speed controllers set up to use hall effect sensors, or pwm? it's a brushed dc motor controller, but since there's only 12v going to the rx it's hard for me to tell.
```

---
## \#7 Posted by: psychotiller Posted at: 2016-01-17T06:33:30.924Z Reads: 74

```
I think the brand is emad and 10s may be too much voltage.
```

---
## \#8 Posted by: Turkeybird Posted at: 2016-01-17T06:42:39.601Z Reads: 72

```
It's a 36v controller, and It hasn't left the bench with a pack that's putting out 37v right now. They come with 3 12 SLA batteries. A 12 v SLA charges to 14v. Thats 42V charged with the batteries that they come with, so a 10S shouldn't be too much. They charge to 4.2/cell... same voltage
```

---
## \#9 Posted by: Turkeybird Posted at: 2016-01-17T06:50:44.218Z Reads: 71

```
I just read the Emad instructions... Clearly some traditional Chinglish there.. the instructions aren't any different than what I've done, and the same points that mostwanted made to me were mentioned. stand on the board, and keep in contact with the foil ( checking wire connection being a reasonable follow up )
```

---
## \#11 Posted by: Turkeybird Posted at: 2016-01-17T14:15:57.164Z Reads: 66

```
I guess that I may be in the market for a used controller until i figure this out.
```

---
## \#12 Posted by: dogeatgod Posted at: 2016-01-17T19:23:27.676Z Reads: 60

```
Ah that link I gave has been blocked. It was a link to a supplier of the same controller/board as yours. I recently bought one of these off ebay to convert - the electronics will be surplus to requirement, you're welcome to them with the remote control if you get stuck.
```

---
## \#13 Posted by: Turkeybird Posted at: 2016-01-17T22:11:12.087Z Reads: 56

```
That's awesome! I'm stuck. I would really appreciate it.
```

---
## \#14 Posted by: mostwanted Posted at: 2016-01-18T00:12:33.443Z Reads: 55

```
<img src="/uploads/db1493/original/2X/e/ec1b82eb26f599186e953cead2a752a3415bf6ad.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/e/efcb18270e93beb5373f302f73967bda057171c8.jpg" width="666" height="500">

...my previous eboard was officially a 24V . i dont know why yours is a 12V . check again . maybe ,...... just maybe yours is also a 24V .

as you can see from photo . i bought me a 36V emormous power supplier . and hook it up to power my supposedly 24V dc eboard . waited for half an hour . when i saw the capacitor a holding on pretty safely . i concluded the whole system can take the heat of an awesome 36V LI~ION . and i was satisfied . but the motor got burnt up easily . well , it burnt EVEN B4 i installed the 36V li~ion .

 <img src="/uploads/db1493/original/2X/8/89a4ff47753e806a579df5d8558403fc4c9ee3d5.jpg" width="666" height="500">
```

---
## \#15 Posted by: cmatson Posted at: 2016-01-18T00:19:29.760Z Reads: 50

```
I suggest creating a build thread showing how you've updated some of the parts on your eboard!
```

---
## \#16 Posted by: Turkeybird Posted at: 2016-01-18T01:03:49.578Z Reads: 51

```
I love that rig! I don't think that I was clear before. The motor-controller-tx/rx are made for be 36v. It's just the power to the rx from the controller is 12v. I'm not over-volting. I just mentioned that because I was trying to test to figure out where my problem was. I'm pretty sure that the rx is the weak link there. I was poking around on the site, and saw your battery boxes... awesome! Now I can see what motivated you to build them!
```

---
## \#17 Posted by: Turkeybird Posted at: 2016-01-18T01:54:50.607Z Reads: 48

```
Mostwanted, I had  confused you with psychotiller, He makes those nice battery boxes. I'm guessing that my reply confused you.
```

---
## \#18 Posted by: mostwanted Posted at: 2016-01-18T01:57:13.407Z Reads: 47

```
no problem .
wasnt confused 
 i was just sharing my pics . just trying to encourage you to switch to lithium ion batteries for ultimate satisfactory :smiley:
```

---
## \#19 Posted by: Turkeybird Posted at: 2016-01-18T02:00:35.547Z Reads: 49

```
I am. Currently I've got a 10S 8amp pack from one of my multirotors on board. I just discovered electric skateboards about a month ago, and now I'm on my 2nd one, and hooked. I'm looking forward to building something sweet when I have a little extra cash to do it.
```

---
## \#20 Posted by: psychotiller Posted at: 2016-01-18T03:17:47.370Z Reads: 49

```
Thanks @Turkeybird! Let me know if you decide you want me to make you one
```

---
## \#21 Posted by: Turkeybird Posted at: 2016-01-18T04:33:39.052Z Reads: 51

```
When I can afford it for sure!
```

---
## \#22 Posted by: dogeatgod Posted at: 2016-01-18T08:24:48.613Z Reads: 45

```
No worries @Turkeybird - I'm going to convert board in next couple of weeks so can send bits then. I'm UK so will take a little while to get to you. PM address.
```

---
