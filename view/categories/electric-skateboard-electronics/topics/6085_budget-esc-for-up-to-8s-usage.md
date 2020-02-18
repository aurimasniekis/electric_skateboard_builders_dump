# Budget ESC for up to 8S usage

### Replies: 27 Views: 4574

## \#1 Posted by: Leonardvdj Posted at: 2016-07-14T09:44:35.804Z Reads: 184

```
Hi!

As I don't have money for a VESC(€170 here in Europe...), I'm wondering what budget options there are for a 6S battery.
It would be nice if it had the capability of 8S, since that would later give me the option of switching to 8S for some more power :slight_smile:
Which features does a Car ESC have, that a normal "plane" ESC doesnt have? Just regenerative braking?

Regards,
Leonardvdj

EDIT:
Am i right to assume that an esc of 80Amps or above will be plenty for the Turnigy G160 245Kv? The HobbyKing page says "Max Current: 60A"
```

---
## \#2 Posted by: bigben Posted at: 2016-07-14T14:50:23.649Z Reads: 172

```
I don't know that there is something such as a cheap 8s. 
If you find one let me know! The fvt 120 from bangood is cheap enough to go for 6s to start with.
```

---
## \#3 Posted by: psychotiller Posted at: 2016-07-14T15:14:45.820Z Reads: 170

```
You need the functions of a car ESC  on a board. You will be asking for trouble using a plane or heli ESC.

Those escs dont have the capability to provide linear/progressive braking. The brakes will either be DRAG/Full on/or off. That is dangerous on a board
```

---
## \#4 Posted by: Leonardvdj Posted at: 2016-07-14T17:45:02.461Z Reads: 152

```
@psychotiller http://www.ebay.de/itm/Hobbywing-Ezrun-BL-ESC-MAX8-V3-150A-1-8-T-Plug-Regler-HPI-Traxxas-Arrma-/152100704519?hash=item2369e89107:g:4zkAAOSwQaJXQuLc Would this be fine for 6S then? :slight_smile:
```

---
## \#5 Posted by: Leonardvdj Posted at: 2016-07-14T18:00:27.139Z Reads: 142

```
@Psychotiller I'm trying to shave off as much as possible though, and that EZRun esc is very expensive compared to the HobbyKing BlueSeries 85A... Will any car esc work?
```

---
## \#6 Posted by: psychotiller Posted at: 2016-07-14T18:53:06.640Z Reads: 136

```
Yup! That would work
```

---
## \#7 Posted by: maxchilton Posted at: 2016-07-14T20:37:12.087Z Reads: 129

```
If you find a decent 8s esc that works with eboards please post it. lol
```

---
## \#8 Posted by: Leonardvdj Posted at: 2016-07-14T20:59:59.622Z Reads: 125

```
@Psychotiller For electric longboards, what are the cons of a boat esc compared to a car esc?
```

---
## \#9 Posted by: psychotiller Posted at: 2016-07-14T21:37:36.805Z Reads: 124

```
Again, boats don't brake like cars.
```

---
## \#10 Posted by: bigben Posted at: 2016-07-14T21:51:43.761Z Reads: 120

```
http://m.banggood.com/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-p-985970.html
```

---
## \#11 Posted by: Leonardvdj Posted at: 2016-07-14T22:07:42.234Z Reads: 122

```
@bigben With Denmark's customs, I'm better off buying something more expensive here in Denmark.
```

---
## \#12 Posted by: Leonardvdj Posted at: 2016-07-14T22:08:05.262Z Reads: 120

```
@psychotiller What about the HobbyKing X-Car? Its only €46, and does 2-6S, 120Amps.
```

---
## \#13 Posted by: psychotiller Posted at: 2016-07-14T22:09:59.458Z Reads: 113

```
Don't know about that one...try it
```

---
## \#14 Posted by: Leonardvdj Posted at: 2016-07-14T22:10:25.836Z Reads: 110

```
@psychotiller Yeah alright, thanks for the help nevertheless :thumbsup:
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-07-15T06:23:57.184Z Reads: 106

```
[quote="Leonardvdj, post:12, topic:6085"]
What about the HobbyKing X-Car? Its only €46, and does 2-6S, 120Amps.
[/quote]

Mhm?
Where did you find that ESC? I just saw a Hobbyking X-car 2-3S ESC
```

---
## \#16 Posted by: Leonardvdj Posted at: 2016-07-15T09:14:04.080Z Reads: 103

```
@DeathCookies It's the X-Car "BEAST", http://www.hobbyking.com/hobbyking/store/__77144__HobbyKing_174_8482_X_Car_Beast_Series_ESC_1_8_Scale_120A.html
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-07-15T09:16:32.336Z Reads: 107

