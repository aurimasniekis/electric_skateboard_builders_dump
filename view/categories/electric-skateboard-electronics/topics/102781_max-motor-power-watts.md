# Max motor power (watts)

### Replies: 5 Views: 234

## \#1 Posted by: SquidKingRabbit Posted at: 2019-10-10T12:56:54.714Z Reads: 61

```
Hi I am running a Sk8 6364 245kv motor with 6s 8ah 30c lipos.

Am I right to say the maximum power my vesc (4.12) is able to provide is 4.2v x 6s x batt max settings?

Or does my motor max affect the power output? 

For example my batt max is 30amps which means my max power is 4.2 x 6 x 30 = 756 watts (3.7 x 6 x 30 = 666 watts nominal) 

What I want to know is does motor max affect my power output or is it solely dependent on batt max?
```

---
## \#2 Posted by: annihil8ted Posted at: 2019-10-12T06:52:09.169Z Reads: 41

```
The max power your battery is able to output is: W = IV = (8A * 30c) * 4.2 * 6 cells = 6048W. The 30C in this case is the C rating of your battery. Also if we tweak the equation a little Wh = Ah*V = (8Ah * 30C) * 3.7V *6 cells = 177.6Wh. This gives us Wh which is also more or less the capacity/power of your battery in relationship to time.

The max power your vesc will allow to pass through will be set based on your motor max and battery max settings.

The motor max setting is how much current the vesc is allowed to give to your motors.

The battery max setting is how much current the vesc is allowed to take from your batteries.

Because of the flow (battery -> vesc -> motor), whichever has the lowest settings will determine your max output.

So to answer your question, motor max will affect power output if it's the lowest and battery max will affect battery output if it's the lowest.

Edit: Thank you @FredrikHems for pointing out a very dumb mistake I did in my math :+1:
```

---
## \#3 Posted by: FredrikHems Posted at: 2019-10-12T10:21:42.774Z Reads: 31

```
@annihil8ted This is very wrong. 
Formula for max output from battery is (max current * max voltage), which in this case means **( (8Ah * 30C) * (4.2 * 6)) = 6048watts.** 
Now this is theoreticall and does not take into consideration of voltage drop. 

Your Wh calculation is also totally off. 
Wh = nominal voltage of battery (in V)* capacity (in Ah) 
Therefore; **Wh = ((3.7 * 6) * 8) = 177.6 Wh**

@SquidKingRabbit
To answer your question; 
Your max power will depend on duty cycle, but as a general number (max battery voltage * max battery amps) = (25.2 * 30A) = 756W
```

---
## \#4 Posted by: annihil8ted Posted at: 2019-10-12T17:11:58.571Z Reads: 22

```
Sorry you're definitely right. I forgot to multiply by the number of cells. Thanks for catching that! Let me edit my post.
```

---
## \#5 Posted by: SquidKingRabbit Posted at: 2019-10-12T17:20:20.117Z Reads: 20

```
Thanks @annihil8ted @FredrikHems! You both have been a great help
```

---
