# 10s4p amp output

### Replies: 10 Views: 207

## \#1 Posted by: JoelMatousek Posted at: 2019-07-15T00:02:44.978Z Reads: 76

```
This might be a silly question, but this is my first actual build and I just want to make sure everything is right. I built my own 10s4p liion battery pack using 30q and I ran the setup wizard on the vesc tool. It said I was pulling about 70.1 amps, which I guess is about 10 amps more then what those batteries are rated to discharge. My question is, should it be different? Since this is a diy pack I want to make sure that each battery connected in parallel is actually connected, and I thought that by checking the amp output I should be able to determine whether or not any batteries aren't connected. So did anyone else get an amp output different then me with a 4p pack? Or is there another way I can make sure that every individual battery is connected?
```

---
## \#2 Posted by: Tinp123 Posted at: 2019-07-15T07:13:15.966Z Reads: 59

```
No, you got it wrong. cells by itself won't limit amp draw, there has to be something else, like bms or vesc. you could draw 50 amps from one cells and most probably that will destroy it.

30Q can output up to 20amps. 10s4p is okay with 80 amps discharge, but you will rarely draw so much, and it will be for very short period. it depends on your weight, tires/wheels, riding style, terrain. to many factors to just say that "70 amps is average draw" :)

what do you mean you are not sure if all cells are in parallel?!? do you know how dangerous it could be if they are not connected good, and due to vibrations, in the middle of your ride, one disconnected cell connects back in parallel with other cells of different voltage? they will balance in split of second and your battery pack will explode! you have to be absolutely  sure that every cell is connected permanently!
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-07-15T08:31:32.136Z Reads: 53

```
Frankly, the questions you're asking tell me that you don't have a thorough understanding of the workings of the board you built, and that makes me very nervous to hear you built a battery pack yourself. This is some seriously powerful and potentially dangerous shit if you don't have a very clear understanding of how everything behaves, and I don't think you do.
```

---
## \#4 Posted by: ESK8MTL Posted at: 2019-07-15T08:44:13.017Z Reads: 49

```
FOR REAL don't mess with what you don't understand.... goodluck on putting out the fire tho   :joy:
```

---
## \#5 Posted by: JoelMatousek Posted at: 2019-07-15T10:22:38.141Z Reads: 44

```
Here's the problem with you guys, first of all. If it catches fire, worst comes worst I lose my money. I have taken many precautions to make sure that even if it does catch on fire it won't be near anything flammable, it's currently in my basement surrounded by bricks. Second, I don't plan on riding it until I know the battery pack is safe, which is why I came here. Third, I understand that it's not going to always pull 70a, I understand that it will pull less and more amps, I was just curious because I don't understand how this vesc determined that number. Fourth, do you really think that if you tell someone to stop, they're just going to throw away a $300 battery? No, instead they're going to figure it out, so instead of wishing the worst upon me, why don't you just help? Is it really that hard for you people to be nice?
```

---
## \#6 Posted by: JoelMatousek Posted at: 2019-07-15T10:28:05.501Z Reads: 38

```
Also, I have decided to do full charge to full discharge at least twice (staying in the liion voltage limits) while monitoring the voltage of each pack to make sure nothing is wrong.
```

---
## \#7 Posted by: Tinp123 Posted at: 2019-07-15T11:07:29.511Z Reads: 35

```
first,  it is not just about you, if your battery catches fire somewhere on the streets, it will affect all of us! esk8 will become "dangerous" and "explosive" and we all could be banned from streets because of people like you. sorry if I sound rude, but you have to think about other people too. 

second, there is a big big difference in charging/discharging battery in your basement and while riding your skateboard. conditions are very different and while your battery can survive 10 circles in your basement, maybe it won't hold through one discharging circle on streets, when shaking and vibrating. 

third, what do you mean how vesc determines how much amps it draws? well it draws as much draws as it needs, depending on many factors I mentioned before and how hard you pull the trigger. 

do you have any photos of your battery build and your welds? many people want to help you, just show us what you got.
```

---
## \#8 Posted by: JoelMatousek Posted at: 2019-07-15T11:11:25.495Z Reads: 31

```
What I meant was, in the setup of the vesc, the prompt said "70.1 amp draw." Since I don't know if that was how much it decided to pull, or if that was what it needed to pull to do that specific test.
```

---
## \#9 Posted by: JoelMatousek Posted at: 2019-07-15T11:46:30.008Z Reads: 32

```
Also, I live in a rural part of Ohio. No one cares what happens here
```

---
## \#10 Posted by: ESK8MTL Posted at: 2019-08-07T09:54:19.010Z Reads: 15

```
They may not care there but they will everywhere else. you should've just bought a prebuilt pack if you dont know what your doing....
```

---
