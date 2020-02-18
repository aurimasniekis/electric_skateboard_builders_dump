# How to send randomly generated values to BLDC via FOCBOX

### Replies: 34 Views: 941

## \#1 Posted by: KDoc Posted at: 2017-11-06T21:27:08.110Z Reads: 139

```
Hi,
HELP! 
I want to use BLDC Tool for Mac to send randomly generated rpm (range = 500 to 6000) and duration (range = 30s to 72,000s) values to precisely control a BLDC motor (KEDA 63-64) via my FOCBOX. Any help, alternative directions or suggestions (except for the obviously obscene ones) would be greatly appreciated. Yes....I am a NOOB.
Thanks, KDoc.
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-11-06T22:23:54.984Z Reads: 130

```
need better explanation. What do u mean random value?
```

---
## \#3 Posted by: KDoc Posted at: 2017-11-06T23:22:44.159Z Reads: 120

```
I am using a random number generator to generate a list of motor speeds and durations, for example; 578 rpm for 372 s, 4076 rpm for 5471 s, 2097 rpm for 3201 s, etc., etc. I want the motor to soft shift to these speeds and hold them for the specified duration and then move on to the next set, and so on.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-11-07T00:07:41.791Z Reads: 112

```
Maybe you could take a look at Vedder website for the 4.12 Vesc, which is the same on a firmware level as the focbox http://vedder.se/
```

---
## \#5 Posted by: KDoc Posted at: 2017-11-07T01:39:48.443Z Reads: 100

```
Hi Johnny
I initially got started at Vedder’s site. This is how I ended up with a FOCBOX. I have come at this from the ebike site endless-sphere.com and setting up the parameters for this motor and the FOCBOX is doable through Kepler’s tutorial. What I am hoping to find is a way to interface my MacBook and the FOCBOX via BLC Tools for Mac to precisely control the motor. I could very easily be missing my solution from Vedder’s site, but it seems to me that Vedder's programming tutorial is for downloading the programming tool, setting the motor parameters and then setting up the remote control connection. Please correct me if I am wrong, but I was assuming that the programming tool I need is BLDC for Mac (which I have already) and I was hoping for some help with my specific control parameters. If I am missing the point here, please let me know. At this moment the only point I have a firm grasp of is the one on the top of my head. 
PS 
The reason I am on esk8 is that I have found the posters on this site to be very knowledgable, cutting edge and generous and you seem to really limit the abuse that plagues other sites.
```

---
## \#6 Posted by: Blasto Posted at: 2017-11-07T02:32:09.491Z Reads: 84

```
I don’t know how handy you are with software, but i know i’m fucking useless so this would be my solution:

Use an arduino to generate a ppm signal, put the focbox in duty cycle mode and bench mark the erpm with each given signal. Create a psydo random sognal with the arduino and monitor the results via the real time data
```

---
## \#7 Posted by: saul Posted at: 2017-11-07T04:42:00.362Z Reads: 68

```
this is either a very advanced or completely useless application. i can't tell which...

<img src="/uploads/db1493/original/3X/7/e/7eb80684e2b1223b648673c5e7cd17c03b07ba2d.jpg" width="510" height="385">

either way its a custom application, you will need programming skills. and you will likely burn out more than one esc trying...

Whats the point? what do you actually want to accomplish?
```

---
## \#8 Posted by: KDoc Posted at: 2017-11-07T07:52:03.477Z Reads: 59

```
Hi Blasto,
Thanks for thinking about this. I like a good portion of this solution. I was hoping to avoid the Arduino, but I may have to, as you suggest, “generate a ppm signal, put the focbox in duty cycle mode and bench mark the erpm with each given signal”. I previously decided that while an  Arduino could generate a pseudo-random number, generating random numbers from a Gaussian distribution, where the randomness comes from atmospheric noise is more robust. I have the process to continuously generate the random values I need. I now just need a way to get my computer to tell my motor to spin at these values...damm it. So I am still unclear about how to get the random data into the ppm signal. Any thoughts?
```

---
## \#9 Posted by: KDoc Posted at: 2017-11-07T07:53:18.799Z Reads: 56

```
Hi Saul, 
I suspected this question(s) was coming. I hope this application lies somewhere in the middle of the spectrum between “very advanced or completely useless”. I am trying to get my motor to drive a fixed gear bicycle wheel (in a trainer) at the random values mentioned at the beginning of this post. I am trying to get leg muscles to force neurons to accept overriding and completely random inputs. It is for the treatment of a neuromuscular disorder and so far the esk8 community is the only one I can find that I believe might have the intellectual flexibility, design and construction skills, coupled to an inherent ability to test the crazy stuff you actually build, to be able to give me some guidance. So I suspect, like you, that this might pendulum between “very advanced or completely useless”, but the theory behind the treatment is valid.
```

