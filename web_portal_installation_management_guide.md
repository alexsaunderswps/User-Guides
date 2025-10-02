# WildXr Web Portal Installation Management Guide

## Purpose & Context
This guide introduces the management of installations (the experience presented to headset users) running the WildXR VR application via the WildXR Web Portal (Wildxr.org)

⚠️ **Video Download Time**: Whenever a new instance or update of WildXR is required all associated videos must be downloaded to provide a smooth playback experience. Depending on the video library size and internet speeds, this can take multiple hours. Please consider this when scheduling an update or planning for new WildXR installations.

## Prerequisites
- Windows or Mac computer with internet access
- An internet browser (WPS recommends Chrome)
- A WildXR account with credentials *(may have been created by WPS staff)*
- A **"Device"** - either a VR headset (Quest 2, Quest 3, or Quest 3s) or Computer - with the WildXR application installed

## Quick Overview (for experienced users)
1. Navigate to the Wildxr.org website
2. Log In with your Username and Password *(may be provided by WPS staff)*
3. Navigate to the Admin -> Installations page
4. Edit an exisitng or Add a new Installation
5. Verify the Installation settings
6. Plan for video file downloads as necessary for Installation use

## Detailed Steps

### Access Installation management page on Wildxr.org

1. **Navigate to WildXR web portal**
   - Open web browser and go to WildXR web portal
   - Visit https://wildxr.org

2. **Log In to WildXR web portal**
   - Enter your Username in the appropriate field
   - Enter your Password in the appropriate field
   - Click **"Log In"**
<div style="page-break-after: always;"></div>

3. **Navigate to the Installation management page**
   - In the top navigation bar, click **"Admin"**
   - In the dropdown menu that appears click **"Installations"**
   - *If you are an Organization Admin you will only see installations assocaited with your organization*
   - *If you are a System Admin you will see all installations across all organizations*
   - To **"Add"** a new installation continue to Step 4
   - To **"Edit"** an exisiting installation, continue to Step 10

### Add a New Installation

4. **Begin new installation creation**
   - On the **Installations** page, click **"Add"** in the top right

5. **Name, Organization, Tips**
   - In the **"Name"** field, enter the installation name - *This name is not exposed to the user and is solely for organizational purposes*
   - *WPS recommends a naming structure that identifies your organization, lists the location/function of the installation (if appropriate), and internal organizational information*
   - *For example **BP - Conservation Hallway - Download Only** shows that the installation is for the **Butterfly Pavilion**, to be used in their **Conservation Hallway**, and is specifically for **Downloading** the videos needed for the installation* 
   - Choose the **"Organization"** with which this installation is associated
   - *Only **System Admins** can choose an organization, **Organization Admins** will have this field pre-populated with their specific organization
   - Enter tips into the **"Tips"** field. 
   - Each tip should be separated onto separate lines as shown by the pre-populated tips.
   - *Tips are shown to users while videos load - if you are only playing a single video on a loop tips are unneccessary*

### Tutorial modes

6. **Select the appropriate Tutorial mode**
   - There are four options for **Tutorials** in the WildXR application:
      1. **None** - used when no tutorials are desired or if playing a single video on a loop
      2. **Text** - A text window pop-up displays when a new user is detected in the headset. It briefly describes how to navigate the WildXR application and is closed by the user selecting a **"Close"** button
      3. **Video** - A brief video with narration is played to show a new user how to navigate the WildXR application.
      4. **Dynamic** - If a user does not interact with the WildXR interface for a period of time the **Video** tutorial is played. The tutorial stops as soon as the user interacts with any WildXR elements.
   - **Tutorials** should not be used when playing a single video on a loop otherwise they may interfer with video playback - please select **None** in this situation

### Timer settings

- *Timer settings are only available to **System Admins** as they can influence how the WildXR application interacts with users*

- *If you think your installation would benefit from a specific timer setting, please contact WPS staff for assistance*

7. **App Timer Length, Idle Timer Length, Idle Timer Delay**
   - **App Timer Length Seconds** controlls how long a new user can use the WildXR application before a grey wash overlays the interface. 
   - *This setting is considered a **Beta** feature and may not behave reliably in all situations*
   - **Idle Timer Length Seconds** acts as a backup to the headset **Presence Sensor** as presence detection can be unreliable with various Meta firmware versions
   - **Idle Timer Length** is the amount of time after which a lack of movement within the headset triggers a **Presence Sensor** event within the WildXR application
   - *This setting was primarily used to trigger **Spectator Camera** events on connected systems, but may also be helpful in gathering **Analytic** data*
   - **Idle Timer Delay Seconds** is the delay between the time a headset detects new motion to the time at which it resets the headset view
   - **Idle Timer Delay** reduces the chance that a headset will show a non-standard view when mounted (put on by a user) after having been stored on a hook
   - *This delay is difficult to predict without some experience and should be custom set for each **Installation** if **Idle Timer Length** is being used*

### Globe Starting position 

