# WildXr Web Portal Installation Management Guide

## Purpose & Context
This guide introduces the management of installations (the experience presented to headset users) running the WildXR VR application via the WildXR Web Portal (Wildxr.org).

⚠️ **Video Download Time**: Whenever a new instance or update of WildXR is required all associated videos must be downloaded to provide a smooth playback experience. Depending on the video library size and internet speeds, this can take multiple hours. Please consider this when scheduling an update or planning for new WildXR installations.

⚠️ **Installations** act as the source of truth for how the WildXR application behaves when online. If changes are made via the user interface, and not by updating the **Installation** assigned to a headset, those changes may be overwritten when the headset connects to the internet. Always update an **Installation** if changes to the WildXR application behavior is

## Prerequisites
- Windows or Mac computer with internet access
- An internet browser (WPS recommends Chrome)
- A WildXR account with credentials *(may have been created by WPS staff)*
- A **"Device"** - either a VR headset (Quest 2, Quest 3, or Quest 3s) or Computer - with the WildXR application installed

## Quick Overview (for experienced users)
1. Navigate to the Wildxr.org website
2. Log In with your Username and Password *(may be provided by WPS staff)*
3. Navigate to the Admin -> Installations page
4. Edit an existing or Add a new Installation
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
   - *If you are an Organization Admin you will only see installations associated with your organization*
   - *If you are a System Admin you will see all installations across all organizations*
   - To **"Add"** a new installation continue to Step 4
   - To **"Edit"** an existing installation, continue to Step 19

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
   - *Tips are shown to users while videos load - if you are only playing a single video on a loop tips are unnecessary*

### Tutorial modes

6. **Select the appropriate Tutorial mode**
   - There are four options for **Tutorials** in the WildXR application:
      1. **None** - used when no tutorials are desired or if playing a single video on a loop
      2. **Text** - A text window pop-up displays when a new user is detected in the headset. It briefly describes how to navigate the WildXR application and is closed by the user selecting a **"Close"** button
      3. **Video** - A brief video with narration is played to show a new user how to navigate the WildXR application.
      4. **Dynamic** - If a user does not interact with the WildXR interface for a period of time the **Video** tutorial is played. The tutorial stops as soon as the user interacts with any WildXR elements.
   - **Tutorials** should not be used when playing a single video on a loop otherwise they may interfere with video playback - please select **None** in this situation
<div style="page-break-after: always;"></div>

### Timer settings

- *Timer settings are only available to **System Admins** as they can influence how the WildXR application interacts with users*

- *If you think your installation would benefit from a specific timer setting, please contact WPS staff for assistance*

7. **App Timer Length, Idle Timer Length, Idle Timer Delay**
   - **App Timer Length Seconds** controls how long a new user can use the WildXR application before a grey wash overlays the interface. 
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

### Video Catalogue settings

9. **Select Video Catalogue**
   - A **Video Catalogue** is a collection of videos that can be used for various **Installations**
   - Use the **"Web Portal Video Catalogue Creation Guide"** to create or edit a **Video Catalogue** and for more information about using catalogues for specific purposes
   - If you are logged in as an **Organization Admin**, only catalogues associated with your **Organization** or those created by **WildXR** staff are available
   - **System Admin** have access to all catalogues
   - Select the catalogue to be used for your **Installation**
<div style="page-break-after: always;"></div>

10. **Show adult content**
    - Check the **"Show Graphic Death"** to expose videos that show adult content involving death or gore
    - Check the **"Show Graphic Sex"** to expose videos that show adult content involving reproductive behavior
    - If these boxes are left unchecked, videos that show this content will not be visible within the WildXR application
    - ⚠️ Regardless of whether these checkboxes are selected or not, it is possible to select a video as an **Installation** startup video that contains adult content.
    - ⚠️ Review video selection to ensure content is appropriate for your intended audiences. 

### WildXR application startup behavior

11. **Select Startup Video, Loop Video, Resume Video**
    - Select a **"Startup Video"** to play when WildXR launches.
    - **Startup Videos** must be part of the currently selected **Video Catalogue**
    - Select the **"Startup Video Loop"** checkbox if you want the startup video to play continuously in the headset - this will be the only video that plays
    - If the **Startup Video** is a video introduction to an **Installation** and you want it to play once for each user, leave the **"Startup Video Loop"** box unchecked
    - If you want users to choose their own video from the **Video Catalogue** leave the **"Select Startup Video"** field blank
    - Checking the **"Resume Startup Video on Awake"** box with cause the video to continue playing when a new user picks up the headset instead of starting from the beginning

### Favorites

12. **Select Favorites, Filter Favorites by Default**
    - The **"Select Favorites"** field is multi-select and allows the selection of videos from the current **"Video Catalogue"**
    - Click the field to expose a drop-down menu of videos, or begin typing to have videos suggested based on title.
    - To remove videos from the **Favorites** list, click the **x** button in their title display.
    - Select the **"Filter Favorites By Default"** checkbox to have thumbnail galleries display **Favorites** instead of all videos represented by a **Map Marker**
    - *Users can switch to seeing all videos, instead of only favorites, by selecting the **All** button at the top of a thumbnail gallery*
<div style="page-break-after: always;"></div>

### Set videos to download automatically

