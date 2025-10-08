# WildXR Web Portal Installation Management Guide

## Purpose & Context
This guide introduces the management of installations (the experience presented to headset users) running the WildXR VR application via the WildXR Web Portal (Wildxr.org).

⚠️ **Video Download Time:** Whenever a new instance or update of WildXR is required all associated videos must be downloaded to provide a smooth playback experience. Depending on the video library size and internet speeds, this can take multiple hours. Please consider this when scheduling an update or planning for new WildXR installations.

⚠️ **Installations:** Installations are settings that determine what and how content is shown inside an instance of the WildXR application. If changes are made via the user interface, and not by updating the **Installation** assigned to a headset, those changes may be overwritten when the headset connects to the internet. 

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
<div style="page-break-after: always;"></div>

2. **Log In to WildXR web portal**
   - Enter your Username in the appropriate field
   - Enter your Password in the appropriate field
   - Click **"Log In"**

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
<div style="page-break-after: always;"></div>

### Tutorial modes

6. **Select the appropriate Tutorial mode**
   - There are four options for **Tutorials** in the WildXR application:
      1. **None** - used when no tutorials are desired or if playing a single video on a loop
      2. **Text** - A text window pop-up displays when a new user is detected in the headset. It briefly describes how to navigate the WildXR application and is closed by the user selecting a **"Close"** button
      3. **Video** - A brief video with narration is played to show a new user how to navigate the WildXR application.
      4. **Dynamic** - If a user does not interact with the WildXR interface for a period of time the **Video** tutorial is played. The tutorial stops as soon as the user interacts with any WildXR elements.
   - **Tutorials** should not be used when playing a single video on a loop otherwise they may interfere with video playback - please select **None** in this situation

### Timer settings

- *Timer settings are only available to **System Admins** as they can influence how the WildXR application interacts with users*

- *If you think your installation would benefit from a specific timer setting, please contact WPS staff for assistance*

7. **App Timer Length, Idle Timer Length, Idle Timer Delay**
   - **App Timer Length Seconds** controls how long a new user can use the WildXR application before a grey wash overlays the interface. 
   - *This setting is considered a **Beta** feature and may not behave reliably in all situations*
   - **Idle Timer Length Seconds** acts as a backup to the headset **Presence Sensor** as presence detection can be unreliable with various Meta firmware versions
   - **Idle Timer Length** is the amount of time after which a lack of movement within the headset triggers a **Presence Sensor** event within the WildXR application
   - *This setting was primarily used to trigger **Spectator Camera** events on connected systems, but may also help gather **Analytic** data*
   - **Idle Timer Delay Seconds** is the delay between the time a headset detects new motion to the time at which it resets the headset view
   - **Idle Timer Delay** reduces the chance that a headset will show a non-standard view when mounted (put on by a user) after having been stored on a hook
   - *This delay is difficult to predict without some experience and should be custom-set for each **Installation** if **Idle Timer Length** is being used*
<div style="page-break-after: always;"></div>

### Globe Starting position 

8. **Globe Start Latitude and Longitude**
   - Determines where on the globe a gaze reticle will be positioned for new users
   - Not used when a single video is played on loop
   - If multiple **Map Markers** are used in a **Video Catalogue**, WPS recommends positioning the gaze reticle close to at least one marker
   - *WPS recommends using Google Maps to find a position that works best for your installation*
   - *WPS recommends not positioning your **Globe Start Lat. and Long.** too close to a **Map Marker**, as the associated gallery may open before the user realizes they can navigate the globe* 
   - Lat. and Long. coordinates can include decimal digits, but cannot be 0 and 0

### Video Catalogue settings

9. **Select Video Catalogue**
   - A **Video Catalogue** is a collection of videos that can be used for multiple **Installations**
   - Use the **"Web Portal Video Catalogue Creation Guide"** to create or edit a **Video Catalogue** and for more information about using catalogues for specific purposes
   - If you are logged in as an **Organization Admin**, only catalogues associated with your **Organization** or those created by **WildXR** staff are available
   - **System Admin** have access to all catalogues
   - Select the catalogue to be used for your **Installation**

