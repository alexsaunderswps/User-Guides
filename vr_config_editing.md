# VR Configuration File Editing Guide

## Purpose & Context
This guide walks you through editing the configuration.json file that controls WildXR application behavior. This file determines video catalogs, startup settings, demo modes, and user interface options. Configuration changes take effect when WildXR restarts.

## Prerequisites
- Completed "VR Headset Basic Connection Guide"
- Values for configuration fields you need to change (see field list below)
- Text editor (Notepad, TextEdit, or code editor)
- **Coordinate with WPS staff if unsure about values**

## Configuration Fields You May Need
Before starting, gather the correct values for:
- **VideoCatalogueName**: Name of video collection to display
- **ForceOfflineMode**: true/false - bypasses internet connectivity checks  
- **DemoMode**: true/false - enables demonstration interface
- **IdleTimerLengthSeconds**: Number - auto-return timeout duration
- **ShowMenuTray**: true/false - displays navigation menu
- **StartupVideoId**: UUID string - specific video to play on launch
- **ResumeStartupVideoOnAwake**: true/false - continues video after sleep
- **StartupVideoLoop**: true/false - repeats startup video

## Quick Overview (for experienced users)
1. Connect headset and access com.wps.wildx/files folder
2. Copy configuration.json to desktop
3. Edit required fields with proper syntax (quotes, commas, boolean format)
4. Save and copy back to headset, overwriting original

## Detailed Steps

### Accessing Configuration File

1. **Complete basic connection**
   - Follow "VR Headset Basic Connection Guide" 
   - Navigate to: Quest > Internal shared storage > Android > data > com.wps.wildx > files

2. **Create working copy**
   - Right-click "configuration.json"
   - Select "Copy"
   - Right-click on Desktop
   - Select "Paste"
   
   *Alternative: Drag configuration.json from headset folder to Desktop*

### Editing Configuration

3. **Open configuration file**
   - Double-click configuration.json on Desktop
   - File opens in default text editor

4. **Edit VideoCatalogueName (if needed)**
   ```json
   "VideoCatalogueName": "Your Catalog Name",
   ```
   - Replace value between quotes
   - Keep quotes and comma

5. **Edit StartupVideoId (if needed)**
   ```json
   "StartupVideoId": "uuid-string-here",
   ```
   - Replace null or existing UUID with new value
   - Keep quotes and comma
   - Use null if no startup video desired

6. **Edit StartupVideoLoop (if needed)**
   ```json
   "StartupVideoLoop": true,
   ```
   - Use lowercase: true or false
   - No quotes around boolean values
   - Keep comma

7. **Edit other fields as needed**
   - Follow same syntax patterns
   - **Strings**: Use "quotes" and comma
   - **Booleans**: Use lowercase true/false, no quotes, keep comma
   - **Numbers**: No quotes, keep comma

### JSON Syntax Requirements
⚠️ **Critical formatting rules:**
- String values must have "double quotes"
- Boolean values: lowercase true or false (no quotes)
- Each line except the last must end with a comma
- Maintain all curly braces { }

### Saving and Deploying

8. **Save changes**
   - File > Save (or Ctrl+S / Cmd+S)
   - Keep filename as configuration.json

9. **Close editor**
   - File > Close or click X

10. **Deploy to headset**
    - Drag configuration.json from Desktop to headset's files folder
    - When prompted, select "Copy and Replace"
    - Confirm overwrite

## Troubleshooting

**WildXR won't start after configuration change:**
- Check JSON syntax: quotes, commas, brackets
- Verify boolean values are lowercase
- Restore backup and try again

**File won't save:**
- Ensure headset is still connected
- Close WildXR completely before editing
- Try copying to different location first

**Values not taking effect:**
- Restart WildXR application completely
- Verify file was actually replaced on headset
- Check that values match expected format

## Validation Checklist
Before deploying configuration:
- [ ] All string values have "double quotes"
- [ ] Boolean values are lowercase true/false
- [ ] Each line ends with comma (except final entry)
- [ ] All brackets { } are intact
- [ ] UUID values are complete and properly quoted

## Important Notes

⚠️ **Always backup**: Copy original configuration.json to safe location before editing

⚠️ **WPS coordination**: Contact WPS staff if unsure about field values, especially UUID strings

⚠️ **Testing**: Test configuration changes immediately after deployment

## Next Steps
After successful configuration:
- Restart WildXR to verify changes
- Test affected functionality (startup videos, menus, etc.)
- Document successful configuration for future reference