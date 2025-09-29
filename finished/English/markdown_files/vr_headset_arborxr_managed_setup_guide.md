# ArborXR Managed Quest VR Headset Setup Guide

## Purpose & Context
This guide provides the required steps to setup an ArborXR managed Quest VR headset for the first time. 
WPS may have created some needed accounts as part of their internal VR partner program. Check with WPS staff if you are unsure of what accounts your organization needs.
Account creation by WPS is done to facilitate smooth VR operation and increases our ability to provide technical support. 
Accounts created without the help of WPS staff cannot be accessed by WPS staff during technical support sessions and will not successfully enable ArborXR management.

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

## Prerequisites
- A WiFi internet connection
- Email account credentials associated with your VR setup *(may be provided by WPS)*
- Smartphone with 2FA app capability
- Initial coordination with WPS staff for first-time login
- VR headsets

## Quick Overview (for experienced users)
1. Meta, Meta-for-Work, and ArborXR accounts are created for Organization *(may be provided by WPS)*
2. User registers headset with Meta-for-Work, assigning it a third-party MDM (Mobile Device Management)
3. Recommended settings are applied to headset
4. WildXR and Auto Launch *(if desired)* are installed on headset
5. Headset is registered with WildXR Website for remote provisioning
6. Videos are downloaded or side-loaded to improve WildXR performance 

## Detailed Steps

### Meta Account Creation

- *Currently, all accounts using ArborXR and Meta-for-Work are created by WPS Staff*
- *These accounts are created by WPS Staff to provide IT support for Meta VR Headsets*
- *It is beyond the scope of this guide to intruct users in the creation of ArborXR and Meta-for-Work accounts for their organization*

### Logging in to Meta-for-Work

1. **Navigate to the Meta-for-Work (Horizon Managed) webpage**
   - Open web browser and go to `https://work.meta.com/login/landing/`
<div style="page-break-after: always;"></div>

2. **Enter credentials**
   - Enter the Email address provided by WPS for your Meta-for-Work account
   - Click **"Next"**
   - Enter the Password provided by WPS for your Meta-for-Work account
   - Click **"Continue"**
   - *You may be required to Authnticate via a 2FA application*
   - *Open Google Authenticator on your phone (you may have been provided with a Blu phone for this purpose)*
   - *Google Authenitcator is associated with your Gmail account, this account is provided by WPS Staff*
   - You can choose to **Trust this device** based on security requirements at your organization

### Navigate to the Devices screen

3. **Overview Screen**
   - After logging in you will be on the **Overview Screen**
   - On the left panel, click the **"Devices"** icon (shaped like a mask)
   - *Switch to your new VR headset for the next steps*

### Headset setup

4. **Power on headset**
    - Remove the packing material from the headset
    - Remove battery savers from hand controllers
    - **Quest 2**: Press **power button** on right side
    - **Quest 3 & Quest 3s**: Press **power button** on left side
    - Put on the VR headset

5. **Initial introduction and connect to WiFi**
    - Follow the on-screen prompts in the VR Headset
    - *Occasionally hand controllers will install an update that renders them inoperable for a brief period*
    - Connect your headset to your WiFi internet connection
    - *WPS recommends entering the WiFi details on your headset*
    - *If your WiFi network is hidden goto Step #6*
    - Your headset may apply firmware updates
    - Leave your headset plugged in while updates are downloaded
    - *Your headset may indicate that you can continue setup in the Meta Horizon phone app*
    - ⚠️ **Allow the headset to install all pending updates (*it may restart*) before proceeding** ⚠️
    - ⚠️ **DO NOT continue setup in the Meta Horizon app as this will not allow paring with Meta-for-Work and ArborXR** ⚠️
<div style="page-break-after: always;"></div>

