# Phoenix Zoo VR Setup

## Purpose & Context
This guide details the hardware and software associated with the Phoenix Zoo VR deployment of November 2025 and contains details for both Guest Services (GS) and Information Technology (IT). 

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR, PotPlayer, Windows) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

⚠️ **Accounts and Passwords**: WPS staff have created various accounts for the Phoenix Zoo to allow for smooth functioning of the VR deployment. Details of these accounts will be provided in a separate document. It is **critically important** that the credentials associated with these accounts not be changed without coordination with WPS senior support staff. WPS staff may be unable to retrieve account information if credentials are changed unilaterally and, in some cases, the VR experience may be impacted by such changes ⚠️

## Prerequisites
- None

## Quick Overview

### Hardware:
1. Quest 3 VR headsets managed by third-party software (3P) Meta-for-Work and ArborXR (includes 2 physical controller per headset) - headsets are called a **Device** in the WildXR Web portal ecosystem.
2. Reinforced USB-C cables for power supply to headsets
3. Power bricks for supply, 15W minimum
4. MeLE microcomputers running PotPlayer for video playback
5. 65" TVs
6. Kasa smart power strips, power for all hardware
7. BLU WiFi connected smartphone for account access

### Software:

#### VR Headsets:
1. Autolaunchping.apk - Installed via ArborXR, automatically launches WildXR on headset power on
2. WildXR.apk - Installed via ArborXR, automatically launched by autolaunchping.apk
3. ArborXR suite - Installed via ArborXR to manage headset general settings
<div style="page-break-after: always;"></div>

#### MeLE computers:
1. PotPlayer - Installed by WPS, runs video on loop on startup (added to startup folder)
2. MeshConnect Agent - Installed by WPS, used for remote management by WPS support staff
3. Windows Update Blocker (WUB) - Installed by WPS, used to prevent automatic Windows software updates which can impact user experience
4. AutoHideMouseCursor - Installed by WPS, used to automatically hide mouse cursor during video playback

#### BLU Phone:
1. Google Authenticator - Installed by WPS, used to provide 2FA to other apps or websites
2. Kasa - Installed by WPS, used to manage Kasa power strip settings and schedules
3. Meta Horizon  - **Discontinued Use** Installed by WPS but contraindicated by use of Meta-for-Work and ArborXR

## Details

### Hardware

1. **Quest 3 VR Headsets**
   - *Details about the Quest 3 headset is readily available online, WPS Staff recommends referencing the internet for images and detailed steps that may assist you in any problems you may encounter*
   - *All headset/controller groups are labeled with a 7-character s/n, this is the last 7 characters of the s/n provided by Meta and can be found on the headset left temple and inside the controller battery compartments*
   - **Protective Cage** - 2 piece aluminum. Protects headset from casual damage during everyday use. Secured by 2 security allen key bolts. Flanges on bolt-receiver locks bottom of cage to headset Prevents easy access to power button - drilled to allow intentional access.
   - **Power Button** - Located beneath the left temple. Accessible through drilled hole on cage. **Short Press** - cycles sleep state on headset. **Long Press** - cycles power state on headset. **Excessively long press** - force system reboot on headset (rarely needed)
   - **Interpupillary distance dial (IP dial)** - Located bottom of headset, left of nose. Sets the IP distance for headset lenses influencing focus of VR image. May need adjustment by user on case-by-case basis.
   - **Volume control rocker** - Located bottom of headset, right of nose. Rocking towards nose decreases volume, away from nose increases volume. When controllers are not present, can be used as a selector button for gaze reticle in menu screens and dialog boxes.
<div style="page-break-after: always;"></div>

