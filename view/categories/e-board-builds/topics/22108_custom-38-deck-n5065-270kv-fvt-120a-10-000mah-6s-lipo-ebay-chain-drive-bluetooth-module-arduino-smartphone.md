# Custom 38&rdquo; Deck &#124; N5065 270kv &#124; FVT 120A &#124; 10,000mah 6S LiPo &#124; Ebay Chain Drive &#124; Bluetooth Module Arduino + Smartphone

### Replies: 8 Views: 813

## \#1 Posted by: potatowarrior13 Posted at: 2017-05-01T01:18:48.665Z Reads: 140

```
I have been reading around here, but just want to make sure that these components will have a chance of working. This is my first electric skateboard build but I have experience already in using RC electronics and arduino.
So this is my plan:
I have a custom 38" deck that I have built, it is is a flat deck so it has plenty of clearance.

For the motor I am thinking of using this one in a single drive config - https://www.aliexpress.com/item/New-Arrival-Brushless-Outrunner-Motor-N5065-270KV-1665W-For-DIY-Electric-Skate-Board/32793724521.html
It is on sale for half off, which makes is very inexpensive compared to anything else I can find.

The ESC I want to use is this one - https://www.aliexpress.com/item/FVT-2-6S-LiPo-Battery-120A-Waterproof-Brushless-Car-ESC-For-1-8-1-10-RC/32714867490.html
I have seen other builds using this and it seems like a great choice if you don't have the money for a VESC.

So for the battery I want to have as much clearance as possible under my board, which is why I am looking at using two 10000mah 3S LiPo's in series to make a 6S pack - http://www.ebay.com/itm/ZOP-Power-11-1V-10000mah-3S-25C-Lipo-Battery-W-XT60-Plug-For-RC-Helicopter-Car-/112263064069?hash=item1a23666a05:g:JbcAAOSwnF9Y7II5
It is not a name brand, but I have used ZOP power LiPos on other RC projects and had great results, I have found them to be way better than HobbyKing Zippys, the two Zippy Compacts which I have had have both puffed within a short time of getting them.

For the motor mount I have already ordered this - http://www.ebay.com/itm/252797338872?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
And this - http://www.ebay.com/itm/262844497588?_trksid=p2057872.m2749.l2649&var=561842893377&ssPageName=STRK%3AMEBIDX%3AIT
I have access to a 3d printer at my school so I am planning to 3d print some spacers to go between the wheel and chain sprocket. The one thing I am concerned about is the gearing ratio, it is 14:27, and using RC Calc this gives me a weighted top speed (80% of theoretical) of 20mph (32kph), and I don't know if that single 1665W motor is powerful enough to get myself (65kg, 140lbs) up to that speed.

For control I already have the system mostly sorted out, I am using an HC-06 bluetooth module and an Arduino Uno on the receiving end and my Android smartphone on the transmitting end. I have passed the values coming from the phone's pitch orientation sensor through an exponential smoothing function to eliminate high frequency noise, that data is then sent to the Arduino, which writes it to the ESC. In my small scale tests this setup works great, and is completely customizable, it is your choice as to what you do with the data. The idea is that you will be able to control the skateboard by leaning your phone forward and brake by leaning it backward. If you do not hold down the safety button in the app it will simply put the motor in neutral, if you crash the skateboard won't accelerate out of control lol.

Other components I need are XT60 connectors, 10awg wire, power switch, etc.

So, does this setup look OK for a budget build, I know some people here build insane 12S setups, have very expensive builds, etc. but I don't have that sort of money unfortunately, so does my setup look decent for the price?
```

---
## \#2 Posted by: Sander Posted at: 2017-05-01T02:45:20.286Z Reads: 116

```
I am no motor expert but that motor looks small.
```

---
## \#3 Posted by: potatowarrior13 Posted at: 2017-05-01T03:09:20.684Z Reads: 112

```
What motor would you suggest instead?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-01T03:10:33.156Z Reads: 113

```
If your gonna build a single drive, you need something with more torque like a 6374
```

---
## \#5 Posted by: Sander Posted at: 2017-05-01T03:10:57.635Z Reads: 113

```
Sorry I dont know but I know if the motor is small, it gets hotter fast.
```

---
## \#6 Posted by: potatowarrior13 Posted at: 2017-05-01T03:52:04.965Z Reads: 104

```
do you think that a dual drive with this cheap motor would be good?
```

---
## \#7 Posted by: Namasaki Posted at: 2017-05-01T04:31:13.890Z Reads: 105

```
A dual setup with 50mm motors will work but if your doing that to save money, you will defeat your purpose because you will have to buy another motor controller.
If your trying to stay within a tight budget, then better to do a single drive.
If you need a board that will climb steep hills then your gonna need torque and either a dual with 6355's or a single with 6374.
```

---
## \#8 Posted by: Iam319 Posted at: 2017-05-02T07:49:55.066Z Reads: 89

```
would you or some other knowledgeable person be willing to explain the process of wiring the HM board and how to configure it with your phone? I'd love to be able to use the BLDC app but I am relatively inexperienced with electronics of this sort.
```

---
