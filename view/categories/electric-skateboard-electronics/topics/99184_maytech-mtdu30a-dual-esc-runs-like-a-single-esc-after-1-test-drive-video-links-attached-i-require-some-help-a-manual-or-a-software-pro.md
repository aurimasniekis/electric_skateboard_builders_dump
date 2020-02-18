# Maytech MTDU30A Dual ESC (Runs like a single ESC after 1 test drive) Video links attached. I require some help, A manual or a software pro

### Replies: 4 Views: 119

## \#1 Posted by: Noodless Posted at: 2019-07-26T21:25:26.031Z Reads: 29

```
The setup is made of two 90 inch Maytech Hub motors.

A dual ESC MTDU30A.

A 10sp5 Lipo battery pack with built in BMS.

A maytech mini remote. MTSKR 1712

It is a bought Plug and play set.
After 1 test drive 1 of my motors stopped running. (Still brakes)
And the ESC Led's gave different signals.
Since both my hub motors still function after testing them individually on the still functioning part of the Dual ESC. And all the cables have been switched around to find faulty wiring. I find myself convinced of a software related problem. I will attach 2 links to OneDrive. It seems like the Master/Slave connection is lost and the slave functions as the master while the master is unable to connect.
There are videos of how the ESC reacts after start up and with connecting the remote. I tried reconnecting the remote as well. No luck with that either.  But i would like to put the focus on the Red LED's that upon startup blink untill connection with the remote is made. And after that how the functioning part of the Dual ESC gives a red Light. And the malfunctioning part of the ESC, it's Led just acts weird. I have sent the videos to Maytech there customer service is responding. But its frustrating after 1 test drive how it malfunctions and i dont think i can apply for a refund. :/ 

Thx in advance. 

p.s. Im aware of the 2 MTDU30A topics. I replied to them But the community flagged me for spam. And both my Replies with this question got hidden by a bot. So i decided to start over.

Video-Links: 

[https://1drv.ms/u/s!AhvE8vPuJ2GNdKJ2mWLEUEWyuq4](https://1drv.ms/u/s!AhvE8vPuJ2GNdKJ2mWLEUEWyuq4?spm=a2g0s.imconversation.0.0.68713e5fiPKYFD)

[https://1drv.ms/u/s!AhvE8vPuJ2GNdiS_eDQi9KAobOY](https://1drv.ms/u/s!AhvE8vPuJ2GNdiS_eDQi9KAobOY?spm=a2g0s.imconversation.0.0.68713e5fiPKYFD)

Any reply to confirm my findings on the software issue or decent answer or idea is highly appreciated cause im losing my mind here wondering if i broke it myself or if its a production issue. And how i can fix it without having to buy a new ESC after 1 test drive.
```

---
## \#2 Posted by: Noodless Posted at: 2019-07-26T21:51:00.877Z Reads: 26

```
I read the community guidelines. Is this topic unallowed since it is a personal matter??
```

---
## \#3 Posted by: wafflejock Posted at: 2019-07-26T22:19:59.028Z Reads: 25

```
Issues are fine not sure what the nature of the post was that was flagged but so long as it isn't just vendor bashing and you are looking for a solution to a problem it should be fine.  Perhaps like you said overly aggressive bot saw links and flagged, can also join the new "esk8 dot news" forum (many experienced members from here have moved over to avoid the conflict of interest with this site, and other issues), but honestly not sure many people have experience with this ESC as a majority of us run some variation of the VESC.  

Can say without the original software or diagnostic tools this is going to be hard to troubleshoot if it isn't a known issue to someone.  

One advantage of the VESC is the very good desktop app which can give you a ton of information about the input and output from the ESC (amperage from battery and for each phase, voltage, PPM/PWM/Analog input with real-time display, etc etc.).  Plus uses the stm32 chip that can be directly connected to with a ST Link cable and normally can connect with USB as long as the bootloader exists on the chip.

If it only worked once and blew through no fault of your own I would demand a refund or replacement from the seller, if they offer no compensation I would never buy from them again (waste of your time and money).
```

---
## \#4 Posted by: Noodless Posted at: 2019-07-27T06:57:34.219Z Reads: 13

```
Now this is an answer i can work with. Thank you very much. I will have to invest in the Swedish Vedder ESC's if i cannot fix the problem or get a replacement then. And i was indeed hoping someone had encoutnered this issue as well. As for the config tool and or manual. Im starting to doubt anyone but the seller has it. Thanks for your reply.
```

---
