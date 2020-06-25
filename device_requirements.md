# Device Requirements

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://tools.ietf.org/html/rfc2119).

Exceptions **SHOULD** be made by contacting the administration team.

The device:

- **MUST** 
 
  - Have the device's buildable sources uploaded to [PixelExperience-Devices](https://github.com/PixelExperience-Devices) organization. 
  
  - Have hardware compatibility comparable to stock ROMs.
    
  - Include some commits listed [here](https://github.com/PixelExperience-Devices/required_commits) in device's trees.
    
  - Ship builds with AOSP recovery available by us if the device uses A/B or dynamic parition layout.
    
  - Pass SafetyNet out of the box with no modifications. Other devices' fingerprint **SHOULD** be used if stock device's fingeprint does not pass SafetyNet.

- **MUST NOT**

  - Ship builds with Google Play System Updates/Updatable APEX if the device uses kernel version 3.18 or below, or uses Full Disk Encryption (a.k.a FDE).
    
  - Ship builds with pre-built kernels.
    
  - Ship builds with pre-built TWRP if the device uses A/B partition or dynamic parition layout.

  - Include any features in device-specific packages (i.e. configpanel, XiaomiParts, ...) or any stock firmware camera apps that are not available from the ROM sources.
    
  - Include any Google applications or similar applications to getting Pixel-like features that are not available from the ROM sources.
    
  - Include any stock firmware camera app.

  - Include packages that are not built, do not work, and/or are obsolete.
  
  - Include placebo 'tweaks' and/or packages that contain unnecessary and/or unwanted features.
    
  - Include heavy software modification that may lead to Magisk working improperly.
 
- **SHOULD**  <br>

  - Have SELinux Enforcing.

- **SHOULD NOT** <br>

   - Contain a lot of patches. 
    
# Patches

If the device requires patches to a repo others than the device's specific ones, **MUST** make a patch submitting to [PixelExprience's Gerrit](https://gerrit.pixelexperience.org) and have the following qualities:

- Be **REQUIRED** for the device to build and/or boot successfully, or to enable a function (i.e. Fingerprint On Display).
  
- Have proper authorship.

- Be as minimal and as polished as possible.

- Be in accordance with all the requirements above.

# Exceptions
Device(s)        | Exception(s)                          | Until | Notes
-----------------|---------------------------------------|-------|-------------------------------------------------------------------------------------
All              | VoLTE & NFC                           |       |
All              | Sources Upload                        |       |Must be from LineageOS, TheMuppets or Sony Open Devices Project (SODP) organizations.
All              | Pre-built kernels                     |       | Only for devices unable to boot without using pre-built kernels.
Xiaomi Devices   | Dirac Sound & XiaomiParts             |       |
OnePlus Devices  | Alert Sliders & Offscreen Gestures    |       |
Motorola Devices | Fingerprint Gestures & MotoActions    |       |

Software(s)      | Device(s) Exempted | Until | Notes 
-----------------| -------------------|-------|--------
Google Camera    | All                |       | Allowed
ARCore           | All                |       | Allowed