8. **Globe Start Latitude and Longitude**
   - Determines where on the globe a gaze reticle will be positioned for new users
   - Not used when a single video is played on loop
   - If multiple **Map Markers** are used in a **Video Catalogue**, WPS recommends positioning the gaze reticle close to at least one marker
   - *WPS recommends using Google maps to find a position that works best for your installation*
   - *WPS recommends not positioning your **Globe Start Lat. and Long.** too close to a **Map Marker**, as the associated gallery may open before the user realizes they can navigate the globe* 
   - Lat. and Long. co-ordinates can include decimal digits, but cannot be 0 and 0
<div style="page-break-after: always;"></div>

8. **Enter an installation (Optional)**
   - If you have an **Installation** already created for the device select the **Installation** from the dropdown menu
   - If you do not have a **Installation** ready for this device, leave **Installation** blank and the default **Installation** will be applied
   - *If apply an **Installation** with **Demo Mode** enabled, remember that this removes the ability to manually download videos via the WildXR application*

9. **Save the Device Details**
   - Verify that all **Device Details** are correct
   - Click the **"Save"** button

### Edit an Exisiting Device

10. **Open an exisiting device**
    - Scroll through the devices displayed or navigate to additional pages via the buttons in the lower right
    - *Alternatively you can search for the Device name using the **Search** field in the upper left*
    - Click anywhere on the device row when you have identified the device you wish to edit

11. **Edit the device details**
    - Select the fields in need of updating
    - Verify all changes are correct
    - *If you are a **System Admin** verify that you are assigning the device to the correct organization*
    - Click **"Save"** to save the device details update

### Apply Installation changes to a device

12. **Restart the WildXR App**
    - Changes to a device's assigned **Installation** will not take affect until the WildXR app is restarted on the device
    - *Devices will need to be connected to the internet to accept an **Installation** assignment*

## Troubleshooting

**Unable to log onto the Wildxr.org website:**
- Ensure you are entering the correct credentials to log into Wildxr.org *(May have been supplied by WPS Staff)*
- If someone within your organization created your account; check that they assigned a password to your account *(passwords are not created automatically)*
- Double-check the URL you have entered into your Web Browser *(WPS recommends using Chrome)*
<div style="page-break-after: always;"></div>

**Unable to generate a WildXR number:**
- Ensure that the WildXR application has been successfully installed on the device
- If you are attempting to launch WildXR on a computer you will need to connect a VR headset to successfully navigate the WildXR app
- Verify that you can see the **gear icon** used to access the **"Settings Menu"** 

**Unable to find WildXR number on the Wildxr.org website:**
- Ensure you have correctly typed the WildXR number into the Device Lookup field on the Wildxr.org website
- If you are currently on the **Devices** page of the Wildxr.org website, navigate away and then back before attempting the Device Lookup
- Refresh your browser window *(WPS recommends using Chrome)*

**WildXR number is already generated for a device:**
- Double check that the device has not already been registered on the WildXR.org website
- If you are re-installing WildXR on a computer, you will need to remove the **Wildlife Protection Solutions** folder from your hard drive
  - *Ensure that **Hidden Items** are visible in your **File Explorer***
  - Open a folder and, under **View** options click **"Show"** and check **"Hidden Items"**
  - On Windows navigate to ```This PC -> C -> Users -> [Your User Name] -> App Data -> Local Low```
  - Delete the **Wildlife Protection Solutions** folder
  - Reinstall the **WildXR** application

**Applied changes to Device not visible in Device**
- Ensure that your device is connected to the internet
- If you have assigned a new **Installation** the device must stop the current session of WildXR and relaunch the WildXR app prior to changes taking effect
- Double check that the Wildxr Number is the one assigned to the headset you are using *(Check the settings menu to confirm the Wildxr number)*

**Unable to edit Device Organization**
- If you are logged into the Wildxr.org website as an **Organization Admin** will not be able to change the device's assigned organization
- Log in as a **System Admin** to enable organization assignment or contact WPS Staff
<div style="page-break-after: always;"></div>

## Important Notes

⚠️ **Developer Privileges Required**: Your Meta account must have developer access granted by WPS before MQDH will function properly for custom app installation.

⚠️ **Account Consistency**: The Meta account used in MQDH must exactly match the account associated with your VR headsets. Mixed accounts will prevent proper device recognition.

⚠️ **Security Coordination**: Never modify developer settings or install unauthorized applications without WPS approval. This can compromise headset security and void support agreements.

⚠️ **System Requirements**: MQDH requires modern computer specifications and may not work properly on older or resource-limited systems.

## Verification Steps

Verify that your MQDH application is capable of recognizing, connecting to, and managing VR headsets without additional configuration steps.

**Complete functionality verification:**
- MQDH launches without errors and displays account information correctly
- At least one headset appears as "Active" in the devices list
- USB debugging authorization has been granted and confirmed
- Device management icons are accessible and responsive in the left sidebar
- You can access the headset's file system and application management features