1. **Quest 3 VR Headsets - cont.**
   - **USB C port** - On left temple. Allows both data transfer and power supply to headset. ⚠️*This port is a weak point on the headset and can be damaged if impacted or torqued*⚠️
   - **Headset Cameras** - Central camera manages depth perception, side cameras are a combination of color and IR, all for mixed reality experience (passthrough).
   - **Headset Sensors** - Two on lower "cheeks" of headset used for positioning in space (tracking use position), internal sensor between lenses used for detecting user presence (presence sensor).
   - **Double tap on headset case** - If not managed in settings could provide passthrough (ability to see surroundings) when in Quest main menu. Should not impact WildXR viewing or playback.
   - **Headset Fan** - Internal, top main dome of headset. Cools headset and occasionally can be heard in very quiet environs. If excessively noisy, or if headset is uncomfortable to touch, headset should be removed from operation.
   - **Headset Status Lights** - There are two status lights on the Quest 3 headset, one in at the top center of the headset and one just above the left temple. The center LED shows external sensor activity (solid for sensor are on, blinking for casting or recording) and may not always be visible during use. The left LED shows power level (White - headset is on, Green - headset is fully powered, Orange - headset is charging, Red - headset is critically low, Flashing Red - charging issue with headset)

2. **Quest 3 VR Controllers**
   - *Details about the Quest 3 controllers is readily available online, WPS Staff recommends referencing the internet for images and detailed steps that may assist you in any problems you may encounter*
   - *All headset/controller groups are labeled with a 7-character s/n, this is the last 7 characters of the s/n provided by Meta and can be found on the headset left temple and inside the controller battery compartments*
   - *Controllers each have a **Trigger Button** (under index finger), **Grip Button** (under middle finger), a **Joystick** and three **Face Buttons**. Only specific uses will be covered as button function varies by application*
   - **Meta Button** - found on **Right Controller** is used to interrupt most applications and display resume or quit options along with screen capture and recording. 
      - *If you need to stop the WildXR application for any reason, this is the easiest, but may need to be combined with a sleep/wake cycle on the headset to interrupt the WildXR app*
   - ⚠️*WPS Staff recommends that controllers not be stored with batteries, both to prolong battery life, but also to prevent constant **Controller connection** alerts within the headset which will impact user experience*⚠️
   -⚠️*WPS Staff recommend that controllers be stored near headsets in operation, but hidden from public use as they are not needed for the proper functioning of the WildXR experience*⚠️
<div style="page-break-after: always;"></div>

3. **USB cable & Quest 3 power brick**
   - All USB cables are USB-C to USB-C cables
   - All cables are reinforced with a static climbing rope and mesh sheath to provide some ruggedness to the cable connection
   - Cables for this deployment are for constant power supply
   - Cables include a short, USB-C male-to-female, stress relief cable that attaches to the Headset and then the longer cable
   - ⚠️*Cables can be a tripping hazard and should be managed for length and to ensure no slack lays on the floor of the display*⚠️
   - ⚠️*Power issues are generally caused by loose or unplugged cables, check all joints if a headset is experiencing power issues*⚠️

4. **Silicone face mask**
   - Aftermarket face mask for Quest 3 headsets
   - Can be removed, replaced, best done with cage removed
   - Cleaning with *"Facial Towelettes"* recommended to remove grime (avoid lenses if possible)

5. **Comfort head strap**
   - Aftermarket head strap for Quest 3 headsets
   - Can be removed, replaced, cage and USB cable must be removed prior to removal
   - Provides anchor point for USB cable
   - Adjustable via dial at back of strap
   - Articulated at temples to allow fitting over some glasses and hairstyles

6. **Power and batteries**
   - Headset contains internal lithium ion rechargeable battery which gives roughly 2.5 hours playback
   - External battery can be added for an additional 1 - 1.5 hours playback
   - In WPS experience, constant power supply has not degraded battery life to a significant degree
   - Controllers take AA batteries, generally only the right controller is needed for troubleshooting issues
   - Power supply brick (socket to USB C) should be Meta brand or brick capable of supplying **15W** of power or charging may not keep pace with battery drawdown

7. **MeLE microcomputer**
   - Windows 11 OS computer in small form factor
   - Can get hot to touch, this is normal
   - Connected via HDMI cable to TV
   - Connected to Kasa power strip with proprietary PSU ⚠️**(Do Not Use off-brand PSU - Unit will be bricked)**⚠️
   - Should turn on automatically with supplied power
   - Microcomputer will be scheduled for on/off time via Kasa power strip
   - Wired mini-keyboards with trackballs are supplied for computer control by IT staff when needed
   - Managed remotely by WPS support staff (Windows updates, installed software updates, etc)
