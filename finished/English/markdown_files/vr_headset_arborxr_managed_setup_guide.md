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

- *If WPS staff created the Meta Account used to register headsets this step may be complete*

1. **Navigate to Meta**
   - Open web browser and go to `meta.com`

2. **Access login**
   - Click the **Account icon** *(person silhouette)* in upper right
   - Select **"Sign up or log into a Meta account"**
   - Choose **"Continue with email"**
<div style="page-break-after: always;"></div>

3. **Enter credentials**
   - Click **Continue with Email**
   - Enter Email address associated with your VR setup
   - Click **"Next"**
   - Choose **"Create new account"**
   - Enter your the requested details as needed for account creation
   - *When adding a birthday - WildXR is recommended for ages 13+ - enter a date that satisfies this requirement*
   - Choose a password for your account *(WPS staff will not have access to your password)*
   - Secure your account details (email and password) for future use
   - Click **"Next"**

4. **Manage login persistence (optional)**
   - Choose whether to save login credentials on this computer
   - *Saving credentials only stores email and password information*
   - *Consider security implications of saved credentials on shared computers*

5. **Verify account details** 
   - Review the account details as entered
   - *Uncheck the receive marketing emails box*
   - Click **"Create account"**

6. **Confirm account creation**
   - Open the email account associated with your Meta account
   - Copy the confirmation code from the recent Meta email
   - Enter the confirmation code in the appropriate box.
   - Click **"Next"**

7. **Access account dashboard**
   - You'll return to `meta.com` main page
   - Click the **Account icon** again to access account features *(Icon is now a circle with a letter or Logo)*
   - Select **"Accounts Center"** for main dashboard

### Two-Factor Authentication

- *Now is a good time to set up two-factor authorization as it will be needed later*
- *If you account was provisioned by WPS staff this step may have been completed*

8. **Navigate to security settings**
   - In **Accounts Center**, click **"Password and security"**
   - Select **"Two-factor authentication"**
   - Choose your profile
   - Select **"Authentication app"** and continue to step 9 *(recommended)*
   - Select **"SMS or WhatsApp"** and continue to step 13
<div style="page-break-after: always;"></div>

### 2FA via Authentication App

9. **Install authenticator app (Recommended)**
   - An authenticator application allows management by multiple people
   - Download Google Authenticator (recommended) or Authy
   - Available on both iOS and Android
   - Multiple staff can use same authenticator for shared account
   - SMS or WhatApp authentication is available to only one phone number

10. **Add new device**
    - Click **"Add"** button
    - *QR code and setup key will appear*
    - *Switch to your phone for next steps*

11. **Configure authenticator app**
    - Open authenticator app on phone
    - Add new account *(+ icon)*
    - Choose **"Scan QR code"** or **"Enter setup key"**
    - Scan QR code from Meta website

12. **Complete setup**
    - Enter descriptive name for this device *(eg WPSVR GAuth or Alex's GAuth)*
    - Input 6-digit code from authenticator app
    - Click **"Done"**
    - *Device now appears in 2FA devices list*

### 2FA via SMS or WhatsApp

- *Only one phone number is allowed for 2FA via SMS or WhatsApp*
- *This will restrict the ability to troubleshoot certain issues should they arise*

13. **Add Phone Number**
    - Change Country code if needed *(defaults to United States)*
    - Enter Phone Number
    - Click **"Next"**
    - Input the 6-digit code sent to the device
    - Click **"Done"**

### Meta Horizon app provisioning

14. **Open the Meta Horizon phone application**
    - Choose **Continue with email**
    - Enter the email used to create the Organization's Meta account *(May be provided by WPS)*
    - Click **"Next"**
    - Choose **"Enter password instead"** *(easier than email code)*
    - Enter your Meta account password *(may be provided by WPS)*
<div style="page-break-after: always;"></div>

15. **Verify account via 2FA (*may be required)***
    - Select 2FA method from dropdown
    - Click **"Next"**
    - Open authenticator application or look for SMS/WhatsApp message
    - Enter 6-digit code
    - Click **"Next"**

16. **Manage login persistence (optional)**
    - Choose whether to save login credentials on this computer
    - *Saving credentials only stores email and password information*
    - *Consider security implications of saved credentials on shared computers*
  
### Setup Meta Horizon account

- *The Meta Horizon account is used excusively for Meta's VR space*
- *Some options will be visible to other Meta Horizon users*

17. **Choose a Meta Horizon username**
    - *This username will be visible to other Meta Horizon users*
    - Enter an accepted username *(a green checkmark will indicate username is valid)*
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
