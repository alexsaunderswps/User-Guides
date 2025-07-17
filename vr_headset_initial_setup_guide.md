# Quest VR Headset Setup Guide

## Purpose & Context
This guide provides the required steps to setup a Quest VR headset for the first time. 
WPS may have created some needed accounts as part of their internal VR partner program. Check with WPS staff if you are unsure of what accounts your organization needs.
Account creation by WPS is done to facilitate smooth VR operation and increases our ability to provide technical support. 
Accounts created without the help of WPS staff cannot be accessed by WPS staff during technical support sessions.

⚠️ **Meta**: Meta hardware and software (including MQDH) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta releases to inform users of potential impacts and changes.

## Prerequisites
- A WiFi internet connection
- Email account credentials associated with your VR setup *(may be provided by WPS)*
- Smartphone with 2FA app capability
- Smartphone with Meta Horizon application installed
- Initial coordination with WPS staff for first-time login
- VR headsets

## Quick Overview (for experienced users)
1. Meta account is created for Organization *(may be provided by WPS)*
2. User logs into Meta Horizon phone app
3. Developer mode is enable for headset
4. Recommended settings are applied to headset
5. WildXR and Auto Launch *(if desired)* are installed on headset
6. Headset is registered with WildXR Website for remote provisioning
7. Videos are downloaded or side-loaded to improve WildXR performance 

## Detailed Steps

### Meta Account Creation

- *If WPS staff created the Meta Account used to register headsets this step may be complete*

1. **Navigate to Meta**
   - Open web browser and go to `meta.com`

2. **Access login**
   - Click **account icon** *(person silhouette)* in upper right
   - Select **"Sign up or log into a Meta account"**
   - Choose **"Continue with email"**
<div style="page-break-after: always;"></div>

3. **Enter credentials**
   - Click **Continue with Email**
   - Enter Email address associated with your VR setup
   - Click **"Next"**
   - Choose **"Create new account"**
   - Enter your the requested details as needed for account creation
   - Choose a password for your account *(WPS staff will not have access to your password)*
   - Secure your account details (email and password) for future use
   - Click **"Next**

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
   - Click **account icon** again to access account features *(icon is now a circle with a letter or Logo)*
   - Select **"Accounts Center"** for main dashboard

### Two-Factor Authentication

- *Now is a good time to set up two-factor authorization as it will be needed later*

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

13. **Add Phone Number**
    - Change Country code if needed *(defaults to United States)*
    - Enter Phone Number
    - Click **"Next"**
    - Input the 6-digit code sent to the device
    - Click **"Done"**

### Meta Horizon app provisioning

14. **Open the Meta Horizon phone application**
    - Choose **Continue with email**
    - Enter the email used to create the Organization's Meta account
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

*The Meta Horizon account is used excusively for Meta's VR space*
*Some options will be visible to other Meta Horizon users*

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
    - Your headset may apply firmware updates
    - Leave your headset plugged in while updates are downloaded
    - *Your headset may indicate that you can continue setup in the Meta Horizon phone app*
    - ⚠️ **WPS does not recommend you do so and suggests waiting until the headset displays your pairing code**

20. **Pair headset to Meta Horizon phone app**
    - Your headset will display a five digit code
    - Open your Meta Horizon phone app
    - The Meta Horizon app will show the account avatar and a hamburger menu *(three horizontal bars)* on the right side.
    - Open the hamburger menu
    - Under **Device Management** click **Devices**
    - Find the **Pair New Headet** option and click it
    - Select the correct model of Meta headset
    - *You may be prompted to create an avatar - this step is now required by Meta*
    - *This avatar is visible to other Meta Horizon users*
    - Create an avatar and click **"Continue"**
    - Enter the five digit code when prompted
    - Click **"Continue"** when the paring successful screen is shown

21. **Accept disclaimers in Meta Horizon app**
    - Click **"Continue"** on the safety guidelines
    - Click **"Don't Share"** or **"Share"** on the share additional data request
    - Click **"Not now"** on the Enable hand and body tracking request
    - Click **"Skip"** on the Start 3-month trial offer *(This screen may or may not be present)*
    - Click **"Skip"** on the Add a payment method
    - Click **"Close"** on the You're all set! screen

22. **Finish Headset introduction**
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

### 2FA via SMS or WhatsApp
   ⚠️ **2FA via SMS or WhatsApp is only available to one phone number**

12.  **Add Phone Number**
       - Change Country code if needed (defaults to United States)
       - Enter Phone Number
       - Click "Next"
       - Input the 6-digit code sent to the device
       - Click "Done" 

### Account Management Options

13. **Profile management**
       - Access "Profiles" in left sidebar
       - Edit name, username, profile picture, or avatar
       - Changes affect VR headset display

14. **Password changes**
       - In "Password and security", select "Change password"
       - ⚠️ **Always coordinate password changes with WPS staff**

## Troubleshooting

**Cannot access account:**
- Verify Gmail address is correct for your VR setup
- Contact WPS for password assistance
- Ensure you're using work account, not personal

**2FA codes not working:**
- Codes expire after 30 seconds
- Check time synchronization on phone
- Request new code from WPS if needed

**"Add" button greyed out for 2FA:**
- Account may have maximum devices linked
- Contact WPS to remove unused devices
- Some account types have device limits

**Cannot see profile/settings:**
- Ensure you're logged into correct account
- Try logging out and back in
- Clear browser cache if persistent
<div style="page-break-after: always;"></div>

## Important Security Notes

⚠️ **Password Coordination**: Never change passwords without WPS coordination. This prevents technical support lockouts.

⚠️ **2FA Method Choice**: If SMS or Whatsapp was selected as 2FA method WPS will not have access to these messages to assist with account login, device linking, or account recovery.

⚠️ **2FA Device Sharing**: Multiple staff can safely use authenticator apps for same account. Each device gets unique name.

⚠️ **Time Sensitivity**: 2FA codes expire every 30 seconds. Watch countdown timer in authenticator app.

⚠️ **Account Recovery**: WPS maintains master access for account recovery. Don't remove WPS access methods.

## Understanding 2FA Security

**Why 2FA is required:**
- Meta mandates 2FA for most accounts
- Protects against unauthorized access
- Required for enterprise VR deployments

**How codes work:**
- Apps generate time-based codes
- Codes sync with Meta's servers
- Each code valid for 30-second window
- No internet required for code generation

## Next Steps

With Meta account access established:
- Test VR headset connection and pairing
- Verify profile information appears correctly in headset
- Document 2FA setup for other staff members
- Establish backup access procedures with WPS