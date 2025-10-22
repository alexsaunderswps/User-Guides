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

2. **Quest 3 VR Controllers**
   - *Details about the Quest 3 controllers is readily available online, WPS Staff recommends referencing the internet for images and detailed steps that may assist you in any problems you may encounter*
   - *All headset/controller groups are labeled with a 7-character s/n, this is the last 7 characters of the s/n provided by Meta and can be found on the headset left temple and inside the controller battery compartments*
   - *Controllers each have a **Trigger Button** (under index finger), **Grip Button** (under middle finger), a **Joystick** and three **Face Buttons**. Only specific uses will be covered as button function varies by application*
   - **Meta Button** - found on **Right Controller** is used to interrupt most applications and display resume or quit options along with screen capture and recording. 
      - *If you need to stop the WildXR application for any reason, this is the easiest, but may need to be combined with a sleep/wake cycle on the headset to interrupt the WildXR app*
   - ⚠️*WPS Staff recommends that controllers not be stored with batteries, both to prolong battery life, but also to prevent constant **Controller connection** alerts within the headset which will impact user experience*⚠️
   -⚠️*WPS Staff recommend that controllers be stored near headsets in operation, but hidden from public use as they are not needed for the proper functioning of the WildXR experience*⚠️

3. **USB cable & Quest 3 power brick**
   - All USB cables are USB-C to USB-C cables
   - All cables are reinforced with a static climbing rope and mesh sheath to provide some ruggedness to the cable connection
   - Cables for this deployment are for constant power supply
   - Cables include a short, USB-C male-to-female, stress relief cable that attaches to the Headset and then the longer cable
   - ⚠️*Cables can be a tripping hazard and should be managed for length and to ensure no slack lays on the floor of the display*⚠️
   - ⚠️*Power issues are generally caused by loose or unplugged cables, check all joints if a headset is experiencing power issues*⚠️
<div style="page-break-after: always;"></div>

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

8. **TV**
   - Brand and settings to be determined
   - Should turn on automatically with supplied power
   - Connected to microcomputer with HDMI cable
   - Connected to Kasa power strip and scheduled with on/off times to coincide with microcomputer
<div style="page-break-after: always;"></div>

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
<div style="page-break-after: always;"></div>

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
<div style="page-break-after: always;"></div>

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

## Important Notes

⚠️ **Default Values Warning**: Default values may prolong battery life but can introduce unexpected behavior in the WildXR application.

⚠️ **Developer Prerequisites**: If a Developer section is not visible under Advanced Settings, review the Guide for enabling Developer Settings on your headset.

⚠️ **Update Management**: Meta has instituted forced updates after 30-45 days of delay. Check headsets for pending updates every 21 days and contact WPS for guidance.

⚠️ **Developer Privileges Required**: Your Meta account must have developer access granted by WPS before advanced settings modifications will be available.