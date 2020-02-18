# Modifying 6S board to 8S possible?

### Replies: 2 Views: 500

## \#1 Posted by: leven Posted at: 2016-08-23T08:40:35.850Z Reads: 71

```
Hi, new user and new skateboarder, lots of good info on the forum and learning a lot, riding it is fun but i just cant help myself from do a bit of modifying, building things is also lot of fun. :)
Basically i bought a cheap Chinese dual motor board (benchwheel), and plan to re-use the electronics and motors/trucks and build a new board, using plywood covered with carbon-fiber i have lying around as the deck, and a carbon-fiber box to house the battery and electronics to waterproof it a bit (rains a lot in Sweden).
I was hoping to get some experienced e-skateboardpeople to voice their opinions if its a stupid idea.

The board currently uses a 6S4P 8.8Ah pack and according to the information Samsung 25R-cells (but we know it isnt).
Ideally i would like a litte bit more speed.. So i was thinking about going from 6S4P to 8S3P (and hoping the electronics can take a 7V increase without blowing up), the motors are a version of N5065 270kv and is 8S rated.
Can i use a parallel balance lead-connector to connect an 8S to a 6S balance connector?
The board only have 6S connector.

I like the remote with battery indicator and the breaking etc, so i want to keep this, but if i toast it i'll go with 2xVesc instead. 

I'm planning to build a new pack using LG HG2 3000mah 20A, the board has an 80A car-fuse so a 3P would get me to 60A, i would like 8S4P but then the battery A is right on the limit, do you think will it blow the fuse or will it just manage the current drain better since there is more cells to share the load?

Higher voltage gives me more speed, but will higher Amperage give me more power to go uphill or is that more dependent on the electronics?

Anyway, total newbie on building with RC-parts but have a background in some electronics and computers. I would really appreciate your advice on this.
```

---
## \#2 Posted by: mattdig Posted at: 2016-08-23T14:48:04.443Z Reads: 42

```
You probably wont get more power by just moving batteries around. You'll be able to pull more Volts but fewer Amps out of the pack, and you end up with basically the same Watts. And you really don't want to over-exert the knockoff batteries in that pack.

You cannot just go from a 6s balance connector to an 8s, you need to solder the 8s connector wires onto each parallel set.

The battery indicator probably wont work because it's expecting a 6s system.

And the ESCs are probably only rated for 6s so you need to replace those first.

Final thoughts: Ride the board as is until you can build a new battery pack and buy the VESCs.
```

---
