# Raptor 2.1 brakes while accelerating, advice/suggestions appreciated!

### Replies: 13 Views: 495

## \#1 Posted by: mrjonnyjones Posted at: 2019-04-19T10:23:07.143Z Reads: 105

```
Hi guys, hope you're all well! I thought I would post this on the Builders forum as the Club forum is a little quiet in general.

I've had my Raptor 2.1 since March 1st and it's awesome, the torque is addictive!

BUT, in that time it has applied the brakes at pretty much 100% three times - randomly. The three times it happened I was accelerating from a slow roll - I usually start with a kick-push. The remote is in R-Spec mode all the time, the board has always had the latest firmware on the UNITY as well. Motors and all other components are in good working order as far as I know (motor detection and parameters are always as they should be), the only 'thing' I know of is that the motor phase wires are a bit bent coming off the secondary PCB before they reach the trucks, see photo:

![RAPTOR_INTERNALS_002|666x500](upload://qVFebnNtvKhvK0Vdh8HhD4xUdRP.jpeg) 

I've always checked the motor temperatures after the braking incidents and they are warm but comfortable to touch, so no over-heating.

If any of you have some theories as to why the board slams the brakes on that would be great to read, as I have a reduced confidence in accelerating on the board at the moment - I don't know if I'm going to be thrown forward off the board!

I have contacted Enertion Support a few times, but I don't think they know what's going on either.

Thanks in advance,
Jonny.
```

---
## \#2 Posted by: McErono Posted at: 2019-04-19T11:20:26.944Z Reads: 94

```
Are you sure it brakes? Cutouts feel like braking too.

I had cutouts because I calibrated (in focbox ui) the remote in slow mode instead of r-spec mode.
```

---
## \#3 Posted by: taz Posted at: 2019-04-19T11:43:13.027Z Reads: 95

```
Is that with the nano-x remote? If yes do you calibrate the remote every time you turn it on?
```

---
## \#4 Posted by: mrjonnyjones Posted at: 2019-04-19T11:45:28.625Z Reads: 93

```
I'm not sure to be honest, I just assumed it was braking? UNITY was calibrated with the remote in R-Spec mode.
```

---
## \#5 Posted by: mrjonnyjones Posted at: 2019-04-19T11:45:58.199Z Reads: 90

```
Yes, that's with the Nano-X and it gets calibrated every time before the board is turned on.
```

---
## \#6 Posted by: CarlCollins Posted at: 2019-04-20T03:48:31.655Z Reads: 74

```
Hey There 

Can you please confirm the following?
1: Remote was fully charged?
2: What is the current firmware version on your Unity?
3: Have you adjusted any values or you are using stock ones?
4: Have you checked if receiver servo connector is loose?
```

---
## \#7 Posted by: mrjonnyjones Posted at: 2019-04-20T08:11:22.035Z Reads: 62

```
Hi Carl,

1) Remote is always fully charged
2) Firmware version is 23.43 (updated the other day)
3) No values adjusted
4) All wires are connected in the enclosure

I hope this helps? :slight_smile:
```

---
## \#8 Posted by: mrjonnyjones Posted at: 2019-04-20T20:24:34.118Z Reads: 56

```
Hi again Carl,

I've ridden my Raptor 2.1 all afternoon at an event here in the UK, reaching 27.5mph with ease - felt amazing!

No cut-outs or braking. I wonder, the three previous times the board stopped while accelerating... was it a current draw cut-off? I say this because the board wasn't going very fast when I requested a lot of throttle... could it be possible that it was the UNITY cutting power due to too many amps being drawn?

Today, I rolled up to 10-12mph and then accelerated. No issues at all.

Would you say this is acceptable? Or do you consider the board to not be 100% considering it doesn't like to throttle up from a low speed... sometimes?

Other than that, the Raptor absolutely FLEW up some steep hills on the track I was on, never experienced ease of riding like it, awesome!
```

---
## \#9 Posted by: CarlCollins Posted at: 2019-04-21T10:57:12.864Z Reads: 51

```
I would like to inspect your board remotely or virtually if possible, let me know when you are available?
```

---
## \#10 Posted by: mrjonnyjones Posted at: 2019-04-21T11:23:21.947Z Reads: 50

```
OK great, I'll DM you :+1:
```

---
## \#11 Posted by: mrjonnyjones Posted at: 2019-04-30T07:59:45.750Z Reads: 43

```
Just as a follow-up, @CarlCollins has been *very* helpful with this issue. We completed a virtual desktop support session via TeamViewer and essentially re-flashed the most recent firmware onto the Unity. Motors and Nano-X were re-calibrated. So far I've not had any braking or cut-offs happen... although I am still testing.

Enertion have made a PSA on the [Enertion Boards International Riders Group](https://www.facebook.com/groups/1890905301163087/) on Facebook about this issue now, as there have been a few similar reports. Thanks to Carl and everybody involved at Enertion for acknowledging the issue and recommending a fix. :+1:
```

---
## \#12 Posted by: brenternet Posted at: 2019-04-30T12:37:28.688Z Reads: 36

```
Cheers for the follow up. Carl is a credit to enertion ❤
```

---
## \#13 Posted by: CarlCollins Posted at: 2019-04-30T15:14:57.739Z Reads: 29

```
Glad I am able to help :slight_smile:
```

---
