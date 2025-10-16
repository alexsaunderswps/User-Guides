# Third Party Managed Quest VR Headset Setup Guide

## Purpose & Context
This guide provides the required steps to set up a Third Party Managed Quest VR headset for the first time. 
WPS may have created some needed accounts as part of their internal VR partner program. Check with WPS staff if you are unsure of what accounts your organization needs.
Account creation by WPS is done to facilitate smooth VR operation and increases our ability to provide technical support. 
Accounts created without the help of WPS staff cannot be accessed by WPS staff during technical support sessions and will not successfully enable ArborXR management.

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

⚠️ **Video Download Time**: Whenever a new instance or update of WildXR is required all associated videos must be downloaded to provide a smooth playback experience. Depending on the video library size and internet speed, this can take multiple hours. Please consider this when scheduling an update or planning for new WildXR installations.

## Prerequisites
- A WiFi internet connection
- Email account credentials associated with your VR setup *(may be provided by WPS)*
- Smartphone with 2FA app capability *(WPS recommends Google Authenticator)*
- Initial coordination with WPS staff for first-time login
- VR headsets

## Quick Overview (for experienced users)
1. Meta, Meta-for-Work, and ArborXR accounts are created for Organization *(may be provided by WPS)*
2. User registers headset with Meta-for-Work, assigning it a third-party MDM (Mobile Device Management)
3. Recommended settings are applied to headset
4. WildXR and Auto Launch *(if desired)* are installed on headset
5. Headset is registered with WildXR Website for remote provisioning
6. Videos are downloaded or side-loaded to improve WildXR performance 
<div style="page-break-after: always;"></div>

## Detailed Steps

### Meta Account Creation

- *Currently, all accounts using ArborXR and Meta-for-Work are created by WPS Staff*
- *These accounts are created by WPS Staff to provide IT support for Meta VR Headsets*
- *It is beyond the scope of this guide to instruct users in the creation of ArborXR and Meta-for-Work accounts for their organization*

### Logging in to Meta-for-Work

1. **Navigate to the Meta-for-Work (Horizon Managed) webpage**
   - Open web browser and go to `https://work.meta.com/login/landing/`

2. **Enter credentials**
   - Enter the Email address provided by WPS for your Meta-for-Work account
   - Click **"Next"**
   - Enter the Password provided by WPS for your Meta-for-Work account
   - Click **"Continue"**
   - *You may be required to authenticate via a 2FA application*
   - *Open Google Authenticator on your phone (you may have been provided with a Blu phone for this purpose)*
   - *Google Authenticator is associated with your Gmail account, this account is provided by WPS Staff*
   - You can choose to **Trust this device** based on security requirements at your organization

### Navigate to the Devices screen

3. **Overview Screen**
   - After logging in, you will be on the **Overview Screen**
   - On the left panel, click the **"Devices"** icon (shaped like a mask)
   - *Switch to your new VR headset for the next steps*

### Headset setup

4. **Power on headset**
    - Remove the packing material from the headset
    - Remove battery savers from hand controllers
    - **Quest 2**: Press **power button** on right side
    - **Quest 3 & Quest 3s**: Press **power button** on left side
    - Put on the VR headset
<div style="page-break-after: always;"></div>

5. **Initial introduction and connect to WiFi**
    - Follow the on-screen prompts in the VR Headset
    - *Occasionally, hand controllers will install an update that renders them inoperable for a brief period*
    - Connect your headset to your WiFi internet connection
    - *WPS recommends entering the WiFi details on your headset*
    - *If your WiFi network is hidden goto Step #6*
    - Your headset may apply firmware updates
    - Leave your headset plugged in while updates are downloaded
    - *Your headset may indicate that you can continue setup in the Meta Horizon phone app*
    - ⚠️ **Allow the headset to install all pending updates (*it may restart*) before proceeding** ⚠️
    - ⚠️ **DO NOT continue setup in the Meta Horizon app as this will not allow pairing with Meta-for-Work and ArborXR** ⚠️