<div style="page-break-after: always;"></div>

8. **TV**
   - Brand and settings to be determined
   - Should turn on automatically with supplied power
   - Connected to microcomputer with HDMI cable
   - Connected to Kasa power strip and scheduled with on/off times to coincide with microcomputer

9. **Kasa power strip**
   - Smart power strip with scheduling capabilities
   - 3 outlets will be left unscheduled for 24/7 power supply to headsets
   - 2 outlets will be scheduled based on Guest Services requirements to cycle on/off microcomputer and TV
   - Kasa account for Phoenix Zoo will be created and populated on BLU phone Kasa app
   - Individual outlets can be cycled manually using small button to upper left of outlet
   - A small LED indicates power state of outlet, always check outlet state if power issues are persistent

10. **BLU Android WiFi only smart phone**
    - Provided to allow access to Phoenix Zoo VR related accounts
    - Should remain at display to allow troubleshooting when needed

### Software

11. **Autolaunchping.apk**
    - Small android application created by WPS to allow auto launch of WildXR application on headset startup
    - Can provide "proof-of-life" ping to a healthchecks.io URL if desired to allow remote monitoring of headset state
    - *healthcheck.io ping relevancy questionable with ArborXR integration - contact WPS staff if desired or concerning*
    - Installed automatically via ArborXR settings, visible in **"For Work"** library section of application
    - ⚠️**Must be launched once prior to putting headsets into public use or WildXR will not auto launch on startup**⚠️
    - ⚠️*After initial launch, no interaction is needed under normal operating conditions*⚠️
<div style="page-break-after: always;"></div>

12. **WildXR.apk**
    - Base application that provides the WildXR VR experience
    - Designed and created by WPS staff
    - Provides two experience modes:
       - Single video loop for tightly curated experience - video restarts when new user dons headset, minimal user interaction
       - Open experience - users choose which video to watch from a curated collection, more user options within application
    - The WildXR experience on a headset is called an **Installation**
    - **Installations** can vary in what is shown to a guest, and how it is shown
    - **Installations** can are assigned to headsets via a **WildXR number** that identifies a headset to the WildXR.org web portal
    - Headset experiences can be managed via the WildXR.org portal, but that is beyond the scope of this guide

12. **WildXR.apk - cont.**
    - Reference the **"Web Portal Guides"** for details on managing **Devices**, **Installations**, and other aspects of the VR experience
    - ⚠️*WPS recommends that, initially, all videos required for an **Installation** be sideloaded (physically installed) onto the device*⚠️
    - ⚠️*Streaming or downloading video content is highly dependant on internet bandwidth and stability and almost always degrades the user experience*
    - *The WildXR application is available for free to owners of Meta VR headsets through the Horizon Store or Rift Store*
    - ⚠️*Custom content is not available to the general public through the WildXR application*⚠️

13. **ArborXR Suite**
    - Remote management software installed by ArborXR
    - Required for remote management by WPS support staff
    - WPS does not control or influence the features or effects of ArborXR suite software

14. **PotPlayer**
    - A video playback freeware program installed on supplied microcomputers by WPS staff
    - Settings and updates will be initially managed by WPS staff remotely
    - Set to launch automatically on computer startup (added to startup folder)
    - Set to launch and loop single selected video via PotPlayer settings
<div style="page-break-after: always;"></div>

15. **MeshConnect Agent**
    - MeshConnect is a self-hosted (hosted on a server controlled by WPS on Microsoft Azure) remote access program
    - Allows WPS support staff to remotely access microcomputer to aid in upkeep and troubleshooting
    - No requirement for local permissions to remote access, but all non-system level actions should be visible to institutional staff via the attached monitor/TV
    - Remote access highly dependent on internet bandwidth and stability and may be unavailable at times

16. **Windows Update Blocker (WUB)**
    - Freeware program installed by WPS staff
    - Used to prevent automatic Window OS updates from interrupting guest experience
    - Can be switched off to allow support staff to manually apply updates at scheduled times
    - Can influence the successful updating of other software packages