---
## \#10 Posted by: Maxid Posted at: 2017-11-07T07:56:15.964Z Reads: 56

```
Why not pipe the random numbers through the Arduino? You can just send them as Strings, especially since you are only sending new commands quite far apart
```

---
## \#11 Posted by: KDoc Posted at: 2017-11-07T08:04:36.364Z Reads: 54

```
Hi Maxid,
This might be the solution. My Arduino skills are non-existent, but I will get on this. Anyone with any specific suggestions for deigning/building the Arduino, or any other thoughts/possibilities please let me know. Like I said...I am a NooB.
```

---
## \#12 Posted by: Der6FingerJo Posted at: 2017-11-07T08:12:40.536Z Reads: 52

```
There is a Arduino Library called VescUartControl by RollingGecko, it's currently working for fw 2.18 and he's looking for testers for newer firmware. Also, you can directly set the RPM Values via UART using this library (with the newer firmware anyways). Then you could send the random values to the arduino via Processing (i haven't used it so far but i think that's what to use).
```

---
## \#13 Posted by: saul Posted at: 2017-11-07T08:43:58.814Z Reads: 52

```
[quote="KDoc, post:9, topic:37555"]
I am trying to get leg muscles to force neurons to accept overriding and completely random inputs. It is for the treatment of a neuromuscular disorder
[/quote]

This actually sounds very interesting. an surely a pretty advance biomed Engineering application. (Read: FUN!)
I have a good amount of programming and arduino skills. and fixie thats not in use.

Can you give me some reference to why you want to use "random" input?

also the vesc/focbox has a pretty powerful processor with some unused resources, so it can likely be done directly with a custom application + vesctool. still needs programming but no extra hardware.
```

---
## \#14 Posted by: Maxid Posted at: 2017-11-07T09:05:38.236Z Reads: 48

```
Keep in mind that all you need from the Arduino to drive the VESC is a PWM signal (PPM is what the remote uses but that is "translated" by the receiver to a PWM signal) - see also 
https://hackaday.io/project/12123-electric-longboard/log/42519-vesc-finally-arrived for example.

So doing this should be really easy (far less time consuming than fiddling with custom VESC firmware).

Just look for PWM tutorials for Arduinos and how to send and convert some text over USB. You should have this up and running in an hour.

For the more professional version without an Arduino: There must be a way to connect to the VESC the same way as VESC-Tool does it and then just send the raw UART commands. 
But I can't find a tutorial and since the Arduino solution is so easy, cheap and quick I am not sure if it would be really any better.
```

---
## \#15 Posted by: chuttney1 Posted at: 2017-11-07T09:59:20.257Z Reads: 45

```
 From what I just read and understood, I'm guessing your goal is to prove a concept through a randomly generated over time Gaussian distribution and using the result to drive a motor.  From what I read and understood about the muscle part, you want to force stimulation of muscle in the opposite direction by making the muscle send the action potential into the neuron. That's cool.

**This is a bunch of spiel/thoughts running. Ignore if you don't want to read it. I'm just trying to help** 
I know the Gaussian distribution delivers positive and negative values with an average being the greatest towards the middle. Trying to brute force the numbers into something...., I would try to set the X and Y axis values in a range but what would I label the X and Y axis? I know a motor gives off angular velocity and torque and you want to control its RPM for a set amount of time through the PPM function. The limiting factor is the RPM of the motor.
```

---
## \#16 Posted by: KDoc Posted at: 2017-11-07T18:43:04.253Z Reads: 43

```
Hi Jo,
Thanks for the resourse. I took a look at the Arduino Library. I need some time to explore it. Any help in setting up the Arduino is greatly appreciated, although I now have the benefit of the next few responses so I am trying to refine my request as your collective assistance accrues. A big thanks to everyone that is thinking about this. I am trying to trace how my values will travel from my computer to the motor and what the difference (if any) there is between UART and USB for this application. I feel the thin ice of apples and oranges may be melting under my feet. I appreciate everyones patience.
```

---
## \#17 Posted by: KDoc Posted at: 2017-11-07T18:45:48.051Z Reads: 44

