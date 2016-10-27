# Git_Money_Final_Project
##### Akhil Surapaneni
##### Peter Tang
##### Lucas Bizzaro
BIOE 421      

### Brainstorm for project
**Bluetooth helmet**

- Play music
- Take pictures
- Make phonecall
- Display speed, display gas info
- Combine with windshield headsup display

**3D printer**
- Know when it fails, alert
- Correct layer shift and fix it
- Print fell off bed and stop the printer
- Adjust the tension on the filament feeder automatically
- When the printer makes moves, it uses its current position to figure out where the next position is and moves in a relative manner

**Automatic bed leveling**
- Change flow setting automatically to correct for the failure
- If the motor skips steps, it fixes it. 

**Google glass**
- Facial recognition
- Display information 
- From facebook of the person
- Weather
- Have a button take picture, then search up on internet for similar pics/info

**Muscle fatigue tracking suite**
- Using EMG  to track signal
- Display info on phone or something

**Party controller**

- Set party mode
- Set music, lighting   

**Smart bike rack**        
- Swipe the ID card, if the bike info matches and there is opening, lock
- Student can add other student ID on there for access

**Video chatting mirror**
- Would use heads up display technology
- Touch screen?

**Force measuring boxing gloves**
- Put a pressure sensor and an accelerometer into the gloves

**Belt that integrates with Google Maps that vibrates for bikers; maybe can keep track of blindspot**
Actually, scratch that. You have a Pi Board on the top of the bike that has an HUD with salient information about exercise stuff (so it has the salient info of an exercise bike), etc. vibrates on the handlebar with the Google Maps, and automatically flashes the LED in low light situations. Maybe a rearview mirror? Left and right turn signals, you can track location of this pi if it gets lost
- Bike pedaling charges battery pack when not in use
- Combination of lock (track location)
- Rap around on handlebar, when not using, wrap around the wrist
- Vibration wouldnt work, LED may be good
- How are we going to get GPS data? Pure distance? Or how to extract information from google map?

**Make an AI that talks back (akhil this is shitty idea lol)**
- Raspberry Pi Dialysis Machine

**Smart toilet**
- Trackes urine volume
- Determines turbidity viscosity/concentration

** Leave room reminder**
- Ask you bunch of question before leaving room (key? lights?)
- Take a pic for fun
- Could be a key hanger that releases key only after you said what it likes 

**Foot pressure sensing pads**
- Measure different pressure at different location of foot using straing gages
- Get bunch of biometric data including steps, walking style, perhaps can infer mood from the data
- Then can generate messages/serach up news and feed it to you based on that info
- Can look at how long you are sitting give suggestions
- Measure pressure during running so it quantifies how hard you run (incorborate accelerometer feature)
- Can tell how durnk you are by looking at how unsteady your steps are
- Calculate average weight of day, advise on weight control over days

**Smart electronics**
- Remind you to turn it off

We might be going forward with the smart bike idea

Music synchronize with running steps

**Grunt at gym**
- after finishing a rep plays a grunt noise and after a set play a victory sound

### Pi DJ
-How do we interact with the DJ softwares


https://en.wikipedia.org/wiki/Advanced_Linux_Sound_Architecture
https://en.wikipedia.org/wiki/PulseAudio
http://blog.scphillips.com/posts/2013/01/sound-configuration-on-raspberry-pi-with-alsa/
The "sound stack" can be visualized as follows, with programs in the upper layers calling elements in the lower layers:
Applications (e.g. mp3 player, web video)
Sound server (e.g. aRts, ESD, JACK, PulseAudio)
Sound subsystem (described as kernel modules or drivers; e.g. OSS, ALSA)
Operating system kernel (e.g. Linux, Unix)
http://www.mixxx.org/wiki/doku.php/hardware_compatibility
We are basically using the glove to tell mixxx what to do
http://www.mixxx.org/wiki/doku.php/start#controller_mapping_documentation how to tell the mixxx




https://en.wikipedia.org/wiki/SoX


These are some python api’s that edit/stream music live?
http://stackoverflow.com/questions/8501141/python-change-pitch-of-audio-file
http://audiere.sourceforge.net/features.php
http://www.pygame.org/docs/ref/mixer.html


Ideas:
Second, we should do clapping with the capacitative force sensor to make a drumbeat, shaking to make reverb
We should also do like temperature: imagine this: we live demo with a curved metal rod. One end is submerged in a hot liquid, the other end is submerged in a cold liquid. We run the temperature sensor along the metal rod, and we should get a temperature gradient
Like think magic trick style presentation for music
Also, if we can get light colors to sync to the frequency of second song, we can use color sensing to change the frequency of the current song to match the second one. We could make songs harmonize


10/27/16
Goals for today: Download Mixxx on Pi, figure out how to play music on Pi, try to either interface with the software directly, or if you need a DJ controller, figure out how to send MIDI commands from Arduino into Mixxx. 
Optimization: Ask Jordan about feasibility of Spotify integration- PianoBar: Pandora for Linux. Might also be able to edit online radio streams. 


Find simplest possible MIDI controller


Review of MIDI, Pi, and music. Why are we unique. 


Mixxx takes from MP3, Itunes, etc. Can Mixxx take input from mouse (don’t have to write MIDI code and can just control Mixxx)


Branch #2:
Proof of concept: Circuit Playground plays Sandstrom and we can edit tempo using accelerometer.  Individual notes are hardcoded into 8-bit music. 
-Edit 8 bit music. 
Github: MIDI glove


Branch #3: Draw on touchscreen and Processing to either edit 8-bit or output MIDI for Mixxx. 