6. **Adding a hidden network to WiFi**
    - *You may need assistance from your company IT department if you have a robust WiFi security program*
    - In the WiFi window scroll down to **"+ New Network >"**
    - Click to add a new network
    - Click **"Advanced"**
    - Under **"Hidden Network"** change displayed value to **"Yes"**
    - Generally the default values for the rest of the Advanced menu will be sufficient
    - *If you continue to have issues connecting to a hidden WiFi network you may need to contact your company IT department*
    - Click **"Confirm"**
    - If your WiFi network has a password, it most likely uses **WPA/WPA2-Personal** as the **"Security"** setting
    - Enter the remaining details of your WiFi network
    - Click **"Connect"** to finish WiFi setup and connect to the network

### Pair headset to Meta-for-Work

- *After all updates have been applied you will see a **Pair your headset with the Meta Horizon app to Continue** screen*
- *At the bottom of this screen you will see a **Connect to your organization** button*

7. **Begin headset connection**
   - Click the **Connect to your organization** button to continue
   - Click **"Continue"** on the **Connect your headset to work or school** screen
   - Click **"Continue"** on the **You'll need your computer for the next step** screen
   - *Switch to your computer for the next steps*

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
<div style="page-break-after: always;"></div>

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
    - *Your headset will not be visible in the **Managed Devices** section of the Meta-for-Work webpage until configuarion is complete*
    - *Switch to your VR headset for the next steps*

### Headset configuration

13. **Finish initial headset configuration**
    - *You will need to be wearing the headset to complete the initial configuration*
    - On the **Connect to device management** screen click the **"Continue"** button
    - On the **Configure your headset** screen click the **"Continue"** button
    - On the **Headset configured** screen click the **"Continue"** button
    - On the **Configuring** screen click the **"Continue"** button
    - A few more screens may show during installation, leave the headset on during this process or progress may halt.
    - *Refresh the Meta-for-Work **Devices** web-page - your device should now be visible*

### **Accept conditions from Meta**

14. **Accept disclaimers in VR headset**
    - Click **"Continue"** on the safety guidelines
    - Click **"Continue"** on the privacy declarations
    - Click **"Don't Share"** or **"Share"** on the share additional data request
    - Click **"Not now"** on the Enable hand and body tracking request
    - Click **"Skip"** on setting up accessability settings
    - *We recommend not having controllers available to the public during WildXR use which negates all accessability options*
    - Click the **"Welcome"** button to see tutorial options
    - Participate in tutorials as desired *(Skipping tutorials does not affect headset setup)*
<div style="page-break-after: always;"></div>

### **Connect VR headset to ArborXR group**

*Your Meta VR headset is read for management through the ArborXR website*
*Your headset now has the base installation for use, but needs to be assigned a group in ArborXR before other needed software is loaded*

### **Log in to ArborXR web portal**

15. **Navigate to the ArborXR webpage**
    - Open web browser and go to `https://api.xrdm.app/login`

16. **Navigate to Devices page**
    - Click on the **"Devices & Groups"** tab in the left column
    - *This interface lists all the **Devices** currently managed by WPS through ArborXR*
    - *Before you make any changes, verify that the device you are about to edit belongs to your organization*
    - *Check the device serial number on the ArborXR website matches the device name on the Meta-for-Work webiste*

### Claim your device

17. **Move your device to your organization group**
    - *Before you make any changes, verify that the device you are about to edit belongs to your organization*
    - *Check the device serial number on the ArborXR website matches the device name on the Meta-for-Work webiste*
    - Select the checkbox next to your device serial number
    - Click on the **"Actions"** drop-down menu
    - Select the **"Assign to Group"** option from the menu
    - Click the **"Select group..."** field and select you organization group
    - *There should be only one option for group selection*
    - *If there is more than one option, or the correct option is not clear, please contact WPS Staff for assisstance*
    - Click the **"Assign to Group"** button

### Finish device configuration

18. **Allow ArborXR configuration to finish**
    - Once assigned to a group additional configuration parameters will be added to the headset
    - *Your headset may reboot during this ArborXR configuration, that is normal*
    - Click **"Continue"**
    - You will be taken to the Meta Horizon dashboard

### Headset setup