10. **Show adult content**
    - Check the **"Show Graphic Death"** to expose videos that show adult content involving death or gore
    - Check the **"Show Graphic Sex"** to expose videos that show adult content involving reproductive behavior
    - If these boxes are left unchecked, videos that show this content will not be visible within the WildXR application
    - ⚠️ Regardless of whether these checkboxes are selected or not, it is possible to select a video as an **Installation** startup video that contains adult content.
    - ⚠️ Review video selection to ensure content is appropriate for your intended audiences. 
<div style="page-break-after: always;"></div>

### WildXR application startup behavior

11. **Select Startup Video, Loop Video, Resume Video**
    - Select a **"Startup Video"** to play when WildXR launches.
    - **Startup Videos** must be part of the currently selected **Video Catalogue**
    - Select the **"Startup Video Loop"** checkbox if you want the startup video to play continuously in the headset - this will be the only video that plays
    - If the **Startup Video** is a video introduction to an **Installation** and you want it to play once for each user, leave the **"Startup Video Loop"** box unchecked
    - If you want users to choose their own video from the **Video Catalogue** leave the **"Select Startup Video"** field blank
    - Checking the **"Resume Startup Video on Awake"** box will cause the video to continue playing when a new user picks up the headset instead of starting from the beginning

### Favorites

12. **Select Favorites, Filter Favorites by Default**
    - The **"Select Favorites"** field is multi-select and allows the selection of videos from the current **"Video Catalogue"**
    - Click the field to expose a drop-down menu of videos, or begin typing to have videos suggested based on title.
    - To remove videos from the **Favorites** list, click the **x** button in their title display.
    - Select the **"Filter Favorites By Default"** checkbox to have thumbnail galleries display **Favorites** instead of all videos represented by a **Map Marker**
    - *Users can switch to seeing all videos, instead of only favorites, by selecting the **All** button at the top of a thumbnail gallery*

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
<div style="page-break-after: always;"></div>

### Control, Demo Mode, Menu Tray, and Session Data

14. **Select Control**
    - By default, users interact with the WildXR user interface with **Gaze** control - controlling a selection reticle with head movement
    - Select **Hand Controllers** to allow users to use the physical controllers, modelled as hands, to interact with the WildXR user interface
    - ⚠️ The **Hand Controllers** option is still in development and may cause unexpected behavior in the app and is not recommended for public use
    - ⚠️ Giving the public access to the physical controllers associated with VR headsets allows them to exit WildXR and gain access to the general VR interface which is generally undesirable

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
<div style="page-break-after: always;"></div>

18. **Save new installation**
    - Click the **"Save"** button to save your new installation and allow its assignment to registered devices
    - Click the **"Cancel"** button to discard your installation and return to the **Installations** page

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

**Installation not showing in headset**
- Make sure you have assigned the **Installation** to a **Device** on the **Devices** page (refer to the **Web Portal Device Management Guide**)
- Ensure that the device in question is registered to the wildxr.org website and has a **WildXR Number**

**Unable to log onto the Wildxr.org website:**
- Ensure you are entering the correct credentials to log into Wildxr.org *(May have been supplied by WPS Staff)*
- If someone within your organization created your account; check that they assigned a password to your account *(passwords are not created automatically)*
- Double-check the URL you have entered into your Web Browser *(WPS recommends using Chrome)*

**Unable to edit an existing Installation:**
- **Organizations** are only allow to edit **Installations** that were created by their **Organization**
- **Organizations** can see **Installations** that were created by WPS Staff under the **WildXR** organization, but do not have permission to edit their contents

**Unable to change the Organization field during Installation creation or editing:**
- If you are logged in to the wildxr.org website as an **Organization Admin** you will not be able to edit the **Organization** field of an **Installation**
- If you feel the **Installation** in question should belong to a different **Organization** please contact WPS staff for assistance

**Organization field shows different Organization than expected or does not match my Organization:**
- Please double-check that you are logged into the correct account
- If you are a **System Admin** users, you will have access to all **Organizations** and can choose the correct value for the **Organization** field
- If you require further assistance please contact WPS staff
<div style="page-break-after: always;"></div>

**Tips do not display:**
- **Tips** are only shown to users during loading screens, both for the WildXR application and for videos within the WildXR application
- Most deployments launch WildXR automatically before opening hours and the initial loading screen tips will not be seen
- If your deployment includes videos on a loop, no loading screen will be shown and therefore **Tips** will not be displayed
- Most deployments have downloaded videos, not streaming videos, to increase playback quality, this results in a very brief loading screen before video playback and **Tips** may not be visible

