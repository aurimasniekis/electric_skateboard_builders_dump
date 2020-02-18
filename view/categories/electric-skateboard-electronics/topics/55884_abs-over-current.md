# ABS over current

### Replies: 12 Views: 433

## \#1 Posted by: moadymoad Posted at: 2018-05-18T13:39:41.254Z Reads: 110

```
I was running my (replaced) dual focbox for 20km without issue when the board stopped accelerating. Checked the vesc and am getting an overcurrent fault.

It is definitely not the settings, check cabling and it all looks fine. It is constantly happening now. If I accelerate on the bench I hear a "click" then it shuts off with the overcurrent fault.

Is this another vesc issue?
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-05-18T13:53:35.119Z Reads: 104

```
It would be best if you add your settings for the community to see.
```

---
## \#3 Posted by: moadymoad Posted at: 2018-05-18T14:06:34.257Z Reads: 98

```
10s3p 30q

each vesc

motor max 60
motor min -40
bat max 22
bat min -6
```

---
## \#4 Posted by: Jinra Posted at: 2018-05-18T14:06:35.955Z Reads: 91

```
can you take a picture of your battery as well
```

---
## \#5 Posted by: moadymoad Posted at: 2018-05-18T14:11:54.822Z Reads: 88

```
Hows the attitude regarding replacement. PSA for anyone looking at purchasing the "platinum" warranty...

Chat started: 2018-05-18 01:51 PM UTC

(01:51:11 PM) Customer Service: Hi Nick Moad, welcome back! What can we help you with?
(01:51:14 PM) Nick Moad: getting over current fault ondual FOCBOX
(01:51:20 PM) *** Eric joined the chat ***
(01:51:47 PM) Eric: Hi Nick
(01:51:50 PM) Eric: Welcome
(01:51:52 PM) Nick Moad: Hi Eric
(01:52:10 PM) Eric: It happens due to incorrect settings
(01:52:38 PM) Eric: try loading the default settings again and configure it according to your setup specs
(01:52:47 PM) Eric: because FOCBOX must be showing the blue light
(01:52:48 PM) Nick Moad: I assure you my settings are correct
(01:53:04 PM) Eric: and I assure you FOCBOX is not faulty
(01:53:22 PM) Nick Moad: there is no need for sarcasm here
(01:53:32 PM) Eric: I am not showing any
(01:53:37 PM) Eric: I am aware of this error already
(01:53:46 PM) Eric: dealt with it many times
(01:54:00 PM) Nick Moad: ok no worries, which setting are you referring to?
(01:54:06 PM) Eric: FOCBOX settings
(01:54:12 PM) Nick Moad: yep which setting?
(01:54:29 PM) Eric: all of the settings you've changed
(01:54:33 PM) Nick Moad: i havent
(01:54:33 PM) Eric: till now
(01:54:35 PM) Nick Moad: its all defaut
(01:54:42 PM) Nick Moad: default*
(01:54:50 PM) Eric: then I think you must configure it according to you setup
(01:55:00 PM) Eric: I am not able to provide you the help with settings
(01:55:25 PM) Eric: because we discontinued DIY support back in AUgust 2017
(01:55:27 PM) Nick Moad: yep so i adjusted bat max to match my battery which is a 3p battery of 30q so max is 45a draw continous. I set each vesc to 22
(01:55:51 PM) Eric: Batt max value must not increase 30A
(01:56:02 PM) Nick Moad: yes 22 is less than 30
(01:56:16 PM) Eric: and what about motor max?
(01:56:20 PM) Nick Moad: 60
(01:56:26 PM) Eric: so the settings are not at default
(01:56:38 PM) Nick Moad: i then set them back to default and have the same issuye
(01:56:50 PM) Eric: check your wiring as well
(01:57:09 PM) Eric: or go to the ESK8 forum for further setup help
(01:57:26 PM) Nick Moad: yeah wiring has been checked. It is all taped and secure
(01:57:38 PM) Eric: If FOCBOX is showing blue light still then it's just a settings issue
(01:58:19 PM) Nick Moad: well it was still showing blue light on the last faulty focboc i had where one of the motor phase cables had come loose and shorted the DRV so not sure thats entirely accurate
(01:58:52 PM) Nick Moad: so you have never seen over current fault due to a faulty controller?
(01:58:52 PM) Eric: The last one must not be recognizable with the PC also
(01:59:00 PM) Eric: Yeah, never seen
(01:59:21 PM) Eric: over current fault only happens if you have wired the FOCBOX wrong or settings are incorrect
(01:59:39 PM) Nick Moad: even though it was working fine for some time before?
(01:59:46 PM) Eric: Yeah
(02:00:20 PM) Eric: If it was working fine and something got shorted, it might possible to cause of this
(02:01:19 PM) Nick Moad: nothing moved around i dont see how anything was shorted. but if that was the case are you suggesting the focbox could be damaged?
(02:01:47 PM) Eric: But if it damages like this, you won't be able to get a replacement or repair with out platinum warranty purchased
(02:01:55 PM) Nick Moad: i have platinum
(02:02:07 PM) Eric: Have you already got a replacement on that warranty?
(02:02:18 PM) Nick Moad: yep
(02:02:26 PM) Eric: if you got one replacement already then you have to purchase it again
(02:02:36 PM) Eric: because it works with only single FOCBOX
(02:02:56 PM) Nick Moad: lol wow ok, I'll have to go to ACCC for a refund
(02:03:07 PM) Nick Moad: this is very dissapointing
(02:03:09 PM) Eric: on replacement you will not able to get the rfund
(02:03:17 PM) Eric: even with the ACCC
(02:03:27 PM) Eric: We have the proof to provide you the replacement already
(02:03:27 PM) Nick Moad: are you aware of the australian consumer guarantee
(02:03:31 PM) Eric: yeah
(02:03:36 PM) Eric: that's why I am saying that
(02:03:49 PM) Eric: because we already provided you a free FOCBOX replacement
(02:04:03 PM) Nick Moad: then you are misinformed and by being misleading you are actually opening yourself up to a fine from ACCC
(02:04:04 PM) Eric: we have the proof of that which we can provide to ACCC
(02:04:20 PM) Eric: We already dealt with this situation before so it will be fine :)
(02:05:05 PM) Nick Moad: aside from your obligations it is really disappointing that is your attitude
(02:05:10 PM) Eric: But I'm still sure that your FOCBOX is not faulty
(02:05:14 PM) Nick Moad: anyway, I'll get things underway
(02:05:37 PM) Eric: Sur
(02:05:38 PM) Eric: Sure
(02:06:20 PM) Eric: you can also email to support@enertionboards.com
(02:06:33 PM) Eric: I think higher management can help you with this
(02:07:39 PM) Eric: Is there anything else I can assist you with?
```

---
## \#6 Posted by: 91stantheman Posted at: 2018-05-18T14:28:03.977Z Reads: 70

```
sorry to burst Eric's bubble but I had a over current fault because of bad wiring on their part. poor soldering joint on one of the phase wires on the terminal had broken and was barely making contact. make sure to check those and also make sure you are using good connectors on the motor side.
```

---
## \#7 Posted by: moadymoad Posted at: 2018-05-18T14:30:18.836Z Reads: 69

```
Well I just had to return one due to a phase wire coming loose and shorting so can’t be ruled out.