17. **Auto Hide Mouse Cursor**
    - Freeware program installed by WPS staff
    - Used to automatically hide the mouse cursor to enhance guest experience
    - Cursor reappears on mouse movement and will automatically hide after 5 seconds of inactivity

18. **Google Authenticator**
    - Installed on BLU phone to allow access to accounts that require two-factor authentication (2FA)
    - Account access can be installed on personal or work phones as needed by organization
    - *Google Authenticator allows multiple accounts to be stored in the 2FA application*

19. **Kasa**
    - Installed on BLU phone to allow control and monitoring of Kasa smart power strips
    - Will be associated with Phoenix Zoo account
    - Can be installed on personal or work phones as needed by organization

20. **Meta Horizon**
    - ⚠️*Use of the Meta Horizon app is not needed for the standard VR deployment and will only be necessary under specific circumstances*⚠️
    - ⚠️*If VR headsets are removed from 3P management, WPS staff can assist the migration of headsets into the **Meta Horizon** ecosystem - this is a time and labour intensive process*⚠️
    - Installed on BLU phone to allow management of personal headsets through Phoenix Zoo account
<div style="page-break-after: always;"></div>

## The VR experience in WildXR

### Initial Setup and Launch
These steps will have been completed by WPS staff on deployment. They are covered here to allow for replacement headsets to be incorporated at a future date if needed. Reach out to WPS staff is assistance or clarification is needed

**Autolaunchping and WildXR**
- When WildXR is installed on a **Device** it must be launched once to build a file structure on the headset
- WildXR will not be launched automatically until the Autolaunchping app has been run once
- Autolaunchping will show a small interface for entering a URL endpoint, this interface will be hidden by WildXR in most cases, and will not show again on subsequent headset boot up events
- If the Autolaunchping interface is needed, manual launch the app from the **For Work** section of the app library
- WildXR must be tied to a **Device** through the Wildxr.org web portal (see the **"Web Portal Device Management Guide"**) to show custom content

**Video sideloading**
- Video content can be streamed from the cloud, but is not recommended for public use as quality is highly dependant on internet bandwidth and stability
- Video content can be downloaded to **Devices** and can be triggered manually or automatically based on **Installation** settings assigned to the **Device** (see respective **Web Portal Guides** or contact WPS staff for assistance)
- Video download is dependant on internet bandwidth and stability and can result in artifacts if interrupted
- Videos can be sideloaded (directly transferred to the **Device**) from a computer via USB C cable and is the preferred method of installing multiple videos.
- *WPS Staff will generally install the entire WildXR catalogue onto devices as SOP, but this may not include custom content - Contact WPS Staff for clarification of what has been installed if there are concerns*
<div style="page-break-after: always;"></div>

### Daily operation
- WPS recommends staff perform a functionality check of all hardware associated with a display each day prior to opening and once again prior to display close
- Cleaning each headset along with functional morning and evening checks is recommended
- Adjust cable length and check for security to physical cabinets (guests cannot pull to gain more cable length) daily with morning functional check
- If pest species are present on grounds (crickets, cockroaches, etc) check for presence during AM checks and consider bagging headsets in mesh vegetable bags overnight 
- ⚠️**Avoid storage headsets in plastic bags or any material that will allow heat buildup or headset damage may occur**⚠️
- Check cage bolt tightness once per week or after especially heavy use days

**Stand alone headsets**
These VR headsets are connected to power so that they are ready for guest use at any time. The WildXR will be playing and need no interaction by staff of guests (save for volume and IP adjustment). Videos will start from the beginning for each new guest that dons the headset (presence sensor between lenses may need cleaning for consistent behavior). Videos may restart if the guest "peeks" out of the headset.
*Any issues can generally be solved by rebooting the headset (power off / 15s pause / power on)*
*If menu or alert interaction is needed, a gaze reticle should appear and selections can be made using the volume rocker button*

### Looped video installation