```
Hi Saul,
Thanks for the positive response and relevant, clarifying questions, especially with your previous Futurama reference as I really feel the oscillation between Philip J. Fry (with my limited electronic and programming skills) and Farnsworth (I am comfortable with my neuromuscular interface design with a solid neuroscience background). So on with your question; I am using true random speed and duration values because the brain has a remarkable knack for detecting and accommodating patterns, resulting in iterative behavior. By iterative behavior I mean the capacity to repeat a task over and over to the point where the task response becomes embedded. This works well when the brain and body are well synchronized, but not so much when either has gone awry. One tends to lead the other in a very undesirable direction. So before the muscles atrophy into a non-desirable pattern it is possible to push large muscles to force the neurons to try to accommodate a reversed (hence new) neural signal (“you don’t tell me what to do...I tell you what to do”). It is then possible to allow the neurons to reestablish control, albeit with a new neural output, and then repeat the disruption as needed.
The use of a random signal is to ensure the brain cannot settle back into a physically destructive pattern, and let me be emphatic, the brain is a pretty tricky customer and it can smell a non-randomized rat a mile away. Therefore, a computer generated random number is not adequate because the number is not truly random and the brain has a way of detecting this and developing a work around. It took me a while to find and generate a true random number generator, but I feel comfortable with this part of the (non) equation. I have generated a number of sets for this project. I just need to get the damn values from my computer to my motor.

I got stopped at the computer/Focbox/motor junction, but believed, as you do, that programming the Focbox would be enough, and that no new hardware would be required. It seems that if I do need hardware that an Arduino might solve my problem, but I was/am hoping for a Focbox programming solution or some other simple way to drive the motor with my random values. 

I am also dogged by the future in this. For now I will gladly accept a wired solution with a computer operator (me) pushing the values, but eventually this will require a bluetooth, wifi solution when I cannot physically be with the patient (a close friend) that I am creating this for. So I need to get the mechanics of this working, but I will eventually have to push each ensuing treatment/workout over wifi (Arduino?), but that is for later. 

PS
Returning to the Fry-Farnsworth analogy the last programming I did was in FORTRAN. 
P
Also, see my response to chutney below for fixie information.
```

---
## \#18 Posted by: KDoc Posted at: 2017-11-07T18:47:13.254Z Reads: 39

```
Hi Maxid,
Hopefully you have read the last few responses because I have tried to address a few of your insights. Both of your suggestions regarding; “PWM tutorials for Arduinos and how to send and convert some text over USB” and especially “There must be a way to connect to the VESC the same way as VESC-Tool does it and then just send the raw UART commands.” are worth investigation. I will try to get on this. Please keep any thoughts and resources coming.
```

---
## \#19 Posted by: KDoc Posted at: 2017-11-07T18:48:33.592Z Reads: 38

```
Hi chuttney,
I am glad I was able to “curry” a response (sorry) and any help is welcome. I set the parameters for time by determining the “normal” work out length my friend could maintain when he was riding unimpeded (healthy), including warmup, workout and warm down. I then generated random duration for each of these periods. I then determined the minimum and maximum cadence he might be comfortable with in these three workout intervals while also increasing the maximum cadence to include super high values achieved in spin workouts with very fit elite athletes (cadence as high as 300 rpm for a few seconds. This seems incredible to me, but we will see, plus this max value can easily be changed). I then generated random cadence values within these parameters. The idea is to disrupt not just the present disfunction, but also previous “healthy” cadence patterns. The BLDC motor I have has a non-load speed of about 6000 rpm. When coupled to a 27” wheel with a fixed gear I get crank cadence within the range I am looking for (at least to begin with). I internally seized an old Shimano Dura-Ace free-hub body and using the myriad of gear size cogs available from my old stash and a few local bike store trash bins I am able to get pretty good cadence selection with a direct drive chain set up.
```

---
## \#20 Posted by: KDoc Posted at: 2017-11-07T18:49:27.967Z Reads: 35

