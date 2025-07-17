# Configuration Template Guide for IT Support

## Purpose & Context
This guide enables IT support personnel to locate, customize, and distribute pre-configured configuration.json templates for WildXR deployments. Using templates streamlines end-user setup and reduces configuration errors during support sessions.

## Prerequisites
- Access to WPS Google Drive (WPS Team Drive)
- Google account logged in through Chrome or web browser
- Understanding of JSON syntax requirements
- Text editor or IDE for file modification
- End-user specific configuration values

## Quick Overview (for experienced users)
1. Access WPS Team Drive > VR > Trouble Shooting Guides > Templates
2. Download appropriate version template
3. Customize fields for specific end-user deployment
4. Distribute modified template to end-user before/during support session

## Detailed Steps

### Accessing Template Repository

1. **Open Google Drive**
   - Open new browser window
   - Navigate to Google Drive (drive.google.com)
   - Or click 3x3 grid icon in Chrome > Google Drive
   - Ensure logged into WPS Google account

2. **Navigate to shared templates**
   - Click "Shared drives" in left sidebar
   - Double-click "WPS Team Drive"
   - Double-click "VR" folder
   - Double-click "Trouble Shooting Guides" folder
   - Double-click "Templates" folder

3. **Select appropriate template**
   - Template filenames indicate compatible WildXR versions
   - Choose template matching end-user's WildXR installation
   - Select template file

4. **Download template**
   - Click "Download" button
   - File saves to default download location
   - Access via browser download notification

### Customizing Template

5. **Open template for editing**
   - Double-click downloaded configuration.json template
   - Opens in default text editor/IDE
   - Notepad++, VS Code, or similar recommended

6. **Customize key deployment fields**
   - **VideoCatalogueName**: Set to user's video collection name
   - **ForceOfflineMode**: true/false based on connectivity requirements
   - **DemoMode**: true/false for demonstration vs. production use
   - **IdleTimerLengthSeconds**: Numeric value for timeout duration
   - **ShowMenuTray**: true/false for interface preferences
   - **StartupVideoId**: UUID for specific startup video
   - **ResumeStartupVideoOnAwake**: true/false for wake behavior
   - **StartupVideoLoop**: true/false for video repetition

### JSON Syntax Validation

7. **Verify critical formatting**
   - **String values**: Surrounded by "double quotes"
   - **Boolean values**: lowercase true or false (no quotes)
   - **Numeric values**: No quotes required
   - **Line endings**: Comma after each field except last
   - **UUID values**: Complete string with proper quotes

8. **Save customized template**
   - Use descriptive filename: `configuration_[EndUserName].json`
   - Save to easily accessible location
   - Consider desktop or support session folder

### Distribution and Support

9. **Pre-session preparation**
   - Send customized template to end-user via email
   - Include brief explanation of purpose
   - Highlight that this saves time during support session

10. **During support session**
    - Request screen sharing from end-user
    - Verify each field value as they enter it
    - Watch for common syntax errors:
      - Missing quotes around strings
      - Uppercase True/False instead of lowercase
      - Missing commas
      - Incomplete UUID strings

### Quality Assurance Reference

11. **Access reference configuration**
    - Download `configuration_REFERENCE_1.5.json` if needed
    - Contains "vanilla" settings from fresh WildXR installation
    - Use for comparison or restoration purposes

## Common Configuration Scenarios

**New Deployment:**
- DemoMode: false
- ForceOfflineMode: false  
- ShowMenuTray: true
- StartupVideoId: null

**Demo/Kiosk Mode:**
- DemoMode: true
- IdleTimerLengthSeconds: 300
- StartupVideoLoop: true
- ShowMenuTray: false

**Offline Environment:**
- ForceOfflineMode: true
- VideoCatalogueName: "Local Videos"
- Reduced connectivity features

## Troubleshooting Support Issues

**End-user syntax errors:**
- Guide them to check quotes, commas, brackets
- Compare their version to your template
- Use screen sharing to spot errors in real-time

**Values not taking effect:**
- Verify file deployment to headset completed
- Confirm WildXR application restart
- Check that original file was overwritten

**Template won't download:**
- Verify WPS Google Drive access
- Try different browser
- Check organizational permissions

## Important Notes

⚠️ **Template Integrity**: Never edit files directly in Google Drive. Always download, modify, and distribute copies.

⚠️ **Version Compatibility**: Ensure template version matches end-user's WildXR installation.

⚠️ **Validation Support**: Always verify JSON syntax before distributing templates.

⚠️ **Documentation**: Keep records of custom configurations for future reference.

## Support Best Practices

**Pre-session:**
- Prepare customized template in advance
- Verify all required values with end-user
- Have reference configuration available

**During session:**
- Use screen sharing to guide input
- Double-check every character in critical fields
- Test configuration immediately after deployment

**Post-session:**
- Document successful configuration
- Save working template for future use
- Follow up to ensure stable operation

## Next Steps

With template system established:
- Build library of common configuration scenarios
- Train additional support staff on template usage
- Develop automated validation tools for complex deployments
- Create user-specific template archives for repeat support