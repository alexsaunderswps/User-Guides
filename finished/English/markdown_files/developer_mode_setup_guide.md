# Developer Mode Setup Guide

## Purpose & Context
This guide provides the required steps to authorize a Meta account and headsets associated with that account with developer credentials. 
Developer credentials are required to enable certain features that are needed to resolve connection issues, manage device settings, or troubleshoot VR applications.

⚠️ **Third Party Software**: Third Party hardware and software (Meta, ArborXR) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta and ArborXR releases to inform users of potential impacts and changes.

## Prerequisites
- An internet connection
- Email account credentials associated with your VR setup *(may be provided by WPS)*
- Meta account password *(may be provided by WPS)*
- Smartphone with 2FA app capability
- Smartphone with Meta Horizon application installed
- Initial coordination with WPS staff for first-time login
- VR headsets

## Quick Overview (for experienced users)
1. Organizations's Meta Account is added to WPS Developer group
2. Developer Mode toggled on for each device in Meta Horizon app
3. Developer Mode toggled on in each headset via Advanced Settings

## Detailed Steps

### Initial Developer Authorization

1. **Request WPS Staff to add your Organization's Meta Account to WPS Developer group**
   - *If WPS staff created the Meta Account used to register headsets this step may be complete*
   - *The following steps are best completed during a video call*
   - Send WPS staff Meta account information (**Email address** or **User Name**) requesting Developer access
   - WPS staff will invite account to join organization as a Developer
   - Check email for invitation to Meta Quest Developer Dashboard from Meta Horizons

2. **Accept invitation to join WPS Developer group**
   - Open invitation email
   - Click **"View Invitation"** - a web link will open - *(We recommend using Chrome or Firefox browsers for this step)*
<div style="page-break-after: always;"></div>

3. **Enter credentials**
   - Click **Continue with Email**
   - Enter Email address associated with your VR setup
   - Click **"Next"**
   - Choose **"Enter password instead"** *(easier than email code)*
   - Enter your Meta account password *(may be provided by WPS)*
   - Click **"Log in"**

4. **Two-factor authorization (may be required)**
   - *If you have not enabled two-factor authorization (2FA) for your Meta account you will need to do that now*
   - *See the Meta Account Access and Security Setup Guide for details on enabling 2FA*
   - *If your account was created by WPS staff you will need to coordinate access*

5. **Accept invitation and verify authorization** 
   - Accept invitation on Meta web site
   - *An "accept invitation" checkbox should be visible on the webpage*
   - Confirm with WPS staff that the invitation has been accepted and Developer credentials have been authorized

### Connect Headset to Meta Horizon phone application

6. **Power on VR headset**
   - *The following steps assume that the VR headset has been initially setup*
   - *If this is not the case - see **VR Headset Initial Setup Guide** for required steps*
   - Connect VR headset to internet
   - *It is best to have only one headset powered on at a time*

7. **Open Device Options**
   - Open the Meta Horizon phone application
   - *The account used for the VR headset must be the same used for the Meta Horizon account*
   - The Meta Horizon app will show the account avatar and a hamburger menu *(three horizontal bars)* on the right side.
   - Open the hamburger menu
   - Under **Device Management** click **Devices**

8. **Connect to device**
   - *You may see multiple devices listed* 
   - One device should show a green circle and be listed as **"Nearby"**
   - Click the **Nearby** device
   - A new screen shows device details and four **Manage your device** options
<div style="page-break-after: always;"></div>

9. **Toggle on Developer Mode**
    - Click on **Headset Settings** - *(may be obscured by Manage profiles notification)*
    - You should see a number of options under **Headset settings**
    - Click on **Developer Mode**
    - Toggle on the **Developer Mode** switch

### Enable Developer settings on VR headset

- *You will be wearing the VR headset for the next steps*
- *For detailed instructions on accessing the Settings menu see - **Recommended Headset Settings***

10. **Open the Advanced Settings menu**
    - Open the **Quick Settings** menu by clicking on the time/WiFi/battery display
    - Click **Settings** on the top right
    - On the left, scroll down to find **Advanced Settings**
    - Click on the **Advanced Setting** option

11. **Toggle on Developer Mode**
    - Scroll down to find **Developer** section
    - Toggle on **Enable Developer Settings**
    - An additional list of options should appear
    - Toggle on **Enable MTP Notification**
    - Toggle off **Physical Link Features**
    - Toggle off **Link Auto-Connect**

## Troubleshooting

**No Invitation Email received from WPS**
- Coordinate with WPS staff prior to sending follow up email
- Verify the Email address sent to WPS staff
- Check your spam folder

**Unable to log into Meta account**
- Verify the correct Email for the Meta account
- When logging in, use email code instead of password to confirm account match
- Ensure password is correct for account 
- If Meta account was created by WPS, coordinate further troubleshooting with staff

**Two-factor authorization issues**
- If account was created by WPS, coordinate or receive 2FA access *(usually Google Authenticator)*
- Ensure you are choosing the correct method for 2FA *(if multiple options exist)*
- WPS staff will be unable to assist with 2FA via phone or SMS
<div style="page-break-after: always;"></div>

**Unable to accept invitation to join Organization**
- Ensure Meta account matches Email address on invitation
- Attempt to accept invitation using Chrome or Firefox browsers - *(Safari has caused issues in the past)*

**Unable to find Device in Meta Horizon app**
- Ensure both VR headset and phone are using the same internet source
- Verify that VR headset and phone are logged in with same Meta account
- Restart both headset and Meta Horizon app
- To reduce possible confusion, ensure that only one VR headset is powered on

**Multiple Devices show as **Nearby** in Meta Horizon app**
- Turn off other nearby Devices to simplify setup
- Match serial numbers *(serial number is found on left temple on headset)*
- *Serial number is on inside of left temple - Quest 3*
- *Serial number is on outside of left temple, under head-strap cover - Quest 2*

**Developer Mode not available in Meta Horizon app**
- Ensure that Meta account has been added to WPS Organization as developer
- Log out of Meta Horizon app and log back in
- Verify the correct Meta account is being used in Meta Horizon app

**Developer Mode toggle does not stay on in Meta Horizon app**
- Verify that Meta account has been added to WPS Organization as developer
- Ensure correct Meta account is being used in Meta Horizon app
- Check VR headset for warning dialog or action messages

**Developer Settings not seen in Advanced Settings on headset**
- Verify headset has had Developer Mode toggled on in Meta Horizon app
- Restart VR headset
- Check headset for pending updates - *(apply any pending updates)*

## Important Notes

⚠️ **WPS Organization Invite**: Coordination of this step is required prior to any further Developer account settings

⚠️ **Account Consistency**: Meta accounts must match between the Meta Horizon application and the VR headset.