6. **Adding a hidden network to WiFi**
    - *You may need assistance from your company's IT department if you have a robust WiFi security program*
    - In the WiFi window, scroll down to **"+ New Network >"**
    - Click to add a new network
    - Click **"Advanced"**
    - Under **"Hidden Network"** change displayed value to **"Yes"**
    - Generally, the default values for the rest of the Advanced menu will be sufficient
    - *If you continue to have issues connecting to a hidden WiFi network you may need to contact your company's IT department*
    - Click **"Confirm"**
    - If your WiFi network has a password, it most likely uses **WPA/WPA2-Personal** as the **"Security"** setting
    - Enter the remaining details of your WiFi network
    - Click **"Connect"** to finish WiFi setup and connect to the network

### Pair headset to Meta-for-Work

- *After all updates have been applied, you will see a **Pair your headset with the Meta Horizon app to Continue** screen*

- *At the bottom of this screen, you will see a **Connect to your organization** button*

7. **Begin headset connection**
   - Click the **Connect to your organization** button to continue
   - Click **"Continue"** on the **Connect your headset to your work or school** screen
   - Click **"Continue"** on the **You'll need your computer for the next step** screen
   - Your device should now show a website address and 8-character code
   - *Switch to your computer for the next steps*
<div style="page-break-after: always;"></div>

### Enroll headset on Meta-for-Work website

8. **Enroll device on Meta-for-Work website**
   - Return to the **Devices** page of the **Meta-for-Work** website
   - Click the **"+ Enroll devices"** drop-down menu
   - Select the **"In Admin Center"** option

9. **Select device configuration**
   - An **Enroll devices** pop-up window will appear
   - Click the **"Select device preset, third-party enrollment or group"** drop-down menu
   - Click the **"Device groups"** drop-down menu
   - You should see an option related to your **Organization** with a sub-text **ArborXR-Third-party**
   - Click the option listing your **Organization**
   - *If there is more than one option, or if the correct option is not clear, please contact WPS Staff*

10. **Enter device temporary code**
    - There should be an 8-character code shown in your VR headset.
    - Enter this 8-character code in the appropriate field on the **Enroll devices** pop-up
    - If you have entered the code correctly a third step should now be visible on the **Enroll devices** pop-up

11. **Select device account**
    - Ensure that **Complete device setup with your own managed Meta Account** is selected.
    - Click the **"Enroll device"** button
    - *There is a time limit on 8-character code validation*
    - *If you are told **This code has expired** click the **"Back"** button twice to return to the **"You'll need a computer for the next step"** screen and then click **"Continue"** to regenerate a new code*

12. **Return to Manage devices screen**
    - Click the **"Manage devices"** button to return to the Meta-for-Work device management page.
    - If you have more headsets to enroll, click the **"Enroll another headset"** button
    - *Your headset will not be visible in the **Managed Devices** section of the Meta-for-Work webpage until configuration is complete*
    - *Switch to your VR headset for the next steps*
<div style="page-break-after: always;"></div>

### Headset configuration

13. **Finish initial headset configuration**
    - *You will need to be wearing the headset to complete the initial configuration*
    - *You will see various linking and connecting screens while the device is linked to your Meta-for-Work account*
    - On the **Connect to device management** screen, click the **"Continue"** button
    - *A **Connecting to management** screen will show*
    - On the **Configure your headset** screen click the **"Continue"** button
    - *A **Configuring your headset** screen will show*
    - On the **Headset configured** screen, click the **"Continue"** button
    - On the **Configuring** screen click the **"Continue"** button
    - A few more screens may show during installation, leave the headset on during this process or progress may halt.
    - *Refresh the Meta-for-Work **Devices** web-page - your device should now be visible*

### **Accept conditions from Meta**