I don’t mind if that is the problem but the attitude of the “support” stuff is very very disappointing.

I’ve just jiggled the wires around and it’s not doing it anymore so it could well be a loose connection someewhere in there.
```

---
## \#8 Posted by: 91stantheman Posted at: 2018-05-18T14:36:28.991Z Reads: 71

```
I'm slowly becoming disappointed with this company. they make a great product but they sound like they are afraid to stand behind it. from what I have read online, if you even change out the bullet connectors you void the warranty... 

as far as the wires it sounds like that is your problem, mine did the exact same thing. its to bad you cant cut off the shrink wrap and resolder the joint without voiding your warranty.

btw I'm not sure why they limit you to 30A on the battery side, there are a lot of people running way more on BOTH the motor and battery and never having issues.
```

---
## \#9 Posted by: moadymoad Posted at: 2018-05-18T14:53:08.242Z Reads: 67

```
It seems it might be cabling... I just went for another run without issue.

Not sure if it’s within the vesc or my wiring but will check it all out again later when I pull it apart

Edit: I’m relieved it is repairable but still disappointed in the response
```

---
## \#10 Posted by: 91stantheman Posted at: 2018-05-18T14:55:31.496Z Reads: 69

```
yah take a hard look at the phase wires when you tear it down. I would put money on that being the issue.
```

---
## \#11 Posted by: professor_shartsis Posted at: 2018-05-18T18:12:38.020Z Reads: 62

```
here’s some info from a different thread...

[quote="professor_shartsis, post:14, topic:55724, full:true"]
please verify the absolute current limit setting is set well above the battery and motor current limit settings.
[/quote]
```

---
## \#12 Posted by: onepunchboard Posted at: 2018-05-18T22:29:14.293Z Reads: 50

```
Make sure to place receiver away from phase wire. This cause remote cutouts. And yes abs usually cause by motor wire shorting.
```

---