```
I realize this thread is getting a little away from an esk8 topic and I do not want to hijack or disrupt this site. I will move it (uncertain where to) or entertain thoughts from esk8 users on where to put this if it becomes a nuisance. I really appreciate the insight, information and suggestions that have come from this community and as I said in the beginning this community is really unique and is responding in exactly the way I hoped for. Thank you.
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-11-07T19:05:13.770Z Reads: 32

```
definitely not a nuisance!  this is a very interesting topic AND it’s for the greater good. no need to go anywhere :)
```

---
## \#22 Posted by: KDoc Posted at: 2017-11-07T19:20:30.694Z Reads: 27

```
Thanks GrecoMan!
```

---
## \#23 Posted by: KDoc Posted at: 2017-11-07T19:43:49.387Z Reads: 26

```
Just to make sure the image everyone is getting of the set up is correct I am using the motor as a friction drive for the 27” inch wheel.
```

---
## \#24 Posted by: Der6FingerJo Posted at: 2017-11-07T20:54:45.142Z Reads: 28

```
[quote="KDoc, post:17, topic:37555"]
Thanks for the positive response and relevant, clarifying questions, especially with your previous Futurama reference as I really feel the oscillation between Philip J. Fry (with my limited electronic and programming skills) and Farnsworth (I am comfortable with my neuromuscular interface design with a solid neuroscience background).
[/quote]

I love how you can meet so many people with different skills in this community, neuroscience completely black magic for me :D

Just a small summary for the Arduino way of doing this. You would need to send the random values via serial communication to the arduino, which in turn requires the app Processing as a middle man between your numbers and the arduino. Then the arduino would either send a PWM Signal to the VESC in Duty Cycle Mode or send the actual RPM Value via serial communication to the VESC. (latter would probably give more resolution). This would require an Arduino Mega for best serial performance.

This of course is the quick and dirty, and probably less reliable, way to do this. But it's easy because there is no additional hardware and software required and it doesn't require programming on any VESC related things, so it might be good for a proof of concept. 

Another idea would be to use a USB to UART adaptor (or FTDI Stick), so you could directly send serial data to the VESC from you computers USB Port. But i am not sure how to get a sort of VESC Library for this method.
```

---
## \#25 Posted by: Maxid Posted at: 2017-11-08T10:24:25.334Z Reads: 26

```
For some Arduino sample this might work but I have not tested it and it is only a theory. No guarantee that it works - use it at your own risk.


	// VESC PWM Signal connected to this pin (can be another PIN - make sure to adjust this for the Arduino you are using) - don't forget to connect GND as well

	int VescPin = 9; 



	void setup() {

	  // put your setup code here, to run once:

	  Serial.begin(9600);

	  // sets the pin as output

	  pinMode(VescPin, OUTPUT);   

	}



	void loop() 

	{

	  // Read serial input:

	  while (Serial.available() > 0) {

		int inChar = Serial.read();

		if (isDigit(inChar)) {

		  // convert the incoming byte to a char and add it to the string

		  inString += (char)inChar;

		}

		

		// if you get a newline send command to VESC as PWM then print the string's value

		if (inChar == '\n') {

		  

		  long value = inString.toInt();

		// Send to VESC via PWM

		analogWrite(VescPin, value);  //analogWrite values from 0 (0% duty cycle) to 255 (100% duty cycle)

		// the signal will be sent until you give a new command - so make sure that your main application handles that




		  // Any non integer value will be intercepted here

		  if(value == 0)

		  {

			// send identification lines to PC when asked non-integer string

			// can be used for automatic identification of correct COM-port in Windows app

			Serial.println("VESC Control Arduino");

			// multiline allows detailed description    

			Serial.println("This Arduino accepts integer values and sends a PWM signal to the VESC");   

		  }

		  else

		  {

			// feedback of what the Arduino has been sent

			Serial.print("Value: ");

			Serial.println(value);

		  }

			  

		  // clear the string for new input:

		  inString = "";

		}

	  }

	}
