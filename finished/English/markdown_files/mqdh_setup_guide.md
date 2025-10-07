# Meta Quest Developer Hub Setup Guide

## Purpose & Context
This guide establishes the Meta Quest Developer Hub (MQDH) on your computer, which serves as the foundation for advanced VR headset management. MQDH enables you to install custom applications like WPS Auto Launch, manage developer settings, and perform advanced troubleshooting. This is a one-time setup process that creates the development environment needed for WildXR deployments.

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

## Prerequisites
- Windows or Mac computer with internet access
- Meta account credentials for your VR setup (including 2FA access)
- Administrative rights to install software on your computer
- Meta Quest headset with Developer mode enabled
- USB cable compatible with your Quest headset
- Headset and computer connected to the same WiFi network

## Quick Overview (for experienced users)
1. Download MQDH from Meta developers site and install
2. Launch MQDH and authenticate with Meta account
3. Complete initial setup and accept developer terms
4. Connect headset and establish USB debugging authorization
5. Verify full functionality with connected headset management

## Detailed Steps
*Only the Windows operating system will be covered in the following steps.*
*An Apple iOS version of MQDH is available following the link below*

### Downloading and Installing MQDH

1. **Navigate to Meta Developer Downloads**
   - Open web browser and go to Meta's developer site
   - **Windows**: Visit https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-win/
   - **Mac**: Visit https://developers.meta.com/horizon/downloads/package/oculus-developer-hub-mac/
<div style="page-break-after: always;"></div>

2. **Download MQDH package**
   - Click "Download" button in upper right corner
   - Accept license terms when prompted
   - Choose download location and click "Save"
   - File downloads as "Meta-Quest-Developer-Hub.zip"

3. **Extract and install MQDH**
   - Navigate to downloaded zip file location
   - Right-click "Meta-Quest-Developer-Hub.zip"
   - Select "Extract All" and choose destination (default location works well)
   - Click "Extract" to unpack files
   - Open extracted folder and locate "Meta-Quest-Developer-Hub.exe"
   - Double-click the executable to begin installation

4. **Complete installation process**
   - Follow installation wizard prompts
   - Accept default installation location unless specific requirements exist
   - When installation finishes, check "Run MQDH" checkbox
   - Click "Finish" to complete installation and launch application

### Initial MQDH Authentication

5. **Begin MQDH setup**
   - Application opens to welcome screen
   - Click "Continue" in bottom right corner
   - Select "Log in with a Meta account" option
   - System opens browser window for authentication

6. **Authenticate with Meta account**
   - Browser redirects to Meta login page
   - Choose "Continue with email" option
   - Enter Email address associated with your VR setup *(may be provided by WPS)*
   - Click "Next" to proceed

7. **Complete password authentication**
   - Select "Enter password instead" *(easier than email code)*
   - Enter your Meta account password *(may be provided by WPS)*
   - Click "Log in" to authenticate
<div style="page-break-after: always;"></div>

8. **Handle 2FA verification**
   - System presents 2FA method dropdown
   - Select method specified by WPS staff
   - Click "Next" to proceed
   - Enter 6-digit authentication code when prompted
   - Click "Next" to complete 2FA verification

9. **Manage login persistence (optional)**
   - Choose whether to save login credentials on this computer
   - *Saving credentials only stores email and password information*
   - *2FA verification will still be required for future login sessions*
   - *Consider security implications of saved credentials on shared computers*

### Completing MQDH Setup

10. **Accept developer terms**
    - MQDH displays Terms and Documents screen
    - Review developer agreement terms
    - Click "Continue" to accept and proceed

11. **Handle ADB path warning (if appears)**
    - System may display warning about multiple ADB paths
    - This warning is typically safe to dismiss
    - Click "Cancel" or close warning without modifying ADB settings
    - MQDH will use appropriate defaults for your system

12. **Verify successful installation**
    - MQDH main interface should now be visible
    - Left sidebar shows device management icons
    - Upper toolbar displays account information
    - Application is ready for headset connections and app management

### Connecting Your Headset and Establishing USB Debugging

13. **Establish physical connection**
    - Power on your VR headset completely
    - Connect USB cable between headset and computer running MQDH
    - Ensure cable connection is secure at both ends
    - Headset should remain powered throughout the connection process
<div style="page-break-after: always;"></div>

14. **Check for automatic device recognition**
    - In MQDH, click the headset icon in the left sidebar
    - Look for your device listed as "Active" in the Devices section
    - If device appears as Active, proceed directly to step 18 for USB debugging
    - If device is not shown or shows as inactive, continue with device setup

15. **Initiate new device setup (if needed)**
    - Click dropdown menu in upper right corner of MQDH
    - Select "Set Up New Device" from menu options
    - You may need to scroll down to locate this option
    - Click "Next" to begin device configuration wizard

16. **Configure device connection**
    - Select your specific headset model from available options
    - MQDH will scan for compatible devices on your network
    - Choose your headset from "Choose Device" list when it appears
    - Click "Next" to proceed with account verification

