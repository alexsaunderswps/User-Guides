# Quest VR Headset Recommended Settings

## Purpose & Context
This guide details recommended settings for Quest 2, Quest 3, and Quest 3s, to make the WildXR VR experience consistent and reliable.

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

## Prerequisites
- Quest headset and controllers with batteries

## Quick Overview (for experienced users)
1. Enter the **Settings** menu
2. Change power settings to match desired use case
3. Enable:
    - **Do Not Disturb**
    - **Developer Mode**
    - **Enable MTP connection**
4. Disable:
    - **Cloud Backup**
    - **Automatic Updates**
    - **Interactive Elements**

## Detailed Steps

### Accessing the Settings Menu

1. **Quit the WildXR Application (if running)**
   - Press the **Meta-logo button** (Quest 3 and Quest 3s) or the **Horizontal Oval button** (Quest 2) on the right hand controller
   - Select **"Quit"** on the App management window that appears
   - If the App management window does not appear:
     - Press the **headset power button** to sleep the headset
     - Press the **headset power button** again to wake the headset
     - Press the **Meta-logo button** on the right hand controller
     - Select **"Quit"** on the App management window
<div style="page-break-after: always;"></div>

2. **Open the Quick Settings Menu**
   - Click the **button that displays time, WiFi strength, and battery level** on the left Menu Bar
   - *A new floating window should appear, displaying Quick Menu Settings*

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