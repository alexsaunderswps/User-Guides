# Phoenix Zoo VR Setup

## Purpose & Context
This guide details the hardware and software associated with the Phoenix Zoo VR deployment of November 2025.

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR, PotPlayer, Windows) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

## Prerequisites
- None

## Quick Overview

### Hardware:
1. Quest 3 VR headsets managed by third-party software (3P) Meta-for-Work and ArborXR (includes 2 physical controller per headset)
2. Reinforced USB-C cables for power supply to headsets
3. Quest 3 VR headsets for backup purposes (one for each station)
4. MeLE microcomputers running PotPlayer for video playback
5. 65" TVs
6. Kasa smart power strips, power for all hardware
7. BLU WiFi connected smartphone for account access

### Software:

#### VR Headsets:
1. Autolaunchping.apk - Installed via ArborXR, automatically launches WildXR on headset power on
2. WildXR.apk - Installed via ArborXR, automatically launched by autolaunchping.apk
3. ArborXR suite - Installed via ArborXR to manage headset general settings

#### MeLE computers:
1. PotPlayer - Installed by WPS, runs video on loop on startup (added to startup folder)
2. MeshConnect Agent - Installed by WPS, used for remote management by WPS support staff
3. Windows Update Blocker (WUB) - Installed by WPS, used to prevent automatic Windows software updates which can impact user experience
4. AutoHideMouseCursor - Installed by WPS, used to automatically hide mouse cursor during video playback
<div style="page-break-after: always;"></div>

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
   - **USB C port** - On left temple. Allows both data transfer and power supply to headset. ⚠️*This port is a weak point on the headset and can be damaged if impacted or torqued*⚠️
   - **Headset Cameras** - Central camera manages depth perception, side cameras are a combination of color and IR, all for mixed reality experience (passthrough).
   - **Headset Sensors** - Two on lower "cheeks" of headset used for positioning in space (tracking use position), internal sensor between lenses used for detecting user presence (presence sensor).
   - **Double tap on headset case** - If not managed in settings could provide passthrough (ability to see surroundings) when in Quest main menu. Should not impact WildXR viewing or playback.
   - **Headset Fan** - Internal, top main dome of headset. Cools headset and occasionally can be heard in very quiet environs. If excessively noisy, or if headset is uncomfortable to touch, headset should be removed from operation.
<div style="page-break-after: always;"></div>

2. **Quest 3 VR Controllers**
   - *Details about the Quest 3 controllers is readily available online, WPS Staff recommends referencing the internet for images and detailed steps that may assist you in any problems you may encounter*
   - *All headset/controller groups are labeled with a 7-character s/n, this is the last 7 characters of the s/n provided by Meta and can be found on the headset left temple and inside the controller battery compartments*
   - *Controllers each have a **Trigger Button** (under index finger), **Grip Button** (under middle finger), a **Joystick** and three **Face Buttons**. Only specific uses will be covered as button function varies by application*
   - **Meta Button** - found on **Right Controller** is used to interrupt most applications and display resume or quit options along with screen capture and recording. 
      - *If you need to stop the WildXR application for any reason, this is the easiest, but may need to be combined with a sleep/wake cycle on the headset to interrupt the WildXR app*
   - ⚠️*WPS Staff recommends that controllers not be stored with batteries, both to prolong battery life, but also to prevent constant **Controller connection** alerts within the headset which will impact user experience*⚠️
   -⚠️*WPS Staff recommend that controllers be stored near headsets in operation, but hidden from public use as they are not needed for the proper functioning of the WildXR experience*⚠️

3. **Open the Settings Menu**
   - Click **"Settings"** in the top right of the Quick Settings Menu display
   - *A new floating window should appear, displaying headset Settings*
   - *Some options will not be visible until you scroll the left-hand list of setting categories*
   - *Joysticks on either controller will allow you to scroll when the aiming reticle is hovered over the list*

### General Settings

4. **Software Update Settings**
   - Click the **"Software Update"** tab
   - Toggle **off** all options:
     - `Software updates`
     - `Security and Critical updates`
     - `Automatically power headset to update`
     - `Update and backup before shutdown`

5. **Cloud Backup Settings**
   - Click the **"Cloud Backup"** tab
   - Toggle **off** `Cloud Backups`