14. **Accept disclaimers in VR headset**
    - Click **"Continue"** on the safety guidelines
    - Click **"Continue"** on the privacy declarations
    - Click **"Don't Share"** or **"Share"** on the share additional data request
    - Click **"Not now"** on the Enable hand and body tracking request
    - Click **"Skip"** on setting up accessibility settings
    - *We recommend not having controllers available to the public during WildXR use which negates all accessibility options*
    - Click the **"Welcome"** button to see tutorial options
    - Participate in tutorials as desired *(Skipping tutorials does not affect headset setup)*

### **Additional headset settings**

- *Additional headset settings need to be applied before your headset is ready for use - See Step #19*

- *WPS recommends completing the ArborXR connection steps below first, as some settings may be unavailable before doing so*
<div style="page-break-after: always;"></div>

### **Connect VR headset to ArborXR group**

- *The assignment of your headset to an ArborXR must currently be done by WPS staff*

- *To prevent other organizations from seeing your devices, access in ArborXR is limited to devices already in your organizational group*

- *Contact WPS Staff to move your device to the correct group before proceeding with Step #18 below*

- *Your Meta VR headset is ready for management through the ArborXR website*

- *Your headset now has the base installation for use, but needs to be assigned a group in ArborXR before other needed software is loaded*

### **Log in to ArborXR web portal**

15. **Navigate to the ArborXR webpage**
    - Open web browser and go to `https://api.xrdm.app/login`

16. **Navigate to Devices page**
    - Click on the **"Devices & Groups"** tab in the left column
    - *This interface lists all the **Devices** currently managed by WPS through ArborXR*
    - *Before you make any changes, verify that the device you are about to edit belongs to your organization*
    - *Check the device serial number on the ArborXR website matches the device name on the Meta-for-Work website*

### **Claim your device**

17. **Move your device to your organization group**
    - *Before you make any changes, verify that the device you are about to edit belongs to your organization*
    - *Check the device serial number on the ArborXR website matches the device name on the Meta-for-Work website*
    - Select the checkbox next to your device serial number
    - Click on the **"Actions"** drop-down menu
    - Select the **"Assign to Group"** option from the menu
    - Click the **"Select group..."** field and select you organization group
    - *There should be only one option for group selection*
    - *If there is more than one option, or the correct option is not clear, please contact WPS Staff for assistance*
    - Click the **"Assign to Group"** button
<div style="page-break-after: always;"></div>

### Finish device configuration

18. **Allow ArborXR configuration to finish**
    - Once assigned to a group additional configuration parameters will be added to the headset
    - *Your headset may reboot during this ArborXR configuration, that is normal*
    - *You should see notifications that **Social** and **Horizon Store** features have been disabled for your headset*

### Additional Headset set-up steps

19. **Decline to install additional apps**
    - *A screen prompting you to install additional applications may appear in your VR headset*
    - *ArborXR should automatically install the **WildXR** and **WildXRAutoPing** applications*
    - *Other applications are not needed for the proper functioning of **WildXR** and do not need to be installed*

20. **Recommended settings for VR headsets**
    - Follow the **Recommended Headset Settings** guide
    - *Occasionally with managed headsets the **Passthrough** view will not be disabled as expected while editing **Developer Settings***
    - *If you have toggled off **Physical Space Features** but can still see the external environment through the headset do the following:*
        1. Toggle on **Physical Space Features**
        2. Open the **Quick Settings Menu** - click the button displaying time, WiFi strength, and battery level
        3. Click the **Passthrough** button so that passthrough shows **Off** and the external environment becomes hidden
        4. Return to the **Developer Settings** and toggle off **Physical Space Features**
    - *Not all of the **Recommended Settings** will be available in managed headsets - this is normal and expected*

21. **Remove unneeded software**
    - Follow the **Library Management** guide
    - *In managed headsets the primary library curation will be the **Hiding** and **Locking** of unneeded applications*
    - *Not all of the **Library Management** options will be available in managed headsets - this is expected*
