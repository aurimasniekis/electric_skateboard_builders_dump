# Can Vesc setting short a motor? (Problem solved)

### Replies: 10 Views: 1247

## \#1 Posted by: Cube Posted at: 2016-03-31T20:13:45.950Z Reads: 126

```
Brand new build with Vesc from chaka.
8s tacon 160 245kv 16/36 80mm wheels
Made it about five hundred feet on flat ground and motor mount came loose/ belt started to slip. 
Walked back home tightened everything up and tried to start the motor. First pull on the trigger it spun good second pull and a puff of smoke came out of the windings. Shorted motor. Now it only twitches forward then backword. Sooo... I ordered a new motor but I'd really like to not repeat this.
My best guess is that the motor was slipping long before I noticed it and caused it to overheat or I didn't properly configure the vesc.
With the vesc I basically just hit the read configuration and the motor spooled up then hit write configuration and setup the transmitter. Are there more changes I should have made in the bldc tool. It's all rather foreign to me. One other thing I did with this build was cut the motor wires about an inch outside of the housing and soldered on silicone 10awg 200c wire for more flexible motor leads. Maybe this could have caused an issue. Thanks in advance for any advice.
```

---
## \#2 Posted by: chaka Posted at: 2016-03-31T20:41:19.855Z Reads: 123

```
Hey Jason,

Tried calling you but no answer. When you calibrated your bldc settings did you hit the "apply" button before writing config?

When you cut your motors phase wires did you make sure you burned off all the enamel and get every strand of wire soldered?

Are your connections secure?

In my opinion the symptoms point to a bad phase wire connection. the good news is you can probably just improve the solder job where you cut them short and have your board running again. The initial run likely melted the weak connection. I have seen the same thing happen with other users and cold joints from trying to solder connectors with a little iron.
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-04-01T06:29:38.395Z Reads: 105

```
Did you run a motor detection?
```

---
## \#4 Posted by: Cube Posted at: 2016-04-01T13:57:46.287Z Reads: 98

```
Problem solved. Thanks chaka. When cutting and replacing the stiff motor wires I didn't get the enamel completely removed. Unsoldered everything and torched the wired to burn of the enamel then buffed them with a dremel. Everything works great now.
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-04-01T14:20:58.378Z Reads: 89

```
This is why i don't go all the way into the winding when i replace my phase leads. I cut the existing leads at the housing and leave just enough wire hanging out to make a butt-joint between the existing 12 or 14 gauge lead and the 10 gauge silicone leads i like to use. Then i heat shrink the individual connections, and after that, add another layer of heat shrink to bunch all three leads together for about an inch past the housing to give them direction. 

but i'm also not replacing them because i'm worried about the current they're handling. I'm doing it because i need the leads to curl and bunch in a very particular way due to where i place the plugs on my decks and i need them to not crack and peel or break after repeated bending, so our individual needs may vary.
```

---
## \#6 Posted by: Cube Posted at: 2016-04-01T16:22:55.771Z Reads: 86

```
Ok. I cut mine with about an inch and a half hanging out of the motor. Not sure where the windings stop inside the wire. But I believe it goes all the way to the stock 4mm bullet. I put silicone wire on for the same reasons you stated. Copying your design. Thanks for the input
```

---
## \#7 Posted by: willpark16 Posted at: 2016-04-14T08:45:07.342Z Reads: 77

```
So what was the original problem, was it the motor or vesc? Im running a similar setup and would like to avoid blowing up my motor
```

---
## \#8 Posted by: Cube Posted at: 2016-04-14T14:46:29.246Z Reads: 70

```
It was the motor phase wires. Moral of the story is don't shorten your wires unless your willing to completely strip the insulation off of the windings. From my experience they are insulated all the way to the stock bullet connector so any shortening of the stiff wires and you will have to strip. On my new motor I attached the silicone wire to the ends of the stiff phase wires and still gets me what I was after. Just wanted flexible wires to loop back and under the trucks through a cut out riser pad.
```

---
## \#9 Posted by: chaka Posted at: 2016-04-14T14:47:01.154Z Reads: 71

```
The OP shortened the motors phase wires without removing the enamel coating resulting in a weak connection. Once he resoldered the connection with the enamel removed it was good to go!
```

---
## \#10 Posted by: willpark16 Posted at: 2016-04-14T17:39:10.448Z Reads: 65

```
haha ohh i thought it was vesc configurations
```

---