17. **Complete device setup**
    - Confirm correct Meta account is displayed on Account page
    - Click "Next" to proceed to network configuration
    - Select appropriate WiFi network for your deployment environment
    - Click "Next" to continue with developer mode verification
    - Toggle "Enable Developer Mode" switch if not already active
    - Click "Next" to complete initial device setup

18. **Authorize USB debugging access**
    - Put on the VR headset to view system prompts
    - Look for "Allow USB debugging?" dialog box
    - This dialog authorizes your computer to install applications and access system functions
    - You may need to look around the virtual environment to locate the dialog

19. **Grant permanent debugging permissions**
    - Click "Always allow from this computer" button in the dialog
    - This button may be partially obscured at the bottom of the dialog window
    - The "Always allow" option prevents repeated authorization requests
    - Remove headset after confirming the authorization

20. **Complete setup verification**
    - Return to MQDH on your computer
    - Click "Finish" if device setup wizard is still open
    - Your headset should now appear as "Active" in the devices list
    - USB debugging is now permanently authorized for this computer-headset pair
<div style="page-break-after: always;"></div>

## Understanding Developer Hub Components

**Why MQDH is Essential:**
Meta Quest Developer Hub serves as the bridge between your computer and VR headsets for advanced management tasks. While basic headset operation works through the standard Meta app, MQDH unlocks developer capabilities that are essential for custom application deployment like WPS Auto Launch. Think of it as the difference between using a smartphone as a consumer versus having developer access to install custom apps and modify system behavior.

**ADB Integration:**
MQDH integrates with Android Debug Bridge (ADB), which is the underlying communication protocol for managing Android-based devices. Meta Quest headsets run on a modified Android system, so ADB provides the technical foundation for installing custom applications, accessing system settings, and performing advanced troubleshooting. The ADB warning you might see during setup relates to ensuring MQDH uses the correct communication pathways.

**Account Requirements:**
Your Meta account must have developer privileges enabled by WPS before MQDH will function properly. This isn't something you can enable yourself - it requires coordination with WPS staff who manage the developer organization settings. This security measure ensures that only authorized personnel can install custom applications on WildXR deployment headsets.

## Troubleshooting

**Download fails or is corrupted:**
- Verify stable internet connection throughout download
- Try downloading from different browser or incognito mode
- Check available disk space before downloading
- Contact WPS if download consistently fails

**Installation process stops or fails:**
- Ensure administrative privileges on computer
- Temporarily disable antivirus during installation
- Verify system meets minimum requirements
- Restart computer and retry installation

**Authentication fails repeatedly:**
- Verify Gmail address matches VR setup account
- Confirm password accuracy with WPS staff
- Check that account has developer privileges enabled
- Ensure 2FA codes are current (30-second expiration)
<div style="page-break-after: always;"></div>

**MQDH won't launch after installation:**
- Check Windows Defender or antivirus quarantine
- Verify installation completed successfully
- Try running as administrator
- Restart computer and retry launch

**Headset not recognized by MQDH:**
- Verify both computer and headset are connected to the same WiFi network
- Confirm your Meta account has developer privileges through WPS
- Check that developer mode is enabled in both the Oculus phone app and headset Settings > Advanced > Developer
- Ensure no pending headset updates exist under Settings > General > Software Update

**USB debugging authorization not appearing:**
- Verify USB cable connections are secure at both ends
- Check for pending headset updates that might prevent authorization
- Look for pending MQDH updates indicated by banner across application top
- Try disconnecting and reconnecting USB cable after 30 seconds
- Power cycle the headset completely and retry connection

**Device appears connected but shows as inactive:**
- Confirm USB debugging was properly authorized with "Always allow" option
- Verify Meta account consistency between MQDH and headset
- Check that developer mode remains enabled in headset settings
- Try removing and re-adding the device through MQDH setup wizard

## Important Notes

⚠️ **Developer Privileges Required**: Your Meta account must have developer access granted by WPS before MQDH will function properly for custom app installation.

⚠️ **Account Consistency**: The Meta account used in MQDH must exactly match the account associated with your VR headsets. Mixed accounts will prevent proper device recognition.

⚠️ **Headset Linking**: MQDH requires headsets to be ADB to be enabled for some funcitonality. If functionality is missing this may be the issue.

⚠️ **Software Updates**: MQDH is in a constant state of development and as such will often require an update. If possible, always update MQDH when prompted prior to completing other tasks in MQDH.
<div style="page-break-after: always;"></div>

## Verification Steps

Verify that your MQDH application is capable of recognizing, connecting to, and managing VR headsets without additional configuration steps.

**Complete functionality verification:**
- MQDH launches without errors and displays account information correctly
- At least one headset appears as "Active" in the devices list
- USB debugging authorization has been granted and confirmed
- Device management icons are accessible and responsive in the left sidebar
- You can access the headset's file system and application management features