18. **Power on headset**
    - Remove the packing material from the headset
    - Remove battery savers from hand controllers
    - **Quest 2**: Press **power button** on right side
    - **Quest 3 & Quest 3s**: Press **power button** on left side
    - Put on the VR headset

19. **Initial introduction and connect to WiFi**
    - Follow the on-screen prompts in the VR Headset
    - *Occasionally hand controllers will install an update that renders them inoperable for a brief period*
    - Connect your headset to your WiFi internet connection
    - *WPS recommends entering the WiFi details on your headset*
    - *If your WiFi network is hidden goto Step #20*
    - Your headset may apply firmware updates
    - Leave your headset plugged in while updates are downloaded
    - *Your headset may indicate that you can continue setup in the Meta Horizon phone app*
    - ⚠️ **WPS does not recommend you do so and suggests waiting until the headset displays your pairing code**
<div style="page-break-after: always;"></div>

### Add a hidden WiFi network

20. **Adding a hidden network to WiFi**
    - *You may need assistance from your company IT department if you have a robust WiFi security program*
    - In the WiFi window scroll down to **"+ New Network >"**
    - Click to add a new network
    - Click **"Advanced"**
    - Under **"Hidden Network"** change displayed value to **"Yes"**
    - Generally the default values for the rest of the Advanced menu will be sufficient
    - *If you continue to have issues connecting to a hidden WiFi network you may need to contact your company IT department*
    - Click **"Confirm"**
    - If your WiFi network has a password, it most likely uses **WPA/WPA2-Personal** as the **"Security"** setting
    - Enter the remaining details of your WiFi network
    - Click **"Connect"** to finish WiFi setup and connect to the network

### Pair headset to Meta Horizon phone app

21. **Navigate to Devices in Horizon app**
    - Open your Meta Horizon phone app
    - The Meta Horizon app will show the account avatar and a hamburger menu *(three horizontal bars)* on the right side.
    - Open the hamburger menu
    - Under **Device Management** click **Devices**

22. **Pair headset with Meta Horizon app**
    - Find the **Add Device** or **Pair New Headset** option and click it
    - Select the correct model of Meta headset
    - *You may be prompted to create an avatar - this step is now required by Meta*
    - *This avatar is visible to other Meta Horizon users*
    - Create an avatar and click **"Continue"**
    - Select the correct WiFi connection state of your device
    - *If you connected to WiFi in Step 19, select **Device is already connected to WiFi*** 
    - Your headset should be displaying a five digit code
    - Enter the five digit code when prompted
    - Click **"Continue"** when the paring successful screen is shown

### **Accept conditions from Meta**

23. **Accept disclaimers in Meta Horizon app**
    - Click **"Continue"** on the safety guidelines
    - Click **"Don't Share"** or **"Share"** on the share additional data request
    - Click **"Not now"** on the Enable hand and body tracking request
    - Click **"Skip"** on the Start 3-month trial offer *(This screen may or may not be present)*
    - Click **"Skip"** on the Add a payment method
    - Click **"Close"** on the **You're all set!** screen
<div style="page-break-after: always;"></div>

### **Finish headset setup**

24. **Finish Headset introduction**
    - Put on the VR headset for a brief introduction to your headset from Meta
    - Follow on-screen prompts
    - Participate in tutorials as desired *(Skipping tutorials does not affect headset setup)*
    - *You must keep the headset on during the introduction*
    - After the introduction you will be shown the Horizon dashboard

## Next Steps

**Enable Developer Mode**
- Follow the **Developer Mode Setup** guide
- Developer mode is needed to apply some recommended settings
- Developer mode is needed to remove the required safety boundary

**Apply Recommended Headset Settings**
- Follow the **Recommended Headset Settings** guide

**Remove Unneeded Software**
- Follow the **Library Management** guide

## Troubleshooting

**Cannot access Meta account:**
- Verify Email address is correct for your VR setup *(If provided by WPS)*
- Contact WPS for password assistance

**Confirmation code from Meta absent:**
- Confirmation codes can be delayed by slow or intermittent internet connections
- Check the **Spam** folder in your email browser
- Ensure you are looking in the correct email account *(account may have been provided by WPS)*

