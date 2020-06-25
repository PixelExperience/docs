# Device Requirements

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://tools.ietf.org/html/rfc2119).

1. Device or software exceptions **SHOULD** be made via change request to this repository.

2. The device **MAY** have SELinux Enforcing.

3. The device **MUST** have hardware compatibility comparable to stock ROMs (i.e. if IR blaster works on stock ROMs, it **MUST** work on PE) 
  
4. The device's trees are **REQUIRED** to include some commits listed [here](https://github.com/PixelExperience-Devices/required_commits).

5. The device **MUST** pass SafetyNet out of the box with no modifications.
  
    5.1. If the device's stock fingeprint passes, it **MUST** be used.
    
    5.2. If that device's stock fingerprint does not pass SafetyNet, other devices' fingeprints (e.g. Pixels' fingerprints) **SHOULD** be used.

6. The device **MUST NOT** include, but is not limited to:

    6.1. Packages that are not built, do not work, and/or are obsolete.
  
    6.2. Placebo 'tweaks' and/or packages that contain unnecessary and/or unwanted features, as stated in #6 of [Maintainers' Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).

7. The device's sources **MUST** be in accordance with #6, #7, #8, #9, and #10 (if applicable) as stated in [Maintainers' Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).

8. If the device uses Full Disk Encryption (a.k.a FDE) or uses kernel version 3.18 or below, it **MUSTN'T** ship with Google Play System Updates/Updatable APEX enabled, as it only works on devices that use File-Based Encryption (a.k.a FBE) with encryption enabled, and kernel version later than 3.18. 

9. The device **SHOULD NOT** use a lot of patches.

10. If the device **MUST** use a lot of patches, and/or there are commits needed in repos other than the device-specific's ones, they **MUST**:

    10.1. Be **REQUIRED** for the device to build and/or boot successfully, or to enable a function (i.e. Fingerprint On Display).
  
    10.2. Have proper authorship.

    10.3. Be pushed to [PixelExprience's Gerrit](https://gerrit.pixelexperience.org).

    10.4. Be as minimal and as polished as possible.

    10.5. Be in accordance with #6, #7, #8, #9, and #10 (if applicable) as stated in [Maintainers' Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).
  
## Exceptions
Device(s) | Exception | Until
----------|-----------|-------
All       | VoLTE     |-------
All       | NFC       |-------
