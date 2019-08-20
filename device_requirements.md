# Device Requirements

- The device may enforce SELinux.

- The device must have working and bug-free:

  - General audio.

  - RIL (phone calls and mobile data). VoLTE is not required in any way.

  - Camera.

  - Bluetooth.

  - NFC if applicable. GooglePay and payments methods that uses NFC aren't required to be working.

  - Fingerprint scanner if applicable.

  - Proximity sensor.

  - WiFi.

- The device trees must have some required commits. You can check them at [this url](https://github.com/PixelExperience-Devices/required_commits).

- The device must not include any unused overlays and packages. This includes but is not limited to packages not being built, obsolete packages, placebo 'tweaks' or any packages that will include unnecessary features, as stated in the rule #8 at [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/pie/maintainers_code_of_conduct.md).

- If there're commits that are needed in repos other than the device specific ones, they must:

  - Be necessary for the device to build, boot, or even having a device function working properly (e.g Fingerprint On Display).

  - Have proper authorship.

  - Be pushed to [Gerrit](https://gerrit.pixelexperience.org).

  - Be as minimal and polished as possible.

  - Be in accordance with rule #8, stated at [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/pie/maintainers_code_of_conduct.md).
  
