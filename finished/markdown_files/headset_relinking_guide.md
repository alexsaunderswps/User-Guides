# VR Headset Meta Account Relinking Guide

## Purpose & Context
This guide addresses the process of reconnecting a VR headset to its associated Meta account when the link has been broken or lost. Account relinking becomes necessary when headsets lose their connection to Meta's authentication servers, which can occur after extended offline periods, system updates, or account security changes.

⚠️ **Meta**: Meta hardware and software (including MQDH) are outside WPS control. Meta updates may cause unexpected functionality changes in VR systems. WPS monitors Meta releases to inform users of potential impacts and changes.

## Prerequisites
- Stable internet connection for both computer and VR headset
- Email account credentials associated with your VR setup *(may be provided by WPS)*
- Meta account password *(may be provided by WPS)*
- **If you have completed "Meta Account Access and Security Setup Guide":**
  - Smartphone with configured 2FA authenticator app
  - Access to your previously configured authentication device
- **If you have NOT completed "Meta Account Access and Security Setup Guide":**
  - Immediate coordination with WPS staff for real-time 2FA code provision
  - Scheduled time with WPS support for guided authentication process

## Quick Overview (for experienced users)
1. Navigate to `meta.com/device` and authenticate with Meta account credentials
2. Complete 2FA verification using your configured device or WPS-provided code
3. Enter the eight-character verification code displayed in the VR headset interface
4. Confirm successful relinking and test account-dependent features

## Detailed Steps

### Accessing Meta's Device Management Interface

1. **Navigate to device management portal**
   - Open web browser and go directly to `meta.com/device`
   - *This specialized URL takes you directly to Meta's device management interface*
   - *Avoid using the general meta.com site as it requires additional navigation steps*

2. **Initiate account authentication**
   - Select **"Continue with email"** from the available login options
   - *This method provides the most reliable authentication path for account management tasks*
<div style="page-break-after: always;"></div>

3. **Complete primary authentication**
   - Enter the Email address associated with your VR setup
   - Click **"Next"** to proceed to password verification
   - Choose **"Enter password instead"** *(easier than email code)*
   - Enter your Meta account password *(may be provided by WPS)*
   - Click **"Log in"** to proceed to two-factor authentication

### Completing Two-Factor Authentication

4. **Handle 2FA verification**
   - System presents dropdown menu for available 2FA methods
   - Select the method you have previously configured or as directed by WPS staff
   - Click **"Next"** to proceed to code entry
   - Enter the six-digit authentication code from your authenticator app
   - *If you haven't configured personal 2FA, use the code provided by WPS staff during your scheduled support session*
   - Click **"Next"** to complete authentication

5. **Manage login persistence (optional)**
   - Choose whether to save login credentials on this computer
   - *Saving credentials only stores email and password information*
   - *2FA verification will still be required for future login sessions*
   - *Consider security implications of saved credentials on shared computers*

6. **Locate headset verification code**
   - Put on your VR headset or check its display
   - *If a relink code is needed, generally nothing else will be shown in the headset*
   - *This code is unique to this session and expires after a reasonable time period*
   - *Note the code carefully as it is case-sensitive and must be entered exactly*

7. **Enter verification code**
   - Return to the Meta device management interface on your computer
   - Confirm that the correct Meta account information is displayed
   - Enter the eight-character code from your headset into the designated field
   - *Double-check each character before proceeding as incorrect entry requires starting over*
   - Click **"Continue"** to initiate the relinking process

8. **Verify successful connection**
   - System should display confirmation that your device has been reconnected
   - The headset should show updated account status information
   - Meta account features should become available immediately in the headset interface
<div style="page-break-after: always;"></div>

## Troubleshooting

**Authentication fails repeatedly:**
- Verify Gmail address matches VR setup account
- Confirm password accuracy with WPS staff
- Check that account has developer privileges enabled
- Ensure 2FA codes are current (30-second expiration)

**Eight-character code not accepted by Meta interface:**
- Verify web and headset Meta accounts match
- Confirm eight-digit code entered correctly
- Restart headset to refresh code

**Relinking appears successful but account features remain unavailable:**
- Allow time for account to relink
- Restart the headset

## Important Notes

⚠️ **Password Coordination**: Never attempt to change Meta account passwords independently. Always coordinate password modifications with WPS staff to prevent technical support lockouts and ensure that all related systems receive necessary updates.

⚠️ **Account Consistency**: The Meta account used for relinking must exactly match the account originally configured on the headset. Using different accounts, even if they belong to the same organization, will create persistent access issues.

⚠️ **Security Timing**: 2FA codes are time-sensitive. 2FA codes expire every 30 seconds.