```
Okay thank you!

I had seen this before but i am sceptical:
The description says: Suitable Motor Type : 4 Pole sensorless and sensored brushless motor

I dont think it wont fit with our big motors unless you have a sensored motor?
Please correct me if i am wrong!
```

---
## \#18 Posted by: Leonardvdj Posted at: 2016-07-15T09:18:34.560Z Reads: 104

```
@DeathCookies it does say "sensorless AND sensored", so it should work with our sensorless motors.
http://www.electric-skateboard.builders/t/green-cobra-generic-ebay-deck-custom-trucks-sk3-6374-192kv-custom-mount-6s-x-car-beast-120a/2312 This guy is using the X-Car Beast 120A, and he doesnt seem to have any trouble with it.
```

---
## \#19 Posted by: DeathCookies Posted at: 2016-07-15T09:20:25.776Z Reads: 102

```
If i had known this earlier i wouldnt have bought a heli esc... :weary:
```

---
## \#20 Posted by: Leonardvdj Posted at: 2016-07-15T09:23:04.876Z Reads: 100

```
@DeathCookies Have you used the ESC yet(The heli esc), or have you just ordered it? How is it riding without brakes, is it completely impossible or?
You could ofcourse either 1) Return the ESC, or 2) Buy an arduino, put that between the receiver and ESC, and then make it have a throttle curve, but that'd require you to know a bit of coding and such.
Easiest is probably to just return the esc, depending on shipping costs
```

---
## \#21 Posted by: DeathCookies Posted at: 2016-07-15T09:33:55.910Z Reads: 100

```
I am already using the YEP 6S 120a ESC since 1-2 months.
I am software developer so i could dig into it and make it happen but i dont have the time for it...

Who says that the ESC does not have brakes? That is a bad lie! It has brakes but they are not very comfortable. You have to get used to the ESC but it works without problems. If i brake to hard it will throw me off the board.... So i need to learn to brake with this ESC more gently.
```

---
## \#22 Posted by: DerBrecher Posted at: 2016-07-15T12:58:15.579Z Reads: 97

```
I am using the X-Car Best 120A ESC and it is perfect for the price. I ordered the programming card and set the breaks to 70% and it is working like a charm. The only issue i had so far was with the voltage cut-off because it has no soft off. When i was going up hill on medium throttle the voltage dropped under 3.4V/Cell limit I had set. Therefore the ESC turned off and i fell from the Board.
```

---
## \#23 Posted by: DeathCookies Posted at: 2016-07-15T13:00:51.899Z Reads: 96

```
[quote="DerBrecher, post:22, topic:6085"]
it has no soft off.
[/quote]

That sounds like a no go! Just like you said: [quote="DerBrecher, post:22, topic:6085"]
Therefore the ESC turned off and i fell from the Board.
[/quote]

It is way to risky without soft cutoff or you need to be best friend with you battery and know when it is depleted... but that is kinda hard. like @whitepony says: Make a max speed check to see if they are depleted
```

---
## \#24 Posted by: DerBrecher Posted at: 2016-07-15T13:33:00.056Z Reads: 91

```
I got have a Voltmeter in the Cut Out of my front Trucks so i can keep track of the voltage and know how hard i can push the board. I lowered the Cut-off voltage to 3.0V/Cells and since then i had no problems. Just make sure to order the programming card so you can change these settings, if you are going to order this ESC. 

And i dont think that many cheap Car ESCs have a soft off when the battery gets low. Why would they have such a thing your RC Car.
```

---
## \#25 Posted by: Leonardvdj Posted at: 2016-07-16T02:34:42.123Z Reads: 85

```
@DerBrecher Which programming card did you order for the x-car? The USB one, the small lcd one, or the thing you can use your phone for?
```

---
## \#26 Posted by: DerBrecher Posted at: 2016-07-16T10:34:51.682Z Reads: 75

```
@Leonardvdj [This one](http://www.hobbyking.com/hobbyking/store/__77150__HobbyKing_174_8482_X_Car_Beast_series_LCD_Program_Card.html) and used the PC Tool provided in the download section.
```

---
## \#27 Posted by: Leonardvdj Posted at: 2016-07-16T10:49:42.511Z Reads: 71

```
@DerBrecher Dang, on backorder..
EDIT:
Other than the voltage cutoff(Whats the default?), was there anything you had to change?
2nd EDIT:
Random question, how many metres of 10awg wire should i buy for an electric longboard with the length of 33"? Is 1 metre of black and 1 of red enough, or should i get 2 of each?
```

---