**Single video experience**
- Headsets are assigned an **Installation** that loops a single video on startup. 
- Videos will restart automatically after a brief fade out of image and sound. 
- Videos will restart when a headset is removed and donned by a new guest.
- The looping video assigned to a headset can be changed - see the **Web Portal Guide** series for help with assigning an **Installation** to a **Device**.

### Visitor choice installation

**Multiple video experience**
- Headsets are assigned an **Installation** that offers a curated catalogue of videos.
- Guests will navigate a globe interface to choose from either **Map Markers** representing a video/collection of videos, or from a **Menu Tray** showing **All Clips** or **Short Films**.
- Guests have the ability to play more than one video
- Guest have the ability to pause, rewind, and fast-forward videos
- Guest can choose to stop a video before the videos natural end
<div style="page-break-after: always;"></div>

## Troubleshooting

**Headset chimes and shows a "Port Debris Warning":**
- Using the gaze reticle or hand controllers, select the **"Ok"** button to clear the alert
- Alert generally appears on power up, wake up, and when USB cable is reconnected
- Alert will overlay WildXR and all other user interfaces
- Caused by a firmware issue of the headset itself and *rarely* relates to actual debris within the USB port
- Port cleaning, with compressed air, may reduce the frequency of the alert in some cases

**Headset display appears frozen:**
- Tap the power button once to sleep the headset and again, after a brief pause, to wake the headset
- Display should return to normal upon wake - if problem persists, reboot the headset (power off / 15s pause / power on)
- Occasionally occurs when headset wakes from overnight sleep state or with reboot of headset and launch of WildXR

**Black screen which appears on with or without audio playing:**
- Tap the power button once to sleep the headset and again, after a brief pause, to wake the headset
- Display should return to normal upon wake - if problem persists, reboot the headset (power off / 15s pause / power on)
- Occasionally occurs when headset wakes from overnight sleep state or with reboot of headset and launch of WildXR

**Video not starting from beginning for new users:**
- Clean the presence sensor with a cleaning wipe (between the headset lenses) and retry
- Generally caused by grime on the sensor window
- If problem persists, reboot the headset (power off / 15s pause / power on)
- If problem is chronic, contact WPS staff as this can be influenced by **Installation** settings

**Volume adjusts on it own, remains too quiet or too loud:**
- Cage might be pressing on volume rocker switch
- Adjust cage and try manual adjustment again
- Rocker switch may need cleaning

**Display is out of focus:**
- Lenses may need cleaning with a lens cloth or microfiber cloth
- IP dial may be out of adjustment, direct user on how to adjust IP for their eyes
- Users with glasses may not be able to adjust the IP to help with vision issues

**Headset too loose or too tight:**
- Adjust head strap with dial at back of strap
- Adjust velcro strap along top of head strap
<div style="page-break-after: always;"></div>

**Headset plays incorrect video:**
- Headsets (**Devices**) are assigned videos (**Installations**) based on their **WildXR Number**
- These settings are available on the Wildxr.org web portal and can not be changed by directly interacting with the headset
- Changes to the assigned **Installation** will only take effect when a **Device** is connected to the internet and WildXR is relaunched
- Contact WPS staff if assistance is needed or consult the **Web Portal Guide** series for more information

**Headset video plays once and does not loop:**
- Headsets (**Devices**) are assigned playback parameters (**Installations**) based on their **WildXR Number**
- These settings are available on the Wildxr.org web portal and can not be changed by directly interacting with the headset
- Changes to the assigned **Installation** will only take effect when a **Device** is connected to the internet and WildXR is relaunched
- Contact WPS staff if assistance is needed or consult the **Web Portal Guide** series for more information

**Headset opens into a Globe scene:**
- Headsets (**Devices**) are assigned a guest environment (**Installations**) based on their **WildXR Number**
- These settings are available on the Wildxr.org web portal and can not be changed by directly interacting with the headset
- Changes to the assigned **Installation** will only take effect when a **Device** is connected to the internet and WildXR is relaunched
- Contact WPS staff if assistance is needed or consult the **Web Portal Guide** series for more information

**Video playback is choppy, lags, or has audio distortion:**
- These are symptoms of streaming video
- Videos may not have been downloaded or sideload properly
- If recent adjustments have been made to content, new videos may have been assigned and not loaded onto the **Device**
- Consult the **Video file transfer guide** for steps on sideloading video content
- WPS can assist with file location and download if needed