13. **Automatic Download Mode**
    - ⚠️ Automatic video download is affected by current internet connection strength and speed
    - ⚠️ A weak or intermittent internet connection can cause playback issues in videos (distorted audio or clipped video playback)
    - ⚠️ Downloading videos while a video streams (or plays locally) can impact video playback quality
    - ⚠️ WPS recommends that all videos be allowed to download completely prior to using headsets in a public setting.
    - There are four options to choose from under WildXR's **"Automatic Download Mode"**:
      1. **Download Nothing** - No videos are automatically downloaded when WildXR launches
      2. **Download Startup Video** - The currently selected **Startup Video** is automatically downloaded when WildXR launches
      3. **Download Favorites** - All videos selected as **Favorites** are downloaded when WildXR launches
      4. **Download Entire Catalogue** - All videos in the currently selected **Video Catalogue** are downloaded when WildXR launches
    - ⚠️ Sideloading a headset with videos (transferring video files via a USB connection) is recommended for large videos and large video catalogues

### Control, Demo Mode, Menu Tray, and Session Data

14. **Select Control**
    - By default, users interact with the WildXR user interface with **Gaze** control - controlling a selection reticle with head movement
    - Select **Hand Controllers** to allow users to use the physical controllers, modeled as hands, to interact with the WildXR user interface
    - ⚠️ The **Hand Controllers** option is still in development and may cause unexpected behavior in the app and is not recommended for public use
    - ⚠️ Giving the public access to the physical controllers associated with VR headsets allows them to exit WildXR and gain access to the general VR interface which is generally undesirable
<div style="page-break-after: always;"></div>

15. **Demo Mode**
    - ⚠️ **Demo Mode** is recommended for most public deployments of WildXR ⚠️
    - When **Demo Mode** is selected it has the following effects on the WildXR user interface:
      1. Addition/Removal of videos from the **Favorites** category is disabled
      2. Addition/Deletion of videos from the **Downloaded** library is disabled
      3. WildXR will return to the **Globe Scene** after a period of inactivity if no **Startup Video** is selected
      4. The **Download Queue** is hidden from the WildXR user interface 
      5. The **Admin Panel** access button is hidden
      6. With **Demo Mode** disabled the **Admin Panel** is shown beside the **Menu Tray** (if the Menu Tray is visible) and gives access to:
         1. Showing/Hiding the **Video Streaming** warning
         2. Showing/Hiding Adult content (videos that show graphic scenes of death, gore, or reproductive behavior)
         3. Starting galleries in the **Favorites** instead of the **All** videos view
         4. Switch between **Gaze** and **Hand Controller** options
         5. ⚠️ Enable **Voice Control** - an experimental feature

16. **Show Menu Tray**
    - The WildXR **Menu Tray** sits beneath the navigation globe and thumbnail galleries giving access to the **All Clips** and **Short Films** galleries
    - **All Clips** is a single gallery view that shows all videos available in the **Video Catalogue** associated with the **Installation**
    - **Short Films** is a gallery that displays videos tagged with either the **Compilation** or the **Short Films** tag

17. **Send Session Data**
    - ⚠️ This feature is in development
    - When selected **Send Session Data** will send information about how users are interacting with the WildXR application and the videos shown in the assigned **Installation**

18. **Save new installation**
    - Click the **"Save"** button to save your new installation and allow its assignment to registered devices
    - Click the **"Cancel"** button to discard your installation and return to the **Installations** page
<div style="page-break-after: always;"></div>

## Edit an existing installation
- *Organization users can only edit installations that their organization owns*
- *If you have concerns about an existing installation that your organization does not own, please reach out to WPS Staff for assistance*
- ⚠️ Updates to an **Installation** are not applied to registered **Devices** until that device is connected to the internet and WildXR is stopped and relaunched

### Access the Installations page on Wildxr.org

19. **Navigate to WildXR web portal**
   - Open web browser and go to WildXR web portal
   - Visit https://wildxr.org

20. **Log In to WildXR web portal**
   - Enter your Username in the appropriate field
   - Enter your Password in the appropriate field
   - Click **"Log In"**

21. **Navigate to the Installations page**
   - In the top navigation bar, click **"Admin"**
   - In the dropdown menu that appears click **"Installations"**
   - *If you are an Organization Admin you will only see installations associated with your organization*
   - *If you are a System Admin you will see all installations across all organizations*

### Search for the installation that needs editing

22. **Locate the installation to edit**
    - Enter all or part of the **Installation** name in the **"Filter by name"** field in the upper left
    - Click the **"Search"** button to filter the visible **Installations**
    - Click on the **Installation** that needs editing to open the editing view

23. **Edit installation and save**
    - Edit the fields as necessary to update the **Installation**
    - Updating the **Video Catalogue** will change which videos are available for **Startup Video** and **Favorites**
    - Updating the **Automatic Download Mode** will not remove any previously downloaded videos, but will stop any downloads in progress when the WildXR application is relaunched
    - Click the **"Save"** button to save updates
    - Click the **"Cancel"** button to discard updates
<div style="page-break-after: always;"></div>

### Applying your installation to devices

24. **Assign installation to registered devices**
    - **Installations** must be assigned to registered **Devices** before they can be seen in the WildXR application
    - Follow the steps in the **Web Portal Device Management Guide** for more information on assigning **Installations** to **Devices**

## Troubleshooting

**Unable to log onto the Wildxr.org website:**
- Ensure you are entering the correct credentials to log into Wildxr.org *(May have been supplied by WPS Staff)*
- If someone within your organization created your account; check that they assigned a password to your account *(passwords are not created automatically)*
- Double-check the URL you have entered into your Web Browser *(WPS recommends using Chrome)*

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