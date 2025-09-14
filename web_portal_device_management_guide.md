# WildXr Web Portal Device Management Guide

## Purpose & Context
This guide introduces the management of devices (headsets or computers) running the WildXR VR application via the WildXR Web Portal (Wildxr.org)

## Prerequisites
- Windows or Mac computer with internet access
- An internet browser (WPS recommends Chrome)
- A WildXR account with credentials *(may have been created by WPS staff)*
- A **"Device"** - either a VR headset (Quest 2, Quest 3, or Quest 3s) or Computer - with the WildXR application installed

## Quick Overview (for experienced users)
1. Navigate to the Wildxr.org website
2. Log In with your Username and Password *(may be provided by WPS staff)*
3. Navigate to the Admin -> Devices page
4. Edit an exisitng or Add a new Device
5. *If adding a new device - you will need to launch the WildXR application to generate a device id*
6. Verify the device settings

## Detailed Steps

### Access Device Management page on Wildxr.org

1. **Navigate to WildXR web portal**
   - Open web browser and go to WildXR web portal
   - Visit https://wildxr.org

2. **Log In to WildXR web portal**
   - Enter your Username in the appropriate field
   - Enter your Password in the appropriate field
   - Click **"Log In"**
<div style="page-break-after: always;"></div>

3. **Navigate to the Devices management page**
   - In the top navigation bar, click **"Admin"**
   - In the dropdown menu that appears click **"Devices"**
   - *If you are an Organization Admin you will only see devices associated with your organization*
   - *If you are a System Admin you will see all devices across all organizations*
   - To **"Add"** a new device continue to Step 4
   - To **"Edit"** an exisiting device, continue to Step 10

### Add a New Device

4. **Generate a WildXR number**
   - Launch the WildXR application on your device
   - There should be a **gear icon** visible to the right of the **Menu Tray** this is the **Settings Menu**
   - Open the **"Settings Menu"** by holding the gaze reticle *white dotnut shaped selector* over the **gear icon**
   - Select the **Generate** button in the bottom right of the **""Settings Menu"**
   - Write down the 10 character WildXR Number
   - Click the **"Acccept"** button and quit the WildXR application

5. **Lookup device on Wildxr.org**
   - Click the **"Device Lookup"** button in the upper right of the **Devices** page
   - Enter the 10 character WildXR Number that was displayed on the device in Step 4
   - Click **"Apply"**

### Enter Device Details and Installation

6. **Confirm WildXR number**
   -In the **"Device Details"** screen, confirm that the WildXR Number matches the number from Step 4

7. **Enter device name and select organization**
   - Enter a descriptive name in the **"Name"** field
   - *WPS recommends including the last 7 characters of the device serial number as well as an abbreviation of your organization's name in the device name*
   - *For example (WPS - Q022VC7 - location)* 
   - If you are a **Organization Admin** the device will automatically be added to your organization
   - If you are a **System Admin** select the correct organization from the **"Organization"** dropdown menu
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