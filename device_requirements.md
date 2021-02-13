# Device Requirements

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://tools.ietf.org/html/rfc2119).

Exceptions **SHOULD** be made by contacting the administration team.

- The device **MUST** be using an ARM 64-bit software base. ARM 32-bit devices are no longer supported from our side.

- The device **MUST** have SELinux Enforcing to release builds. During Beta Stage builds it's allowed to have SELinux Permissive.

- The device **MUST** have complete hardware compatibility corresponding to the stock ROM, i.e. if IR blaster works on the stock ROM, it must work on PE. Only VoLTE is allowed to be ignored, so are NFC payment methods.

- The device **MUST NOT** use custom fingerprints (e.g. Pixels Build fingerprints). PixelExperience based on Android 11 is bypassing SafetyNet without any additional modifications on the device side.

- The device **MUST NOT** include any unused overlays and packages. This includes, but is not limited to, packages not being built, packages that don't work, obsolete packages, placebo 'tweaks' or any packages that will include unnecessary and/or unwanted features, as stated at the [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).

- The device sources **MUST** be in accordance with, if applicable, all the items stated at our [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md) related to the device source code.

- If the device has Full Disk Encryption (a.k.a FDE), it **MUST NOT** ship/build the Google Play System Updates/Updatable APEX, as the same only works on devices that have File-Base Encryption (FBE) with the device encrypted. The same is applicable for kernel 3.18 or devices with older kernel versions.

- Yet on the encryption, the device **MUST** always have the encryption enabled and enforced as per stock, not mattering if it's a FDE or FBE device. Converting the device from FDE to FBE is fine, however converting a device from FBE to FDE is strictly prohibited.

- The device **MUST NOT** have the need for a lot of patches, and if so, it must be in accordance with the following listing below.

- If there are commits that are needed in repos other than the device-specific ones, they **MUST**:

  - Be necessary for the device to build, boot, or even to have a/the device's function(s) working properly (e.g. Fingerprint On Display).

  - Have proper authorship.

  - Be pushed to [Gerrit](https://gerrit.pixelexperience.org).

  - Be as minimal and polished as possible.

  - Be in accordance with the items, if applicable, stated at our [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).