6. **Power Settings**
   - Click the **"Power"** tab
   - Set **"Display Off"** to **4 hours**
   - Set **"Auto Sleep Headset"** to **4 hours** *(may not be present on all headsets)*
   - Toggle **off** all options under **"Battery"**:
     - `Battery Saver`
     - `Low battery audio alert`
     - `Low battery voice alert`

### Notification Settings

7. **Notification Settings**
   - Toggle **on** `Do Not Disturb`
   - Select **"Until I turn it off"** from the options that appear
   - Click **"Done"**
<div style="page-break-after: always;"></div>

### Environment Setup Settings

8. **Interactive Objects Settings**
   - Click the **"Interactive objects"** tab
   - Toggle **off** all options:
     - `Avatar Mirror`
     - `First Encounters`
     - `Portal to Meta Horizon World`

### Advanced Settings

9. **Developer Settings**
   - Toggle **on** `Enable Developer Settings`
   - Toggle **on** `Enable MTP Notification`
   - Toggle **off** `Physical Space Features`
   - Toggle **off** `Link Auto-Connect`

### Next Steps

10. **Create App PIN and lock apps**
    - Follow the **Library Management** guide

## Understanding Recommended Headset Settings

**Why These Settings:**
The recommended settings have been tested in public venues and provide the most consistent and longest lasting user experience to date.

**Software Update Settings:**
Turning off all automatic update settings prevents a headset from being unexpectedly unavailable during public hours. It also allows software updates to be tested in a controlled manner to prevent unanticipated conflicts between WildXR, Auto Launch, and headset software. Meta has instituted forced updates after 30 - 45 days of delay, allowing WPS a window to vet updates for performance and react, when possible, to software conflicts. We recommend checking headsets for pending updates every 21 days as routine maintenance and contacting WPS for guidance regarding installation.

**Cloud Backup Settings:**
There is no benefit to Cloud Backup in most end-user use cases where WildXR is used in a public or educational setting.

**Power Settings:**
Setting **"Display Off"** to **4 hours** allows headsets used in a public or educational setting to be immediately responsive to use. Having the display turn off will prolong battery life, but can cause the headset to be slow to respond to use and influence the orientation of scenes in WildXR in unexpected ways.

**Notification Settings:**
Notifications can cause disruption of user experiences by displaying pop-up windows within the WildXR application.
<div style="page-break-after: always;"></div>

**Interactive Objects Settings:**
A user may find themselves in the Quest main menu screen if there is an unexpected problem with the Auto Launch program or the WildXR application. Users familiar with VR headsets may force exit WildXR in certain situations to access the Quest main menu. By hiding interactive objects we can prevent some malicious or simple curious behavior from altering device settings.

**Developer Settings:**
Toggling off physical space features removes the need to define a boundary in the headset. Boundary setting can interfere with user experience by interrupting the WildXR display if a user moves outside the boundary. Boundaries are also required to be set up each time a headset is moved any distance and can cause unexpected behavior in some situations.
MTP Notifications allow the headset to be seen as a drive when connected to a computer via USB. This allows file transfer and manipulation, needed in some troubleshooting situations.

## Troubleshooting

**Developer section not visible under Advanced Settings:**
- Review the Guide for enabling Developer Settings on your headset
- Ensure your Meta account has developer privileges enabled by WPS
- Verify that developer mode is enabled in both the Meta Horizon phone app and headset settings

**Settings changes not persisting:**
- Ensure you complete each section fully before moving to the next
- Verify the headset is not in a restricted mode or parental controls
- Check that your account has administrative privileges on the device

**Cannot access certain settings options:**
- Confirm your Meta account has the necessary permissions
- Check if the headset is enrolled in an organization management system - managed systems prevent access to some settings
- Verify the headset software version supports all listed settings

**Power settings causing unexpected behavior:**
- Test different **"Display Off"** timing if 4 hours causes issues
- Monitor battery life with adjusted settings
- Ensure the headset remains responsive during peak usage hours
<div style="page-break-after: always;"></div>

## Important Notes

⚠️ **Default Values Warning**: Default values may prolong battery life but can introduce unexpected behavior in the WildXR application.

⚠️ **Developer Prerequisites**: If a Developer section is not visible under Advanced Settings, review the Guide for enabling Developer Settings on your headset.

⚠️ **Update Management**: Meta has instituted forced updates after 30-45 days of delay. Check headsets for pending updates every 21 days and contact WPS for guidance.

⚠️ **Developer Privileges Required**: Your Meta account must have developer access granted by WPS before advanced settings modifications will be available.