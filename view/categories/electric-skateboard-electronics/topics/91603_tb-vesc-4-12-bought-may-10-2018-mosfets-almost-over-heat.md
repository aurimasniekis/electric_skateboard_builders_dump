# TB Vesc 4.12 (Bought May 10 2018) - Mosfets almost over heat

### Replies: 6 Views: 208

## \#1 Posted by: legend27 Posted at: 2019-04-24T14:07:51.054Z Reads: 63

```
Hey everyone!

So my mosfet temperature seems wayyyyy too high. From my understanding most people is somewhere around MAX 40 degrees celsius when riding hard. **My temperature reaches anywhere from 70-85 degrees celsius**. This also causes the board to go from a max speed of 50 km/h to 20-30 km/h (the point where I almost get passed by bicycles :joy:) which luckily saves my vesc from not being toasted.

So after looking around on the forum, it seemed like a few other people had experienced somewhat the same as me with the same vesc bought around the same time. The reason was because of a bad batch. I'm thinking it's the same for me since my settings are not too crazy.

The vesc was bought on the 10 of May 2018 and have been **used for around 125 km in total**, so shouldn't be caused by wear.

There is no hills around me, but I usually like to accelerate as hard as possible

Does anyone have any suggestions?
@torqueboards

**As usual, any input is appreciated and thanks for reading all the way to the end.**


**Vesc settings:**

Video is a bit old, but just realized I had the same issue back then, just never effected speed..

https://www.youtube.com/watch?v=9r7ovni2wDc&amp;t=20s

**Rides:**

Max temperature can be seen upper left for the temperature box in the right top corner.

![IMG_3785|281x499](upload://uQt2HGN8GBBEAL2r9FGEo0ZOiC4.png)
![IMG_3801|281x499](upload://3EsKtjRj6L1xsrQhofxsaly3vHg.png)

![IMG_3877|281x499](upload://bnHdDLcHN9wT5GllRx2ZzHQpQnG.png) 
![image|281x499](upload://lTQ0OsdjvrTfIu1wY2lBkuPCH08.png)

↓↓↓↓ Temperature reached just above cut-off start and got this error code. I got it when I accelerated  as hard as possible. It made the board brake...

![image|281x499](upload://l5vx3MJxfsQmLmzozAILMDMW7u4.png)
![image|281x499](upload://ilzeVHiWLJ6I4U6IRU7NKlnh7Vp.png)
```

---
## \#2 Posted by: Andy87 Posted at: 2019-04-24T14:13:32.417Z Reads: 56

```
I wouldn’t expect something else on a hw 4.12 vesc without extra attached heat sink. I can’t speak out of personal experience but I read that multiple people have over hearing  issues when setting bat max to 30-35 A or above. That was reported from different producer. Tb, Flipsky 4.12, hobbyking etc.
```

---
## \#3 Posted by: legend27 Posted at: 2019-04-24T14:33:15.720Z Reads: 53

```
Will try to set it lower :slight_smile:
Thanks

Then time to look for an old school focbox :money_mouth_face:
```

---
## \#4 Posted by: Mobutusan Posted at: 2019-04-24T15:26:09.711Z Reads: 44

```
What kind of wheels are you using? If they have high rolling resistance that could be your culprit.
```

---
## \#5 Posted by: legend27 Posted at: 2019-04-24T15:46:05.793Z Reads: 42

```
@Mobutusan Both on 90mm and 97mm wheels I get high temperatures. The temperature is a bit higher with 97mm though. Gearing is 16/36
```

---
## \#6 Posted by: legend27 Posted at: 2019-04-24T20:20:12.321Z Reads: 30

```
Changed my settings to:
- Motor max: 65A
- Motor min: -65A
- Batt max: 27A
- Batt min: -8A
- Max wattage: 1300W

I still got really high temperatures.

Even when riding 23 km/h with 20A for motor and 10A battery the temperature was still at 80 degrees celcius the whole time??? Wtf

![image|281x499](upload://eMucDXzgdNq8gkHIfjU8yGJ4zzo.png) 

Also got the same error code as before when I reached max temperature which could have thrown me off (almost did)

![image|281x499](upload://oYuLKBH8zl216jGrjSv6cx5seot.png) 

Here is the whole ride:
![image|281x499](upload://dqjrukvev9O9Q8aytfLK2F7jdUG.png)
```

---
