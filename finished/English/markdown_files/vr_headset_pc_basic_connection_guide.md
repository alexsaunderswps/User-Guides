# VR Headset Basic Connection Guide

## Purpose & Context
This guide establishes the foundation for all VR headset file management tasks. You'll connect your Meta Quest 2, Quest 3, or Quest 3s to a computer and access the WildXR application files. This connection is required before transferring media files, confirming configuration or localConfiguration files, or troubleshooting application issues.

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

## Prerequisites
- Meta Quest 2, Quest 3, or Quest 3s VR headset
- USB-C cable *(recommended)* or USB-C to USB-A cable
- Computer with File Explorer *(Windows)* or Finder *(Mac)*
- AA batteries for controllers
- WildXR application installed on headset
- Developer settings enabled on the headset

## Quick Overview (for experienced users)
1. Power on headset and ensure controllers have batteries
2. Connect USB cable and quit WildXR if running
3. Enable USB connection through Quest notifications
4. Navigate to: `Quest` > `Internal shared storage` > `Android` > `data` > `com.wps.wildx` > `files`

## Detailed Steps

### Initial Setup

1. **Install controller batteries**
   - Both Quest 2 and Quest 3 use **AA batteries**
   - Ensure both controllers are powered

2. **Power on your headset**
   - **Quest 2**: Press **power button** on right side
   - **Quest 3 & Quest 3s**: Press **power button** on left side
<div style="page-break-after: always;"></div>

3. **Connect USB cable**
   - **Quest 2**: USB port located on left side below temple
   - **Quest 3 & Quest 3s**: USB port located on left side on temple

4. **Identify primary controller**
   - **Quest 2**: Right controller has **horizontal oval button**
   - **Quest 3 & Quest 3s**: Right controller has **Meta logo button**

### Exiting WildXR Application

*If WildXR launches automatically, you must exit it to access files.*

5. **Attempt to open system menu**
   - Put on headset
   - Press and release the **oval/Meta button** on right controller
   - If **Quit/Resume** screen appears, skip to step 8

6. **Force menu appearance (if needed)**
   - Press **power button** to sleep headset *(screen goes dark)*
   - Press **power button** again to wake headset
   - Try **oval/Meta button** again
   - Repeat until **Quit/Resume** screen appears

7. **Exit WildXR**
   - Select **"Quit"** using controller trigger
   - *You should see the Quest home environment*

### Enabling Computer Access

8. **Open notifications**
   - Aim targeting dot at **bell icon** on menu bar
   - Press **controller trigger** *(under pointer finger)* to open notifications

9. **Enable USB connection**
   - *You will need to have enabled developer settings on the headset*
   - Find **"USB Detected"** notification
   - Aim at notification and press **controller trigger**
   - *This allows computer to recognize headset as external drive*

### Accessing Files on Computer

10. **Open file browser**
    - **Windows**: Open **File Explorer**, click **"This PC"**
    - **Mac**: Open **Finder**
<div style="page-break-after: always;"></div>

11. **Navigate to headset**
    - Double-click **"Quest 2"**, **"Quest 3"**, or **Quest 3s**
    - Double-click **"Internal shared storage"**

12. **Navigate to WildXR files**
    - Double-click **"Android"**
    - Double-click **"data"**
    - Double-click **"com.wps.wildx"**
    - Double-click **"files"**

*You now have access to WildXR files and folders.*
## Understanding WildXR files and folders

**downloads folder**
- Holds all downloaded videos for the WildXR application
- Files named using universally unique 36-character id (UUID)
- All in MP4 format
- *This folder is where **sideloaded** video files will be placed*

**textures folder**
- Holds all downloaded thumbnail images for the WildXR application
- Files named with UUID that matches video UUID
- All in PNG format

**temp folder**
- Holds temporary files needed by the WildXR application
- Often will hold video files that are being downloaded by the WildXR application

**Unity folder**
- WildXR Unity files
- No access needed by most users

**localConfiguration.json file**
- Configuration settings that are device (headset) specific
- Contains Device ID, Environment, and OfflineMode settings

**configuration.json file**
- Configuration settings that control the appearance of the WildXR application
- If headset or computer (device) is registered through WildXR Web Portal these settings are controlled remotely
- If headset or computer (device) is not registered through WildXR Web Portal these settings are preconfigured by the WildXR application
<div style="page-break-after: always;"></div>

**metadataDatabase.json**
- Metadata required by the WildXR application for proper functioning

**DownloadQueue.json**
- Information for video download function in the WildXR application
- May be empty or absent if no videos are queued for download

**Player.log and Player-prev.log**
- Log files recording the most recent and previous behavior of WildXR application
- Important for diagnosing issues and may be requested by WPS staff for diagnosis

**youtubeData.json**
- Data used to sort videos in thumbnail galleries based on various factors

## Troubleshooting

**Headset not appearing in file browser:**
- Ensure USB cable is fully connected
- Try a different USB port on computer
- Check that you enabled USB connection in step 9
- Verify the USB cable supports data transfer, not just charging

**Can't exit WildXR:**
- Remove headset briefly, then put back on
- Cycle headset *Press power button to sleep headset and then press again to wake*
- Ensure controllers have sufficient battery power

**Controllers not responding:**
- Check battery installation direction
- Try fresh AA batteries
- Ensure controllers are paired *(should happen automatically when headset starts)*
- Power cycle controllers by removing and reinserting batteries

**USB connection notification not appearing:**
- Disconnect and reconnect USB cable
- Try different USB port on computer
- Ensure headset is fully powered on and not in sleep mode
- Check if developer mode is enabled in headset settings
- *You must accept the USB connection notification each time the USB is connected*
<div style="page-break-after: always;"></div>

**Files/folders appear empty or inaccessible:**
- Verify WildXR has been run at least once on the headset
- Check that the correct path is being followed: `Android` > `data` > `com.wps.wildx` > `files`
- Ensure USB debugging permissions were granted if prompted
- Try refreshing the file browser view

## Important Notes

⚠️ **File Editing Restriction**: Files like `configuration.json` cannot be edited directly on the headset. You must:
1. Copy files to your computer
2. Edit them there
3. Copy the modified files back to overwrite originals
4. Files can be opened to verify changes have been applied *(see **File Transfer Verification** below)*

⚠️ **Backup Recommendation**: Always create a backup copy of configuration files before editing.

⚠️ **File Editing Verification**: Always check that edited files have been transferred successfully to the headset.

⚠️ **File Transfer Recommendation**: When sideloading video files, verify the **downloads** folder contains the number of videos you attempted to sideload.

⚠️ **Cable Requirements**: Ensure your USB cable supports data transfer. Some cables are charge-only and will not allow file access.

⚠️ **WildXR Prerequisites**: WildXR must be installed and run at least once before files will be accessible in the expected directory structure.
