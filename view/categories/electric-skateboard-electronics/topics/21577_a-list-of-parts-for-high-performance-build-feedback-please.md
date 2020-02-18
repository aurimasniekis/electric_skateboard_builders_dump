# A list of parts for high performance build feedback please!

### Replies: 2 Views: 635

## \#1 Posted by: filmerskier97 Posted at: 2017-04-23T03:17:42.703Z Reads: 79

```
Hi everybody,

Just sent back my Boosted board dual plus V2. Its a nice board but it doesn't do what I want it to do for the 1700 bucks I spent. The range is terrible. If I am going up a hill I can drain the battery in ten minutes and i want more speed than the 20-22mph it tops out at. I am looking for a board that can do about 30mph with a range of 25 miles. I reached out to the diy electric skateboard guys and they sent me this list of parts for the most high performance build they offer. 

	
Dexter (DIY Electric Skateboard)
Apr 19, 4:24 PM CST

Hi Luke,

Here's the kit that we discussed.

Any questions, let us know.

#1 Highest Performance Kit with Dual Motor Belt Drive Setup (Great for Hill Climbing)    
Dual Mech Kit + 12S4P    Full Electric Conversion Kit (Only need deck)    
Dual Mech Kit    $299.99    diy-electric-skateboard-kits-parts/torqueboards-dual-motor-mechanical-kit/    
6355 190KV * $90ea    $180.00    diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/    
2.4ghz Mini Remote    $60.00    diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/    
VESC * $99.99/ea    $198.00    diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/    
VESC XT90 Parallel    $8.99    diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/    
VESC Canbus    $6.99    diy-electric-skateboard-kits-parts/vesc-canbus-connector/    
VESC Male to Male    $1.99    diy-electric-skateboard-kits-parts/male-male-servo-connector/    
12S4P    $450.00    IN PRODUCTION - ETA 1 month    
$1,205.96    TOTAL VALUE    
$30.00    USA SHIPPING    
$1,235.96    TOTAL PRICE

As far as the deck goes I want something on the shorter end with an kick tail so its easier to point it in different directions. I really like this one so far and the diy guys said it would work with their new battery enclosure https://www.muirskate.com/longboard/decks/71837/jet-2016-vulcan-kick-35-5-longboard-skateboard-deck-w-grip

The purpose of this post is to find out if anyone thinks this is a good idea lol. If anyone has any suggestions of different parts to use or personal experience with the products above a million thanks! Any suggestions or feedback is greatly appreciated!
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-23T03:43:05.549Z Reads: 64

```
Your parts line up looks good.
The Motor KV is a bit high for the Vesc at 12s but you can adjust the erpm limit in the bldc tool to 60k so that you don't fry the DRV chips on your vescs.
The deck looks like a good deal but I would recommend figuring out the dimensions your battery and electronics will need
before settling on a deck. With a belt drive, you might need a longer deck to accommodate a 12s4p and dual vescs.
And I would not recommend mounting the Vescs on top of the battery.
```

---