**"Device appears offline or no videos downloaded" warning appears:**
- Occurs when a **Device** is not connected to the internet and no videos associated with the current **Installation** have been downloaded or sideload
- Connecting the **Device** to the internet will prevent alert from showing, but videos will stream, resulting in lower quality
- WPS recommends sideloading or downloading the video files associated with the **Installation** before using in the public
<div style="page-break-after: always;"></div>

**Device not showing WildXR - displays multiple menus:**
- The headset is most likely in the main Meta Horizon interface
- This may happen due to WildXR quitting unexpectedly or user tampering
- Select the WildXR application icon in the menu-tray with the gaze reticle and launch via the volume control button
- *You can also reboot the **Device** if needed to check that the autolaunch program is functioning as expected* 

**Headset loses power during day:**
- Check all USB connection sites as power cable may have become disconnected
- Check that power brick is firmly inserted into socket
- If a smart power strip is being used, ensure that sockets are on and providing power
- If a smart power strip is being used, ensure that the sockets are not scheduled on/off at certain times of day (via Kasa application)
- Check main power source if power is lost across multiple devices
- Continued power issues may indicate a damaged USB cable or damaged USB headset port
- Replace a USB cable before writing off a headset as damaged

**Headset fan is audible or headset face is becoming hot to touch:**
- ⚠️**If either of these signs are present remove the headset from public use immediately**⚠️
- Damage to a headset fan, usually caused by a hard impact, is difficult and expensive to repair and generally mean retiring the headset from use
- A hot (not warm) headset may indicate that a fan has failed completely and could injure a guest of kept in public use

**TV shows *"No Signal"* not video playback:**
- Boot timing with microcomputer and TV is off
- Either microcomputer or TV powered on prior in advance of paired device
- Power cycle tv (turn off / wait 15s / turn on) or power cycle Kasa smart power strip
- Adjustments to outlet schedule via the Kasa application may be necessary if problem is chronic
- ⚠️*Make sure that staff are not manually turning off / on the tv or computer as this can cause linking issues*⚠️
- ⚠️*Organizations may find it more reliable to have staff manually turn TVs and microcomputers on at the start of shift if linking issues are chronic*⚠️

**Windows desktop displayed on TV:**
- Failure to automatically launch PotPlayer (or other video playback software)
- WPS adds the video playback software as a shortcut to the Windows startup folder
- Check for shortcut in startup folder (Windows Key + R, type "shell:startup", hit enter)
- Create a new shortcut linked to software (PotPlayer, vlc, etc)
- Software may have been moved or updated which can cause autostart issues
- If issue persists contact WPS staff for assistance
<div style="page-break-after: always;"></div>

**Video playback software showing update screen:**
- If you see cursor movement on the screen you computer may be being controlled remotely by WPS staff or your IT department to apply updates.
- If possible confirm that no remote access is happening before moving on to next steps (WPS will generally attempt maintenance/updates late Monday or early Tuesday Denver time)
- Cancel any pending updates and check Settings -> General Settings -> automatically check for updates - this box should either be unchecked or set to "Never" as a dropdown menu option
- Remember to click the **"Apply"** button in the bottom right corner to apply the changes
- Contact WPS staff or you organization's IT department for further assistance

**Video playback software plays video once but does not loop:**
- Incorrect playback options set in PotPlayer
- In PotPlayer window hit F5 (opens settings menu).
- Navigate to Playback -> Playback Settings -> Select "Repeat Video Playback" and choose "Enable: Repeat playing item" from the drop down menu.
- Click the **"Apply"** button in the bottom right corner to apply the changes
- Click the **"Play"** button in the bottom left portion of the PotPlayer window (you may need to hover near the bottom of the screen to show the playback controls)
- If the video does not play and loop, restart PotPlayer
- If the video does not play and loop, navigate to the **"Videos"** folder and double click the video found there (there should only be one video in the top left of the **"Videos"** folder, do not use videos found in the **"Storage"** folder if present)
- If the problem persists, contact WPS staff for assistance