<div style="page-break-after: always;"></div>

22. **Launch WildXR once**
    - After all other steps have been completed, launch the WildXR application.
    - *The **WildXR** application can be found by clicking the **Library** button (a 3x3 dot icon) in the menu bar*
    - *Occasionally, no application will show in the **All** section of the **Library** - click the **For Work** tab if this is the case*
    - A permissions screen may appear - Click the **"Allow"** button
    - Follow the **Web Portal Device Management Guide** to register your device and allow content management
    - ⚠️ **New Installations of WildXR need time to download the appropriate videos. This could take multiple hours depending on the size of the video library.** ⚠️

23. **Launch WildXRAutoPing once**
    - After all other steps have been completed, launch the WildXRAutoPing application.
    - *The **WildXRAutoPing** application can be found by clicking the **Library** button (a 3x3 dot icon) in the menu bar*
    - *Occasionally no application will show in the **All** section of the **Library** - click the **For Work** tab if this is the case*
    - *WildXR should launch, and should now launch each time the headset is powered on*
    - Reboot your headset to ensure that autolaunch is working

## Troubleshooting

**Cannot access Meta-for-Work account:**
- Verify Email address is correct for your VR setup *(If provided by WPS)*
- Contact WPS for password assistance
- Ensure you are accessing the **Meta-for-Work** account (https://work.meta.com) and not the personal Meta account (https://www.meta.com) that you may have used in the past

**Confirmation code from Meta-for-Work absent:**
- Confirmation codes can be delayed by slow or intermittent internet connections
- Check the **Spam** folder in your email browser
- Ensure you are looking in the correct email account *(account may have been provided by WPS)*

**Meta-for-Work account asking for 2-Factor Authorization (2FA):**
- WPS staff will prepopulate a **Google Authenticator** account for Meta-for-Work
- If you were given a Blu phone during deployment, access the Google Authenticator application and look for the Meta-for-Work 2FA code
- If you were not given a Blu phone during deployment, you may be required to download the Google Authenticator application on your work phone
- Use the Gmail account associated with your WPS VR deployment to log into Google Authenticator
<div style="page-break-after: always;"></div>

**No devices shown on Devices screen in Meta-for-Work:**
- Ensure you have logged into the correct **Meta-for-Work** account (one provided by WPS)
- Devices will not show on the Meta-for-Work screen until you have a least one device registered.
- Ensure you are on the **Devices** page and not the **Overview** page

**Headset doesn't recognize hand controllers**
- On the initial boot of a headset, firmware updates may be applied to hand controllers that render them temporarily non-functional
- Wait 2 - 3 minutes before trying to use hand controllers again
- Insert fresh batteries into the hand controllers
- Very rarely there may be other issues with hand controllers - Schedule a help session with WPS Staff for additional guidance

**VR headset not connecting to WiFi:**
- Occasionally a device may have trouble connecting to a WiFi network
- Ensure your IT department allows unrecognized devices to connect to your company's WiFi channel
- Register the VR device with your IT department if needed
- Ensure that you have selected the correct WiFi network if there are many to choose from
- Double check that you have entered the network password correctly
- If you are attempting to connect to a hidden WiFi network you may need assistance from your IT department (hidden networks may have settings not covered by this guide)
- If possible, attempt to connect to a different network or phone hotspot

**Updates are slow to apply:**
- Internet connection speed will dictate how quickly headset updates are applied
- It is difficult to switch networks once updates have begun downloading

**Cannot find the Meta Horizon app:**
- For Meta-for-Work and ArborXR managed headsets you should not use the Meta Horizon application
- The Meta Horizon app is for personal VR account management only
- If you have questions about which service you should be using please contact WPS staff

**Five character code is shown, not eight character:**
- A 5 character code is associated with personal VR account management
- Make sure you have selected the **Connect to your organization** button for headset connection 
<div style="page-break-after: always;"></div>

**Unable to Enroll headset on Meta-for-Work site:**
- Make sure you are on the **Meta-for-Work** account (https://work.meta.com) and not the personal Meta account (https://www.meta.com) that you may have used in the past
- Ensure you are on the **Managed devices** tab of the **Devices** page, not the **Overview** page of Meta-for-Work
- Check you have selected **In Admin Center** from the enrollment options under the **+ Enroll devices** drop down menu

**Unable to select device preset in Enroll devices menu:**
- Click the **Device groups** option under the **Select how the device will be configured** step
- If you do not see your organization's name, contact WPS Staff for assistance with Device registration

**Unable to Log into ArborXR account:**
- Verify Email address is correct for your VR setup *(If provided by WPS)*
- Contact WPS for password assistance

**I cannot add a device to my ArborXR account:**
- In order to prevent access to devices outside of your organization all devices must first be assigned to your organization by WPS staff
- Please reach out to WPS staff to have your headset moved to the appropriate group within ArborXR

**Other applications can be installed on my headset:**
- Meta automatically installs some applications on all headsets by default
- Follow the **Library Management** guide to hide or remove these applications if possible
- Locking applications with a PIN number can prevent unauthorized access by users

**WildXR and WildXRAutoPing are not installed:**
- Depending on settings applied to your headsets, application installations may be limited by day and time
- Contact WPS staff for help if installations are needed sooner or if you are unsure when installations are scheduled

**Unable to toggle off Passthrough:**
- Passthrough allows you to see the external environment while wearing the VR headset
- If you have already toggled off **Physical Space Features** in the **Developer Settings** you will be unable to turn off passthrough
- Return to **Developer Settings** and toggle **Physical Space Features** on, then adjust passthrough settings as detailed in Step #20
<div style="page-break-after: always;"></div>

**Unable to find or change some settings:**
- Both Meta-for-Work and ArborXR configurations remove the ability to change some settings on VR headsets
- It is unlikely that the unavailable settings are impactful to headset use
- If you have concerns, or the headset is not behaving as expected, please contact WPS staff

**Unable to remove or hide some applications:**
- Meta prevents the removal or hiding of some automatically installed applications
- It is beyond the ability of WPS to influence the installation of these applications
- Creating a PIN and locking applications will help with access control

**The WildXR application is not playing the expected content:**
- WildXR instances depend on connection with the WildXR.org website to play specific content
- Ensure that you have created a **WildXR Number** through the application and registered your device according to the **Web Portal Device Management Guide**
- If you have not been trained on the **WildXR.org** website, or are unsure of next steps to assign an **Installation** to your headset, please contact WPS staff for assistance

**The WildXR application is not launching automatically on headset startup:**
- Make sure that the **WildXRAutoPing** application has been installed on your device
- Launch the **WildXRAutoPing** app once by clicking on it
- If you continue to have issues with WildXR not launching on headset startup, please contact WPS staff

## Important Notes

⚠️ **Meta-for-Work**: **Meta-for-Work** is different than the **Meta Horizon** application used to setup Quest headsets. If you are unsure as to which platform you should be using for headset management please contact WPS staff.

⚠️ **Avatar Creation**: Meta may require the creation of a virtual avatar. This avatar is visible in some locations throughout the VR "metaverse" depending on privacy settings.

⚠️ **Application Installation**: While a headset is configuring it may take some time for all applications to be installed. Depending on internet connection speeds and device settings, application installation may occur after normal business hours. If there are continued issues with the installation of **WildXR** or **WildXRAutoPing** please contact WPS staff.

⚠️ **WildXR Content**: Most WildXR content is managed through the WildXR.org website. If you have not received training on the WildXR.org website please contact WPS staff for assistance provisioning your headset. In most cases provisioning new headsets will require the download of video files for the best playback experience. 
