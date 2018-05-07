Jeff Beeby

Guy Verrier

ETR 164


# Final Project: Wrist mounted raspberry pi

As I stated in my propsal, my hope is to take the knowledge that I accuried during my IRC Server project to then make a wrist (well arm) mounted computer. I Know we already have smart watches and cell phones but I think with some tweaking and some nice bit of cutting technology this simple, silly project could have some real world applications that make it a more viable choice then lugging around a have rugged laptop. Any where from technicians have them to setup/ repair/debug networks so military applications for soldiers getting information or controlling small drones for recon. I can also see where this can be used for potential onsite hacking/cracking. Obviously the potential of this idea can be used for both good and bad but like all tools, it is all about the users intent that determins the use.

I was first introduced to this idea while watching a TV show called "Chuck" where character used it to bypass security alarms and navigate though buildings.

![Chuck arm computer](https://github.com/jbeeby/Final/blob/master/chuck.png)

From there I started playing a game called Fallout 4 on Xbox where this idea was reinforced. This was a little bit more relistic in ability but if I could merge the two together I think something interesting could be made.

![Pip Boy 3000](https://github.com/jbeeby/Final/blob/master/Pip-Boy_3000.png)

After a bit of research I was able to find a few like minded people who have either attempted or made this project. One example and the source of most of my project came from this build. [link to adafruit blog](https://blog.adafruit.com/2014/12/03/pipboy-3000-arm-mounted-computer-wearablewednesday/)

![Pip Boy 3000](https://github.com/jbeeby/Final/blob/master/pipboyhope.jpg)

But I do know that my knowledge with linux, python and raspberry pi lacking this will be a challenege project. So my Hope is that it will turn out something that resembles this picture above but my main focus for this project will be creating a mobile raspberry pi. With that the power supply will be what I focus on the most.
With this in mind I searched online and even a few forums/ blogs and emailed a few cosplay outfit fabricators to get a general idea of which direction I should head in. This led me to a blog on the adafruit website that had a detailed instruction on making a pip boy.
[instructions](https://github.com/jbeeby/Final/blob/master/raspberry-pi-pipboy-3000.pdf)
Thinking that this will make it easier I begin to find the parts for my project. Being cheap, I substitued some of the parts listed with ones that I thought would work, and for the most part it did. For the most part all the parts I recieved worked exactly as I had hoped, except for one. The screen I bought was just slightly different then the one used in the project, a difference I did not notice until later in the project. With a few of the parts on back order I started off where I could.

The whole project was going to be mounted and incased in a 3D printed wrist mount, and though I had the files to print them this was my first major Issue with the project. My access to the 3D printer was hindered due to technical issues with the printer itself. Thinking it might be fixed before my project was due I started with the software part.

Since the instructions game me a link to the ISO for this project I thought it would be straight forward. I downloaded it, and burned it on 1 of 2 micro SD card I had. Once this was done I then installed it onto the Pi, hooked up a monitor, mouse and keyboard and turned it on. No luck, just a rainbox of death screen. Thinking it might be because I was using an HDMI cable and not a LCD screen I plugged that in and tried again; with no luck again. After a bit of research, and choice words, I found that others were having issues and it was advised to load raspian first then use a python prgram to emulate the pip boy. So switch modes I tried this, and once I was able to boot up the raspberry pi I downloaded the emulator and followed the instructions. Hoping that this would fix it, again no luck. After many attemps with this I just could not get the emulator to work. From here I contected both of the authors of the emulator and the instructions to see if could get some guidance. So I began to work on the electronics until I heard anything.

Though it had been over a decade I was happy to see that my soldering skills had not been totally forgotten. Though my precision was a little off due to current events, I was happy I could still solder as well as a could. First up was the power circuit; I needed to have a rechargable battery be able to have an output of 5 volts. Thankfully the PowerBoost 1000C took my 2200mAh 3.7 Volt Lithium battery and was able to convert it. Adding a simple switch to the circitry I was able to creat a simple power source that I could turn on and off.

Next I started attaching the speaker; still the 3D printer was not fixed but I had hoped it would be in time. I wired the simple speaker to an Audio amp that was then connected to the power circuit. With the addiction of wiring a headphone jack I created a basic portable speaker that I could adjust the valume with a screw driver. 

I then prepared an LED light to be connected as well to keep the looks of the pip boy as authentic as possible. Once that was done I started with wiring a rotary switch that would take in place of a mouse when using the python emulator. I had not heard back yet from anyone but I was still hopeful. Once the rotary switch was wired up, I came to my first major fork in the road. To proceed with the build I needed the 3D printed case, but it was still not fixed. At this point I decied to proceed with the build without the case thinking that I could always just resolder everything once I get the case and even if I dont then I can still have a working prototype that I could display. So I began to proceed to the next step, soldering the rotoary switch to the screen which inturn would be connected via GPO to the raspberry pi.

This is where buying off brand bit me in the butt, my screen did not have this option. After looking at this in a couple different ways I came up with a gap-fix, solder everything straight to the raspberry pi directly. Before I started this endevor I checked with the two builders to see if they had a fix for the python code. One never got back to me and the other had a couple of possible fixes but could not be bothered to try them. 

With this news I had to revaluate my design. Looking back at my propsal I decided to focus on just the major concern I had, creating a mobile raspberry pi. So I started to salvage what I could since I only had 6 days left before this was due. I scrapt the speaker and kept the power supply; since the pi is bluetooth enable i can just use a bluetooth speaker for sound. Instead of trying to use a rotarty switch on the pi i decied to just use my bluetooth keyboard for navigation of the pi when my fingers are just too big. And since i have the bluetooth keyboard i dont need to have the usb ports open for connection. 

I then used some scrap wood to create a quick case because I was told a week or so "you gotta create some sort of arm case becuase that would just be cool." So with that in mind I began creating a case. Once cut I glued the pieces together and began to sculpted the edges to get a better fit. After that I sanded and spray painted the case to give it a slighly better look. added some elastic to the under carrage i made it so it can be worn on my arm. Though I dont want to because i mounted the component with nails to be temporary so i can eventually print off the case i wanted and modify it later.

![My Pip Boy](https://github.com/jbeeby/Final/blob/master/f1.jpg)

![My Pip Boy](https://github.com/jbeeby/Final/blob/master/f2.jpg)

![My Pip Boy](https://github.com/jbeeby/Final/blob/master/f3.jpg)