**Video playback is unusually slow or fast:**
- Depending on the size and resolution of the video attempting to be played, the microcomputer system may have difficulty with smooth playback
- If the video file was supplied by WPS, contact WPS staff for a new video file for playback
- Only the video playback software should be open, other software (Web browsers, system updates, etc) can interfere with smooth video playback
- Quit and restart the video playback software to see if this resolves the playback issue

**Kasa smart power strip not providing power:**
- If none of the outlets are providing power the power strip may be turned off, check the main switch
- If the main switch shows that power should be supplied to the strip, check the building power (or contact the appropriate staff) as there may be upstream power issues
- If only some of the outlets are providing power, check that the outlet is powered on (a small button at the top left of each outlet cycles power state) 
- A small white LED light should be lit when an outlet is providing power
- Kasa outlets may be set to a schedule for power supply, check in the Kasa application for applied schedules
<div style="page-break-after: always;"></div>

**Kasa smart power strip not responsive in the Kasa application:**
- Communication between the Kasa smart power strip and the Kasa application is dependant on internet connection
- Check that an internet connection is available and that the device running the Kasa application is connected to the correct network
- Kasa smart power strips could be reset by power surges or tampering, check the Kasa application to see if the non-responsive strip is present in the device list

## Important Notes

⚠️ **Account Credentials**: WPS staff will create various accounts that are required for the VR deployment. Please coordinate any changes to account credentials with WPS senior support staff. WPS staff may not be able to retrieve account access if lost and this could critically impact display functionality.

⚠️ **Headset life**: Quest 3 headsets are robust but not indestructible. Monitoring guests for negative interactions with equipment will prolong the life of all VR equipment. Physical damage is by far the most common cause of headset replacement.

⚠️ **Guest safety**: VR experiences are new for the majority of guests. Reactions to VR content is hard to predict. WPS staff recommends reviewing possible safety concerns on a regular basis to align with organizational risk tolerance. Hazards such as tripping, falling, and tipping of equipment must be assessed by the organization and is beyond the scope of this guide.

⚠️ **WPS Support**: WPS Staff look forward to assisting you with any issues you may encounter while deploying a VR system. WPS staff is generally available during normal business hours (Denver Time), and occasionally on weekends. If you are requesting changes to content or device assignment please plan ahead and give 48 - 72 hours for changes to be implemented. New content, or content editing, takes longer and requirements should be discussed with senior support staff. For critical, time sensitive assistance, please call or use the dedicated WhatsApp channel for support.
<div style="page-break-after: always;"></div>

## Commonly used supplies

### Headset pieces

**KIWI design K4 Head Strap**
- ```https://a.co/d/3E2sRVO```

**Meta Quest 3 Silicone Facial Interface**
- ```https://a.co/d/4m69dTP```

### MeLE computer pieces

**MeLE Power Supply Adapter for Mini PC Computer Quieter2/3/4 Series/PCG02 Pro**
- ```https://a.co/d/eMhO2UT```

### USB Cable pieces

**Stress relief USB cable - cannot be used for data transfer**
**2-Pack Right Angle USB2.0 C Adapter，4inch 90 degree USB c Male to Female Extension Cable Flat**
- ```https://a.co/d/9nLRmeE```

**AOLEBA 10.5 mm Static Climbing Rope**
- ```https://a.co/d/a9CX6iL```

**Alex Tech Braided Cable Sleeve**
- ```https://a.co/d/cGpym12```

**10 foot USB C cable**
**LDLrui USB C Cable Right Angle[10ft 2Pack]**
- ```https://a.co/d/9GHdigK```

**16 foot USB C cable**
**Kuject Link Cable 16FT Compatible for Quest 3S/3**
- ```https://a.co/d/5sPqHWJ```

**3M 06133 Scotch 33+ Super Vinyl Electrical Tape**
- ```https://a.co/d/dkCVQ4y```

### Power Supply

**Kasa Smart Plug Power Strip HS300, Surge Protector with 6 Individually Controlled Smart Outlets**
- ```https://a.co/d/e61mVj7```