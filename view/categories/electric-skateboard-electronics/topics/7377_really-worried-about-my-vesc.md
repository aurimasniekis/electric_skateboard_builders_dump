# Really worried about my VESC

### Replies: 4 Views: 691

## \#1 Posted by: robskie Posted at: 2016-08-09T18:48:12.210Z Reads: 70

```
Hi everyone, I hope you are all doing well.

I've finally comitted to building my board, parts are slowly starting to arrive. I've been browsing these forums pretty frequently to learn as much as possible before I start the assembly.
Now, while browsing i've been seeing a lot of issues pop up regarding the Enertion VESC, which is the same one I bought.
Since I don't want to break/blow up my ESC on the day I start my assembly I'd really like to get some pointers as to what I should be looking out for when I receive it, the safest way to handle it,..
I've googled quite a bit and haven't really found any specific guidelines.

Thanks!
```

---
## \#2 Posted by: sl33py Posted at: 2016-08-09T18:57:32.802Z Reads: 68

```
follow the steps from Vedder to setup and make sure you do the discovery for your motor.

as for things to be cautious with - i connect to a low amperage battery or lab power supply to initially connect and configure it the first time.

I would also not go 12s right out of the gate.  I typically shoot for 8-10s even with 200/190kv motors.  There was a great thread on ERPM limits of 60k and less to avoid damaging the DRV chip.  Check that out (i'll search and link in a sec) too.

VESC is great - with some basic common sense setting it up correctly is not too difficult ( i was able to do it... ;) ).

HTH - GL!
```

---
## \#3 Posted by: Jinra Posted at: 2016-08-09T18:58:04.401Z Reads: 63

```
First thing is to insulate the hall sensor pins so they don't short the main power lead.

See here: http://www.electric-skateboard.builders/t/vesc-faq-negative-squared-cross-mark-warning-negative-squared-cross-mark-risk-of-short/6805

Second is go over the board visually and make sure there are no shorts, especially with the positive and negative power leads on the PCB. Then, try it out! Maybe start with a lower voltage power source first.
```

---
## \#4 Posted by: mcfly777 Posted at: 2016-08-09T19:10:37.211Z Reads: 50

```
I don't rev it up without any load (i.e. on the bench). Not sure it helps but can't hurt.

Leo
```

---
