

![Logo](https://i.gyazo.com/7941d6748db107002712ad53378ea480.png)

# Behold its a slimy L,i,me
The first practical and publicly available (*at time of writing*) full 9 IMU case and hardware solution. 
  Each main slime supporting more than 2 IMU's without any software modification. Daring to be small evolution and GIANT leap for all of slime kind!

The projects goals were to streamline (*at time of writing*) a full set of 9 imus as much as possible while staying practical, as well as publicy introduce and encourage the use of multi IMU setups. And prepare for out of the box ideas and additions by others of the slime community and I (whoever comes up and implements the crazy ideas first HA! I love this community) oh and because Erimel decided to make another point of tracking, MUCH love you clever orange fox

As well as introduce many small innovations in hopes for others to be inspired by
Additionally this was to also help facilitate the transition from existing built trackers to a more streamlined setup (I went from ~red~ cases to this)

From the
- **"Amount of components"** used to reduce costs and significantly reduce build time
- **"Overall design"** to increase ergonomics and be the smallest and lightest* overall 9 imu design solution to date, Easier donning and doffing of trackers
- **"Customisability"** for custom layouts and possible addons. Layouts can go from 1+2, 1+3 heck even 0+4
- **"Usage"** Comfort and increase in postions/movements where trackers would traditionally become cumbersome or uncomfortable. Sturdy to protect components. And at the end of the day easy to charge to do it all again


In short going by the quote **"Less is more"**



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

In short we cover every single point of tracking with the use of 3 units, while being the smallest and lightest overall 



The first Lime
![Logo](https://i.gyazo.com/36a4285f534224af641c47bb5025e2df.jpg)


Overall layout on an older model
https://gyazo.com/be5054ebee7b912464fb57d1074dd8e4




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





## Hardware layout 
Due to being a slightly different hardware layout, here is a wiring diagram to follow.
Note to self clean up these diagrams

**NOTES for recommended layout**
--note to self Release diagram or pictures, also notes for sizing cables and looping a cable through the Strap before soldering onto 3rd IMU
For legs, the main tracking unit is on the feet, 2nd aux on ankle and 3rd aux on thigh. For spine Main unit is on chest, 2nd on waist, 3rd on hip


- Size the AUX/EXT cables as you go with your limbs in flexed and extended with your intended layout to allow for enough cable slack for a full range of movement as well as not have an excsessive amount of wires, to prevent tangling/snagging. Though its better to have overestimate than underestimate as this is more easier to fix in the future.
- Before soldering the 3rd IMU loop the LAN cable through inside of the strap
- It is normal for LAN cables to be tight fitting into the case you will need to push it in there, twisting it in helps

BASE Layout (Start with this)

![Base](https://i.gyazo.com/69dc7c70b8b11fc3a2775c80673a7aa6.png)



3 IMU LAYOUT (The main and recommended layout)
![3 IMU LAYOUT here](https://i.gyazo.com/aa39ab299450ce945091e0bdfc0138fa.png)

4 IMU layout here Don't do this unless you have a reason to
![4 IMU LAYOUT here](https://i.gyazo.com/df23a269be14a751d016d65494852174.png)


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
- Optional (Recommended) - Straps from hip strap to connect to thigh straps, to prevent sliding thigh trackers sliding down leg






## Author and people to note

- Loler920a Author and creator of the L,i,me
- HolyLemon pointing out potential issues, reviewing the wiring, and giving the correct vaulue for the battery readout. All in an effort to help prevent magic smoke
- Lemming for secondary testing
- Erimel (although not intentional) for being the final pushing reason why to go ahead with this idea. Though thanks for helping pick the name
- Eiren for making slime VR a thing as well as making it open source



Note to self clean this up more !!! Make a recommended SECTION for how this should be layed out. OR JUST WRITE IT AS RECOMMENDED
ALSO note/include the battery monit.h code edit as well as define.h examples
ALSO just make a comparison drawing between traditional and lime to get the point across