**Tips display, but not as expected:**
- **Tips** display in a carousel, one-by-one, for a set period of time
- Each **Tip** should be one a single line, longer **Tips** should have no line-breaks, return/enter characters, between them
- Depending on the time a loading screen is shown, **Tips** might not be visible, or only the first **Tip** may display

**Tutorial not displayed:**
- Depending on the type of **Tutorial** selected, the interface may not show immediately on launch
- **Dynamic tutorials** will only show if there is not headset movement or interaction with UI elements by the user
- **Text** and **Video tutorials** may not show if a headset is passed from user to user, as opposed to the headset being put down and picked up
- If **Tutorials** continue to behave in an unexpected manner, please contact WPS Staff.

**Tutorial displaying and should not be:**
- Ensure that the **Select Tutorial Mode** field is correctly set to **None** and save the **Installation**
- If the **"Save"** button is light green, no changes have been applied and you can return to the **Installations** screen

**Timer settings:**
- Only **System Admin** users can access the **Timer settings** of an **Installation**
- By default, all **Timer settings** are set to 0.0 seconds, this works in most deployment situations
- If you would like to discuss adding **Timer settings** to your installation, please contact WPS staff
- ⚠️*Headset **Timer settings** interact with certain headset features that are controlled by **Meta** and the effects can change unexpectedly based on firmware updates*
<div style="page-break-after: always;"></div>

**Globe Starting position has no effect:**
- **Globe Starting position** is only used in deployments when users choose their own videos from a **Globe Scene**
- If you are playing a video on a loop **Globe Starting position** is not used
- Ensure that you have entered a valid starting position - a positive or negative decimal number (for example: 100.1212, -27.23)
- The WildXR application does not allow starting positions at the poles of the **Globe Scene**

**Globe Starting position starts application in Thumbnail Gallery:**
- If a **Globe Starting position** is too close to a **Map Marker** on the globe, the gaze reticle may immediately open the **Map Marker gallery** upon launch
- Place the **Globe Starting position** away from all Map Markers by 15° of both latitude and longitude

**Globe Starting position values produce an error:**
- 0, 0 is not considered a valid starting position in WildXR - use a small decimal value instead (for example 0.12, -0.12)

**Unsure of Video Catalogue selection:**
- **Installations** do not need to be assigned a **Video Catalogue** upon creation
- The base WildXR **Installation** is applied to all **Devices** that do not have an assigned **Installation** 
- The base **Installation** contains all WildXR-produced videos and all **Core Map Markers**
- **Video Catalogue** creation can occur after **Installation** creation if the goal is only to control some aspects of the user experience

**Video Catalogue missing:**
- **Organization Admins** only have access to **Video Catalogues** created by their **Organization** or owned by WildXR
- If you have created a **Video Catalogue** but cannot locate it, check the **Video Catalogue** page
- Ensure you are logged into the wildxr.org website with the correct credentials to view the missing catalogue

**Adult content showing in Installation:**
- Ensure that the **"Show Graphic ..."** boxes are not checked in the **Installation** in question
- If **Demo Mode** is not checked, users can access the **Admin Panel** and can expose adult content in the WildXR application
- If you have concerns that a video may not be labelled correctly as **Adult Content** please contact WPS staff
<div style="page-break-after: always;"></div>

**Desired startup video not available:**
- **Startup Video** selection is limited to videos contained within the assigned **Video Catalogue**
- Ensure you are searching for the correct video by title in the **Select Startup Video** field
- ⚠️ *Videos with **Adult Content** are still able to be selected as a **Startup Video** regardless of whether these videos have been hidden from normal view - always review the video selection before to deploying to the public* ⚠️

**Startup Video does not loop:**
- Ensure that the **Startup Video Loop** box is checked in the **Installation** details
  
**Startup Video continues to play when new user puts on headset:**
- Ensure that the **Resume Startup Video on Awake** box is unchecked in the **Installation** details page
- If the headset was being worn when WildXR first launched, this may affect whether the video starts from the beginning, relaunch WildXR and remove the headset before the loading screens to fix this issue
- Clean the presence sensor (found between the lenses) as dirt may prevent it registering a new user

