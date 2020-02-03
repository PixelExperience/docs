# Device Requirements

- The device may have SELinux Enforcing to release builds.

- The device must have complete hardware compatibility according with the stock ROM i.e. if IR blaster works on the stock ROM, it must work on PE. VoLTE alone is allowed to be ignored, so does NFC payments methods.

- The device trees must have some required commits. You can check them at [this url](https://github.com/PixelExperience-Devices/required_commits).

- The device must pass SafetyNet out of the box, without any 3rd part mods. Yet custom build fingerprints (eg. Pixels Build fingerprints) aren't allowed if any device stock build fingerprint works to pass SafetyNet.

- The device must not include any unused overlays and packages. This includes but is not limited to packages not being built, packages that doesn't work, obsolete packages, placebo 'tweaks' or any packages that will include unnecessary and/or unwanted features, as stated in the rule #6 at [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).

- The device sources must be in accordance with rules #6, #7, #8 and #9, stated at [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).

- If the device has Full Disk Encyption (a.k.a FDE) mustn't build the Google Play System Updates/Updatable APEX, as the same just works on devices that has File-Base Encryption (FBE). Same for kernel 3.18 or older versions devices.

- The device mustn't have the need of a lot of patches, and if so it must be in accordance with the following item below

- If there're commits that are needed in repos other than the device specific ones, they must:

  - Be necessary for the device to build, boot, or even having a device function working properly (e.g Fingerprint On Display).

  - Have proper authorship.

  - Be pushed to [Gerrit](https://gerrit.pixelexperience.org).

  - Be as minimal and polished as possible.

  - Be in accordance with rules #6, #7, #8 and #9, stated at [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).
  
## Exceptions yet made

Device(s)                                                         | Exception                                            | Until
-----------------------------------------------------------------:|:----------------------------------------------------:|:-------------------
Redmi Note 4/4X (Mido) | Fingerprint: Goodix fingerprint not working          | February 2020
