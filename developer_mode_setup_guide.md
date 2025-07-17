# Developer Mode Setup Guide

## Purpose & Context
This guide provides the required steps to authorize a Meta account and headsets associated with that account with developer credentials. 
Developer credentials are required to enable certain features that are needed to resolve connection issues, manage device settings, or troubleshoot VR applications.

## Prerequisites
- An internet connection
- Email account credentials associated with your VR setup *(may provided by WPS)*
- Meta account password *(may provided by WPS)*
- Smartphone with 2FA app capability
- Smartphone with Meta Horizon application downloaded
- Initial coordination with WPS staff for first-time login

## Quick Overview (for experienced users)
1. Organizations's Meta Account is added to WPS Developer group
2. Developer Mode toggled on for each device in Meta Horizon app
3. Developer Mode toggled on in each headset via Advanced Settings

## Detailed Steps

### Initial Developer Authorization

1. **Request WPS Staff to add your Organization's Meta Account to WPS Developer group**
   - *If WPS staff created the Meta Account used to register headsets is step may be complete*
   - *The following steps are best completed during a video call*
   - Send WPS staff Meta account information (**Email address** or **User Name**) requesting Developer access
   - Check email for invitation from WPS and Meta

2. **Accept invitation to join WPS Developer group**
   - Open invitation email
   - Vist the web link included in invitation email *(We recommend using Chrome or Firefox browsers for this step)*

3. **Access login**
   - Click **account icon** *(person silhouette)* in upper right
   - Select **"Sign up or log into a Meta account"**
   - Choose **"Continue with email"**

4. **Enter credentials**
   - Enter Email address associated with your VR setup
   - Click **"Next"**
   - Choose **"Enter password instead"** *(easier than email code)*
   - Enter your Meta account password *(may be provided by WPS)*
   - Click **"Log in"**

5. **Set up two-factor authorization (may be required)**
   - *If you have not enabled two-factor authorization (2FA) for your Meta account you will need to do that now*
   - *See the Meta Account Access and Security Setup Guide for details on enabling 2FA*

6. **Accept invitation and verify authorization** 
   - Accept invitation on Meta web site
   - *An "accept invitation" checkbox should be visible on the webpage*
   - Confirm with WPS staff that the invitation has been accepted and Developer credentials have been authorized

### Enable Developer Mode
2. **Access login**
   - Click account icon (person silhouette) in upper right
   - Select "Sign up or log into a Meta account"
   - Choose "Continue with email"

3. **Enter credentials**
   - Enter Gmail address associated with your VR setup
   - Click "Next"
   - Choose "Enter password instead" (easier than email code)
   - Enter your Meta account password
   - Click "Log in"
<div style="page-break-after: always;"></div>

### Two-Factor Authentication

4. **Complete initial 2FA**
   - Select 2FA method from dropdown (WPS will specify which)
   - Click "Next" 
   - Enter 6-digit code provided by WPS staff
   - Click "Next"

5. **Save login information (optional)**
   - Choose whether to save credentials on this computer
   - Note: 2FA will still be required on future logins

6. **Access account dashboard**
   - You'll return to meta.com main page
   - Click account icon again to access account features (icon is now a circle with a letter or Logo)
   - Select "Accounts Center" for main dashboard

### Setting Up Your Own 2FA Device

*This section enables staff to generate their own 2FA codes*

7. **Install authenticator app (Recommended)**
   - An authenticator application allows management by multiple people
   - Download Google Authenticator (recommended) or Authy
   - Available on both iOS and Android
   - Multiple staff can use same authenticator for shared account
   - SMS or WhatApp authentication is available to only one phone number

8. **Navigate to security settings**
   - In Accounts Center, click "Password and security"
   - Select "Two-factor authentication"
   - Choose your profile
   - Select "Authentication app" and continue to step 9.
   - Select "SMS or WhatsApp" and continue to step 12
  
### 2FA via Authentication App

9. **Add new device**
   - Click "Add" button
   - QR code and setup key will appear
   - Switch to your phone for next steps
<div style="page-break-after: always;"></div>

10. **Configure authenticator app**
       - Open authenticator app on phone
       - Add new account (+ icon)
       - Choose "Scan QR code" or "Enter setup key"
       - Scan QR code from Meta website

11. **Complete setup**
       - Enter descriptive name for this device
       - Input 6-digit code from authenticator app
       - Click "Done"
       - Device now appears in 2FA devices list

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