**Desired Favorite video not available:**
- **Favorite** selection is limited to videos contained within the assigned **Video Catalogue**
- Ensure you are searching for the correct video by title in the **Select Favorites** field

**Fewer videos than expected are present in Installation:**
- When the **Filter Favorites by Default** box is checked, all galleries will display only **Favorite** videos, unless the user selects the **"All"** button at the top of the gallery
- If the **Show Graphic ...** boxes are unchecked, you will have hidden all **Adult Content** and only a portion of videos in a **Video Catalogue** will be displayed
- If a headset is offline when WildXR launches, WildXR will only display downloaded content - check your headset internet connection and relaunch WildXR
- Video content is determined by **Video Catalogue** contents, which is influenced by the selected **Map Markers** for a **Video Catalogue**
- Review the **Web Portal Map Marker Management Guide** and the **Video Catalogue Creation Guide** to ensure you have included all the videos desired in a **Video Catalogue**

**Videos not downloading to headset:**
- Video download speed and success are dependent on a strong, reliable internet connection
- Ensure that you have the correct **Automatic Download Mode** set for the behavior you expect
- ⚠️*Because video download success is dependent on internet speed and reliability, WPS recommends using **Download Entire Catalogue** only in specific situations where a **Video Catalogue** contains 20 or fewer videos or the user has an especially robust internet connection* ⚠️
- If there are frequent interruptions in internet service, downloaded videos may be degraded and show artifacts, distorted audio, or incomplete playback
- Always test downloaded video quality, and attempt to use WildXR offline after videos have downloaded and before deploying headsets to the public
<div style="page-break-after: always;"></div>

**Video Catalogue size is too large for download:**
- If you would like to install the entire video catalogue from WildXR, or a large percentage of it, please contact WSP staff for assistance
- ⚠️*Downloads will continue to process as long as the headset is connected to the internet and WildXR is running - 8 hours of download time can occur without user intervention (headset will sleep after 8 hours without interaction by a user)*

**We would like to use Hand Controllers in our deployment:**
- WPS recommends against using **Hand Controllers** in public deployments as it necessitates the user of the physical VR controllers
- Physical VR controllers allow users to exit the WildXR application and access other UI interfaces including headset settings
- Please contact WPS staff if you would like to discuss controller options for interaction with WildXR

**Users can delete/download videos and add/remove favorites:**
- Ensure that the **Demo Mode** checkbox is selected for your **Installation** as running WildXR in **Demo Mode** prevents such interactions
- Remember that headsets will need to be connected to the internet and the WildXR application must be stopped and restarted for changes to **Installation** settings to take effect

**Users can show/hide adult content:**
- Access to the **Admin Panel** can be prevented by running WildXR in **Demo Mode**, refer to Step #15
- Remember that headsets will need to be connected to the internet and the WildXR application must be stopped and restarted for changes to **Installation** settings to take effect

**Save button is unresponsive or light green in color:**
- If you are editing an existing **Installation** and attempt to save without making any changes the **"Save"** button will be unresponsive and light green in color

## Important Notes

⚠️ **Changes to Installation settings:** Changes to an Installation are not automatically applied to instances of WildXR. WildXR must be stopped and re-launched and the headset must have an internet connection for changes to take place.

⚠️ **Installations must be assigned to a registered device to be shown:** Installations are settings that determine what and how content is shown inside an instance of the WildXR application. An **Installation** must be assigned to device. Only devices registered on the wildxr.org website with a **WildXR Number** can be assigned an **Installation**

⚠️ **Video playback quality:** Videos that are not downloaded to your device will attempt to stream from the cloud. Streaming is dependent on internet strength and speed for quality, and is not recommended for use in a public setting. Download all videos necessary for your **Installation** before deploying a device for use in a public setting.

## Verification Steps

Verify that your installation creation or updates have been successful.

**Complete functionality verification:**
- Log out of the Wildxr.org Web Portal
- Log in and refresh the **Installations** page to ensure your installation appears as expected
- Assign your **Installation** to a **Device** and connect that device to the internet. Launch WildXR and confirm that the **Installation** behaves as expected