**2FA devices already exist for Meta account**
- If your Meta account was created by WPS staff it will be prepopulated with 2 - 3 2FA devices
- One of these devices should correspond to the email account provisioned by WPS
- Other 2FA devices will be used by WPS Staff to assist in troubleshooting if issues arise

**"Add" button greyed out for 2FA:**
- Account may have maximum devices linked
- Contact WPS to remove unused devices
- Some account types have device limits
<div style="page-break-after: always;"></div>

**Cannot find Meta Horizon application:**
- The Meta Horizon application is available for download in the Apple App store or Google Play store
- If you are using a phone supplied by WPS the app should be present - search for Horizon
- The Meta Horizon app may not be placed on the first page of your phone
- Use the phone search function to find Meta Horizon and move it to an obvious location

**Cannot log into the Meta Horizon app**
- Ensure you are using the same account that was used in the Meta Account Creation steps
- Ensure you have selected "Enter Password instead" if you are attempting to enter a password
- Double check your password, it will be the Meta Account, not email account password for Horizon login

**2FA fails for the Meta Horizon app**
- Ensure you are using the correct 2FA account for authorization
- If you are using SMS/WhatsApp for authorization only one phone number is associated with the account
- 2FA codes are valid for 30 seconds on average, wait until a new code is generated and attempt to log in

**Meta won't allow my desired username**
- Meta restricts the format of usernames to enforce uniqueness.
- Edit the username to include unlines or numbers
- Remember that this username may become visible to other Meta Horizon users

**Headset doesn't recognize hand controllers**
- On the initial boot of a headset firmware updates may be applied to hand controllers that render them temporarily non-functional
- Wait 2 - 3 minutes before trying to use hand controllers again
- Insert fresh batteries into the hand controllers
- Very rarely there may be other issues with hand controllers - Schedule a help session with WPS Staff for additional guidance

**Headset unable to connect to WiFi**
- Ensure your IT department allows unrecognized devices to connect to your company's WiFi channel
- Register the VR device with your IT department if needed
- Ensure you have the correct WiFi network and password entered into the appropriate fields
- If your WiFi network is hidden, go to Step #20 - *You may need assistance from your IT department with hidden networks*

**Unable to find Devices menu in the Horizon App**
- Ensure you are on the main page of the Meta Horizon app - *You should see your user avatar and name*
- Close the Horizon App and reopen the application to load the main page
- Identify the hamburger menu on the right-side of the application - icon is three stacked horizontal bars
- Open the hamburger menu and scroll down to see the **"Device management"** section
- Check if there are outstanding updates for the Meta Horizon app or your phone operating system
<div style="page-break-after: always;"></div>

**Forced to create an Avatar**
- Meta now forces users to create an Avatar for their user
- If you have disabled or blocked most social media this avatar will be minimally visible to other users
- If you want to check your privacy settings, open the hamburger menu and scroll down to **"Privacy and security"** to open the **"Privacy settings"** section

**5-digit pairing code not accepted**
- It may take a while for headset pairing to complete depending on internet connectivity
- Ensure your phone and headset are on the same WiFi network
- Double-check the code displayed in the headset and as entered into the Meta Horizon app

## Important Notes

⚠️ **Meta Horizon app**: Meta requires the use of the phone application **Meta Horizon** to setup Quest headsets.

⚠️ **Avatar Creation**: Meta requires the creation of a virtual avatar. This avatar is visible in some locations throughout the VR "metaverse" depending on privacy settings.

⚠️ **Difficulty with 2FA**: When Meta asks for a 2FA method there may be multiple options presented. Only one phone number can be used for SMS/WhatsApp alerts for authentication. Ensure you are selecting the correct account for 2FA. 2FA codes generally last for 30 seconds, if a code is about to expire, wait for a new one to be generated.

⚠️ **Internet networks**: If your headset and phone are not connected to the same WiFi network it may not be possible to pair your headset with the app.
