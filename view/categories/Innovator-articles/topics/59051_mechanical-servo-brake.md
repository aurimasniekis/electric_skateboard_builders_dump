# Mechanical servo brake

### Replies: 13 Views: 747

## \#1 Posted by: NeverStopSeeking Posted at: 2018-06-15T21:29:55.982Z Reads: 213

```
Hi guys, I have a cheap 1 motor setup with not a really great breakinh power coming  from this single motor.
Since acceleration and top speed are great I didn't want to go for a dual motor setup so I tried this brake implementation.



With my weight going at 30km/h  pushing the brake causes the wheel to stop immediately and giving a great stoppng power which finally gave me a great security riding my board to stop in really small spaces on cases of need.
```

---
## \#2 Posted by: chinzw Posted at: 2018-06-15T21:31:17.794Z Reads: 204

```
you jumped the gun on the pic upload
```

---
## \#3 Posted by: NeverStopSeeking Posted at: 2018-06-15T21:35:30.178Z Reads: 200

```
Sir you are right. I reupload we them
```

---
## \#4 Posted by: chinzw Posted at: 2018-06-15T21:38:10.354Z Reads: 195

```
I like your idea, i wish it was 100% mechanical. Ever since i had my board go max speed out of control i've been looking for a failsafe way of breaking.
```

---
## \#5 Posted by: Wilsonliang777 Posted at: 2018-06-16T02:53:14.993Z Reads: 179

```
If you have time pls post a video of how it work.  I also have a single drive board too.  I had to bail out once when I attempted to stop on a slop.    I purchased a use frogstop but I have not installed it yet.
```

---
## \#6 Posted by: Acido Posted at: 2018-06-16T08:30:43.541Z Reads: 155

```
I think you will be changing a lot of wheels and that rubber
```

---
## \#7 Posted by: baxter Posted at: 2018-06-16T08:43:02.586Z Reads: 150

```
I thought @Brakeboard solved that problem.  I must admit I haven't seen anyone use their braking truck design on the front of their board.
```

---
## \#8 Posted by: NeverStopSeeking Posted at: 2018-06-16T09:27:46.732Z Reads: 147

```
Brakeboard is great but too much expensive, and you still have to change your foot position to brake, which in case of emergency may not be very practical.

I wanted to make something connected with the same throttle channel of my transmitter so that when I brake it automatically activates both the brake of the motor and the mechanical brake.

So I just have to brake on my transmitter and I can totally focus on maintaining the balance and avoiding the obstacle.

My solution is very cheap also, you only need a cheap 20kg servo (20€) and 6€ worth of steel and aluminium, an old bike inner tube and a couple of hours with the drill press, angle grinder, hammer,  vise, files and contact cement and you are done.

I could not justify spending 500+ euros on a brakeboard truck while my overall board cost is 350€ , so I found this solution that works great for my needs :slight_smile:
```

---
## \#9 Posted by: NeverStopSeeking Posted at: 2018-06-16T09:30:17.508Z Reads: 130

```
Yeah I think also , but I can get four 100mm wheels for 35€ and changing the rubber is a 10 minute process.
For the added security I am happy to trade a change of wheel and rubber  :slight_smile:
```

---
## \#10 Posted by: NeverStopSeeking Posted at: 2018-06-16T09:31:53.833Z Reads: 128

```
What happened? You lost radio signal from transmitter? You electronics went mad?
```

---
## \#11 Posted by: Okami Posted at: 2018-06-16T11:17:05.658Z Reads: 121

```
It is great someone finally made such a system on forum and it looks like u made your own version of it.

As i understand, the servo arm pulls down yhe plate and rubber at that moment, gets pushed against the wheel?

Also.. do u still have motor brake enabled? Do they brake evenly or now with this mechanical brake it is enough to stop?

How do u pass the signal to servo anyways? Do u just plug another cable in receiver or what?.

Curious to find out more..
```

---
## \#12 Posted by: NeverStopSeeking Posted at: 2018-06-16T17:49:46.682Z Reads: 102

```
Yes the servo arm pulls down the curved plate that pushes on the wheel. The lever is designed to have a mechanical advantage of 1:3.

Motor brake is still enabled  and they work wonderfully together .

The signal to servo goes through an Arduino first which filters the signal and only the braking signal goes to the servo.
```

---
## \#13 Posted by: Riako Posted at: 2018-12-30T18:28:24.246Z Reads: 61

```
plop,

if I understand well, _are going to make / did you make_ something like this !?? :star_struck: 
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/8373?u=riako

Maybe it already exists? Does anyone have a thread in mind? 
thx :v:
```

---