```

---
## \#26 Posted by: KDoc Posted at: 2017-11-09T18:49:24.100Z Reads: 21

```
Hi Der...Jo,
Great stuff. These suggestions fill in a lot of the blanks for me. I am trying to get up to speed with the Arduino. I plan to use both your and Maxid’s solutions. Your quick and dirty suggestion makes sense to me and your second idea has me chasing off in a future direction. I need to stay semi focused on the short-term goal of getting the data from my computer to the motor, but please keep any/all suggestions coming. I really do appreciate this.
```

---
## \#27 Posted by: KDoc Posted at: 2017-11-09T18:50:39.989Z Reads: 21

```
Hi Maxid,
Again, great stuff. I really appreciate the effort on your part. This has me digging into Arduino. I have not used an Arduino so I have spent the last day getting familiar with some of the hardware and software. It is a little unfortunate that a “use it an your own risk” is required. It seems crazy that you putting in your time, effort and experience might invite backlash from someone that demands that any outside assistance must be perfect right out of the gate or else. I just continue to be appreciative of everyones effort with great questions, suggestions and solutions. Please keep it coming.
```

---
## \#28 Posted by: Maxid Posted at: 2017-11-09T18:57:24.877Z Reads: 19

```
I simply am not responsible if you break your VESC - as you may know this is new territory for all of us and a prototyp setup. I have personally also not hooked up an Arduino to a VESC so obviously can not guarantee that it will work as intended. Try it and report back!
```

---
## \#29 Posted by: KDoc Posted at: 2017-11-09T19:15:40.035Z Reads: 21

```
Will do.
PS
Staring at my Focbox I feel like I am treating it a little like an “old folk” when they first get their hands on a TV remote and they are reluctant to use it because they think it is kinda like a Star Trek Phaser and they might end up blasting a hole thru their living room wall. If I end up destroying my VESC I can just get another one. I guess when someone says “let’s spark one up” this isn’t what their talking about.
P.
```

---
## \#30 Posted by: Der6FingerJo Posted at: 2017-11-09T19:22:13.898Z Reads: 19

```
Hey there, i'm not totally sure about this but i don't think simply using analogWrite would be enough to get a readable PWM Signal for the VESC. Instead you could use the Servo library which is included in the Arduino IDE i believe. That would also give you 1024 steps of resolution and worked fine for my VESCs so far.
Still, i think using the Vesc Uart Control Library would be the best way to go, it isn't that much harder to implement and would give you direct control about the numeric rpm value with much more resolution.
```

---
## \#31 Posted by: Maxid Posted at: 2017-11-09T20:27:46.253Z Reads: 17

```
No idea - I just looked up how to do PWM and this is what came up. 

Do we even need the UART library? All we need is a single command right?
```

---
## \#32 Posted by: Der6FingerJo Posted at: 2017-11-09T20:57:46.270Z Reads: 19

```
I don't really know much about serial communication, but as far as i can tell the VESC only accepts it's own protocol, which is more complicated than a single command. That's why we need to send the whole package everytime we change one parameter, and that is handled by the library.
```

---
## \#33 Posted by: Blasto Posted at: 2017-11-09T21:36:18.858Z Reads: 21

```
servo.h all of that is implemented. This is what i used, it works. 

     #include <Servo.h>

    Servo myservo;  // create servo object to control a servo

    const int ppmMAX = 2000; //max microseconds
    const int ppmMIN = 1500;
    const int ppmIDLE = 1000;//min 

    void setup() {
        Serial.begin(9600);
      myservo.attach(3);  // attaches the servo on pin 3 to the servo object
    }


    void loop() {
     //fancy code here
     myservo.writeMicroseconds(ppmIDLE); //set ppm to idle
    //fancy code
    //fancy code
    }
```

---
## \#34 Posted by: KDoc Posted at: 2017-11-10T00:54:31.122Z Reads: 19

```
It is great that people are thinking through my programming requirements so I thought I should offer up some estimates for what the data might look like.

For my 190 KV 10S 2000W outrunner spinning a 630mm wheel (with 23mm tire), spinning a 25t x 42t crank, I estimate 3.379629 rpm/v. With 4S to 10S I get a crank cadence range from 49 - 122 rpm. This is a no load value and might have to be re-calibrated once the system is under load, but it may not matter as long as everything stays relative. 

Below is the middle segment of a warm up/work out/warm down patient set.

Randomized Work Out

Time  -  Forced Cadence
69s @ 76rpm
28s @ 103rpm	
1s  @ 52rpm
16s @ 75rpm
90s @ 112rpm
30s @ 118rpm
36s @ 60rpm
70s @ 103rpm
14s @ 115rpm
22s @ 84rpm
68s @ 109rpm
43s @ 106rpm
85s @ 56rpm
3s  @ 88rpm
78s @ 108rpm
54s @ 113rpm
73s @ 84rpm
47s @ 79rpm
76s @ 120rpm
3s  @ 114rpm

Using 3.379629 rpm/v I get the following duration/voltage data for my motor.

69s @ 22.49v
28s @ 30.48v	
1s   @ 15.39v
16s @ 22.19v
90s @ 33.13v
30s @ 34.92v
36s @ 17.75v
70s @ 30.48v
14s @ 34.01v
22s @ 24.85v
68s @ 32.25v
43s @ 31.36v
85s @ 16.60v
3s  @ 26.04v
78s @ 31.96v
54s @ 33.43v
73s @ 24.85v
47s @ 23.38v
76s @ 35.51v
3s  @ 33.73v

If I can hold these type of values with consistent soft transitions I should be good assuming that my presumptions are correct.
```

---
