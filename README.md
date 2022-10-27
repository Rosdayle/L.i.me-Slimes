

![Logo](https://i.gyazo.com/7941d6748db107002712ad53378ea480.png)

# Behold its a slimy L,i,me
The first practical and publicly available (*at time of writing*) full 9/(13) IMU case and hardware solution. 
  Each main slime supporting more than 2 IMU's without any software modification. Daring to be a small evolution and GIANT leap for all of slime kind!

The projects goals were to streamline (*at time of writing*) a full set of 9 imus as much as possible while staying practical, as well as publicy introduce and encourage the use of multi IMU setups. And prepare for out of the box ideas and additions by others of the slime community and I (whoever comes up and implements the crazy ideas first HA! I love this community) oh and because Erimel decided to make another point of tracking, MUCH love you clever orange fox

As well as introduce many small innovations in hopes for others to be inspired by
and guarantee no performance loss for when using multiple IMU's
Additionally this was to also help facilitate the transition from existing built trackers to a more streamlined setup (I went from ~red~ cases to this)


From the
- **"Amount of components"** used to reduce costs and significantly reduce build time
- **"Overall design"** to increase ergonomics and be the smallest and lightest* overall 9 imu design solution to date, Easier donning and doffing of trackers
- **"Customisability"** for custom layouts and possible addons. Layouts can go from 1+2, 1+3 heck even 0+4
- **"Usage"** Comfort and increase in postions/movements where trackers would traditionally become cumbersome or uncomfortable. Sturdy to protect components. And at the end of the day easy to charge to do it all again

# Who is this for?
- L,i,me is for those who wish to streamline their current standard slime setup by easily converting into a L,i,me
- For those who want to make a full no compromise 9 IMU setup from the start (With the option to add an extra 4 more IMU's for shoulder and elbow tracking)
- People on a tight budget but want a performant full 9 IMU setup (with the option to add shoulder and elbow tracking in the future)
- Those who intend to use slimevr for mocap and vtubing

# Why choose L,i,me?

- Unlike **standard slimes** that can only support **2 IMU's**. Each main **L,i,me** supports **4 IMU's** (without any software modification). 
- Meaning you only need to make 3 L,i,me units instead of 6 standard slimes for a full 9 IMU setup
- As a result there are less parts
- Making L,i,me the cheapest full 9 IMU setup (As well as 13 IMU setup with optional addon)
- No compromises to performance due to hardware layout
- Aimed at providing the best stable tracking with comfort and full maneuverability due to being less bulky overall (Less main units)
- Only need to charge and maintain 3 units (4 if you include the optional addon)
- Modular and customisable
- Ongoing support
**Doing more with less**
- Less units
- Less parts
- Less costs
- Less building
- Less maintaining
- Less units to charge


TLDR the quote **"Less is more"** hence the name L,i,me



**mind the mess**, everything is still **WIP**
If you want to see my journey and **more info** of the L,i,m,e check this out https://discord.com/channels/817184208525983775/823930029070876736/939874280802484266

**For any enquires or need for help @Loler920a-Frank on the SlimVR discord server**




# How does it work? 
A typical tracker would have a single D1 mini that can support up to 2 IMU's. 
Well put simply we just added a second D1 Mini board to and thats it done, really thats it
And because of that you can connect an additional 2 IMU's making it a total of 4 supported IMU's. All without altering a single line of code in current slime firmware

The original intended layout is to have 3 main units, with 1 IMU inside and 2 IMU AUX/EXT each. 
- 2 Main unit goes on feet and the other 2 AUX/EXT goes on ankle and thigh
- 1 Main unit goes on chest and the other 2 AUX/EXT goes on waist and spine
It is the authors belief that this provides the most range of movement with no discomfort


However with elbow tracking on the horizon, you can have 1 main unit have 1 IMU inside with 2 IMU AUX/EXT out and have 2 main units with 1 IMU inside and 3 IMU AUX/EXT
- 1 Main unit goes on feet and the other 2 AUX/EXT goes on ankle and thigh
- 1 Main unit foes on feet and the other 3 AUX/EXT goes on ankle, thigh and hip
- 1 Main unit goes on chest and the other 3 AUX/EXT goes on waist and elbows

Edit- Elbow tracking addon for L,i,me is working but requires testing before public release 

In short we cover every single point of tracking with the use of 3 units, while being the smallest and lightest overall 



The first Lime
![Logo](https://i.gyazo.com/36a4285f534224af641c47bb5025e2df.jpg)


Overall layout on an older model
![Logo](https://i.gyazo.com/be5054ebee7b912464fb57d1074dd8e4.gif)




## Index

 - [Parts](https://github.com/Loler920a/L.i.me-Slimes/blob/main/README.md#parts-list)
 - [Variants](https://github.com/Loler920a/L.i.me-Slimes/blob/main/README.md#variants)
 - [Hardware layout](https://github.com/Loler920a/L.i.me-Slimes/blob/main/README.md#hardware-layout)
 - [Wearing](https://github.com/Loler920a/L.i.me-Slimes/blob/main/README.md#where-to-wear-gosh-that-a-tongue-twister-where-to-mount)
 - [Credit](https://github.com/Loler920a/L.i.me-Slimes/blob/main/README.md#author-and-people-to-note)

## Parts List ##

Here is your Shopping list. Items linked are what I personally use.


| Part | Quantity     | Description/Usage                | Notes |
| :--- | :---    | :------------------------- | :-------------------------  |
| TP4056 | x3 USB C | Charging board to charge the battery in the main tracking unit| Best to take USB C|
| Wemos D1 | x6 | Mini computer w/ wifi to connect to your PC and send IMU data | Be sure to have a micro USB cable that allows data transfer and is not only for charging |
| Switch SK12D07VG3 | x3 | A switch to turn the tracker on and off ______________________________________ =_= really | At the moment the case only supports SK12D07VG3 |
| 40mm straps | x2 500mm x2 300mm | To allow for trackers to mount to your body as well as create a pseudo harness | These straps are also elastic, the harness made will keep trackers secure |
| GoPro chest harness | x1 (Optional but recommended) | To mount the chest tracking unit | Technically this is optional but highly recommended for the harness set up|
| LAN Cable | x1 minimum 3m | For use as AUX/EXT cables and as well as a source for main tracker wires | Keeps AUX/EXT cables protected and neat, helps prevent cross talk and is a good source for easy to use wires for the main trackers, you might have spares around|
| IMU (Select from below) | x9 overall (Mix match possible) | These track the rotation of each point and limb they are attached to | Due to chip shortages, and interest in IMU tracking, prices and quality will fluctuate, some IMU's may be non functional, lower end IMU's will drift more overtime |
| BNO08x |  | ~~Considered the best IMU SLIMEVR supports has built in stabilisation for ARVR use | Due to recent price rise and shortage of this IMU, the SLIMEVR community and I can't recommend this anymore. ( I use these) |
| ~~BNO055~~ | Apparantly same size BNO08x | ~~Not exactly the 2nd best but its really a BNO08x without the  stabilisation for ARVR~~ |~~I can't personally comment on this IMU~~|
| ~~MPU 9250~~ | Apparantly same size BNO08x | ~~Now one of the most selected pick due it's price to quality, has magnetometer for stability~~ |~~I can't personally comment on this IMU, but apparantly controllers and a bad environment will affect the magnetometer if its enabled~~|
| ~~MPU 6050~~ | 3D files experimental but functional | ~~Now one of the most selected pick due it's price to quality, apparantly same as 9250 without magnetometer~~ |~~I can't personally comment on this IMU~~|
| Lipo battery 585460 | x3 ( =  or < than 56 x 56x 5.8mm) | The power source of the main tracker 20000mAh (Thats alot of power) | If not sourced locally, shipping times may be quite long. Try get one with built in protection as well. Maximum supported battery dimension 56x 56 x 5.8mm you could use blutak to fill in gaps if you are using a smaller battery to prevent rattling and wires breaking and causing shorts/sparks



Australian local sources WIP/TBD
- I suggest you get batteries from CORE electronics





## Variants

**Loler920a selection**
- Variant A has the traditional handles seen in most slimes
- Variant B has no handles on the case, but instead uses the lid as a handle (A daring new concept)
- Solder guide was specifically designed tool to reduce excess wires and make soldering an easier experience (First of its kind)
- Chest adapter Was specifically designed to allow for Variant A to mount to a gopro chest harness for comfort and stability (Not a new concept but first of its kind really)

| **Loler920a selection** | **Recommended selection**     |
| :--- | :---    |
| Case and lid A x1 | Case and lid A x1  |
| Case and lid B x2 | Case and lid A or B x2 (Your choosing) |
| Divider BNO080 x3 | Divider (IMU) x3  |
| Aux BNO080 case x 6 | Aux (IMU) case x 6  |
| Aux Lid x 6 | Aux Lid x 6 |
| Solder guide (BNO080) x1 | Solder guide (IMU) x1 (Strongly Recommended |
| Chest adapter x 1 | Chest adapter x 1  |


Variant B has no handles, the lid will act like them for you
![Variant B](https://i.gyazo.com/87eb916b487218307826515c56ce38e5.gif)


## Hardware layout 
Due to being a slightly different hardware layout, here is a wiring diagram to follow.
Note to self clean up these diagrams

**NOTES for recommended layout**


- Size the AUX/EXT cables as you go with your limbs in flexed and extended with your intended layout to allow for enough cable slack for a full range of movement as well as not have an excsessive amount of wires, to prevent tangling/snagging. Though its better to have overestimate than underestimate as this is more easier to fix in the future.
- Before soldering the 3rd IMU loop the LAN cable through inside of one of the velcro straps to this will prevent the cable from flapping around loosly
- It is normal for LAN cables to be tight fitting into the case you will need to push it in there, twisting it in helps
- Plan where your soldering iron is going you do not want to burn other wires you just soldered on
- Boards will be tight fitting in the actual case (Let me know if its to tight)


Make sure to have your soldering guide ready
![Guide](https://i.gyazo.com/fddadf71537a5d73609fabd8beb3e79f.png)


BASE Layout (Start with this)
Best to do the diode first
![Base](https://i.gyazo.com/69dc7c70b8b11fc3a2775c80673a7aa6.png)



3 IMU LAYOUT (The main and recommended layout)
![3 IMU LAYOUT here](https://i.gyazo.com/aa39ab299450ce945091e0bdfc0138fa.png)

4 IMU layout here (This is aimed at the elbow and shoulder tracking addon)
![4 IMU LAYOUT here](https://i.gyazo.com/df23a269be14a751d016d65494852174.png)


A full L,i,me unit set without elbow tracking
![Final product](https://i.gyazo.com/10f5527647f185ca48843e1c9ce8461f.jpg)


Also to get proper battery readings edit batteryADCMultiplier in batterymonitor.h

![Battery code](https://i.gyazo.com/a5cd4523d019b85590b168fd06be50fb.png)

Replace line 40 with
   #define batteryADCMultiplier 1.0 / 1023.0 * 6.8


## How to wear (Loler920a recommendation)

--Note to self release diagram and pictures


- Main unit on feet
- AUX, ankle inside, behind ball
- Strap below knee
- AUX, Outside
- Main unit chest
- Wire over shoulder
- Secure to go pro harness
- Aux waist thinnest part of body/above belly button area
- AUX hip belt line

- (Recommended) - Straps from hip strap to connect to thigh straps, to prevent sliding thigh trackers sliding down leg
- The three point buckle (x2) should be on your hip strap, left and right. Loop a velcro strap through the bottom loop and through itself, then connect it to the upper leg strap. (This prevents the upper leg from sliding down)
- (Authors Recommendation) Wear it underneath your clothes for comfort, least sliding and bunching. Wear a singlet/undershirt if if you like.


# FAQ

- **Can I use this with other standard slime trackers?**

Yes, yes you can

- **This is my first time soldering or doing DIY with electronics, is this ok for me to build?**

If you have confidence that you can or learn to splice cables cables together, then you should be good. 
Thats probably the hardest thing in a standard slime build as well, though you will be doing it more with L,i,me


- **Can I convert my standard slimes into L,i,me's**
Yes, in fact I converted my previous slimes into this. Though you may want to change the battery and switch

- **I don't have enough IMU's can I add them later?**
Yes you can in fact start off at minimum 6 IMU's and addon the other IMU's later. Please be sure to plan ahead


- **When will the elbow and shoulder tracking addon be available?**

When I finish testing and can confirm there are no issues

**When will the Neck tracking addon be available?**

When I get to it

**Can I lie down, roll or whatever on the tracker and its extensions?**
Sure go ahead, you will find nothing will prevent you from doing so


- **The IMU I want to use is not listed what do I do?**
You can contact me on the slimevr discord and ask me to model the 3D files for you

- **I have an issue**
You can ask on the slimevr discord for help or from me if you like

- **Where is the L,i,me software?**
There is none, L,i,me is exclusively a hardware solution and will work seemlessly with slime

- **What are the octoslime files?**
WIP models to support octoslime. These are currently only for show



## Author and people to note

- Loler920a Author and creator of the L,i,me
- HolyLemon pointing out potential issues, reviewing the wiring, and giving the correct vaulue for the battery readout. All in an effort to help prevent magic smoke
- Lemming for secondary testing
- Erimel (although not intentional) for being the final pushing reason why to go ahead with this idea. Though thanks for helping pick the name
- Eiren for making slime VR a thing as well as making it open source



Note to self clean this up more !!! Make a recommended SECTION for how this should be layed out. OR JUST WRITE IT AS RECOMMENDED
ALSO note/include the battery monit.h code edit as well as define.h examples
ALSO just make a comparison drawing between traditional and lime to get the point across
