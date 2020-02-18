# Hub motor pin out different from Direct Drive :frowning:

### Replies: 4 Views: 113

## \#1 Posted by: tung Posted at: 2020-01-09T02:36:07.126Z Reads: 34

```
I have a Meepo that i would like to swap out the hub motor with direct drive.
upon opening the Meepo, i see the wiring colors are off by 1 sequence as seen here https://imgur.com/gallery/hU8gEeb: 

**Meepo wire bundle has:**
black
green
blue
yellow
red

**DD has:**
black
blue
green
yellow
red

can i just plug the DD into the Meepo's ESC? OR i have to swap to match the Meepo sequence?
pls help
```

---
## \#2 Posted by: ZachTetra Posted at: 2020-01-09T02:49:17.443Z Reads: 32

```
The Meepo hub ESC is designed for a specific motor kv, most likely 75kv, so anything with a different kv will not run optimally, although it will still behave.  The phase wires (3 big current carrying wires) can be swapped and that will change direction; the sensor wires (5 or 6 small wires) can be swapped to a degree, the middle 3 color wires are hall effect sensors and can be swapped which will also change the direction the ESC expects the motor to turn.  If the motor is running sensored but just vibrates when you press the throttle, you will need to swap the connections, I recommend getting it to run the right direction sensorless, then changing the sensor pins to match (you can use a needle to pick the jst apart to easily change the pins

BTW the link is broken
```

---
## \#3 Posted by: tung Posted at: 2020-01-31T18:07:28.420Z Reads: 11

```
thanks!
i am running it without sensors. acceleration is rough. sometimes the motor would not even move so i would have to manually kick before the board will move.
```

---
## \#4 Posted by: MysticalDork Posted at: 2020-02-01T02:27:08.855Z Reads: 5

```
That is common for sensorless setups, especially hub/dd ones. The new vesc tool release that includes HFI may help though, time will tell.

It is also possible to carefully remove the contacts from the plastic plug and reinsert them the correct order.
```

---
