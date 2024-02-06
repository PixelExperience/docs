# Device Requirements

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://tools.ietf.org/html/rfc2119).

Exceptions **SHOULD** be made by contacting the administration team.

- The device **MUST** be using an ARM 64-bit software base.

- The device **MUST** have 3 GB of RAM or more.

- The device **MUST** be using a kernel 4.4 base with eBPF and binder backports, or newer versions of the Linux kernel.

- The device **MUST** have a minimum of 64 GB of internal storage. SD Card expansions **SHALL NOT** be counted as part of it.

- The device **MUST** have a minimum of about 9 GB of dedicated storage for the system partition, already counting proper storage optimizations being taken place. RemovePackages **SHALL NOT** be considered as such.

- The device **MUST** have SELinux Enforcing to release builds. However, during the alpha or beta stage, having SELinux Permissive is allowed.

- The device **MUST** have complete hardware compatibility corresponding to the stock ROM, i.e. if IR blaster works on the stock ROM, it must work on PE. Only VoLTE is allowed to be ignored, so are NFC payment methods.

- The device **MUST NOT** use custom fingerprints (e.g. Pixels Build fingerprints). PixelExperience since its Android 11 release is bypassing SafetyNet without any additional modifications on the device side.

- The device **MUST NOT** include any unused overlays and packages. This includes, but is not limited to, packages not being built, packages that don't work, obsolete packages, placebo 'tweaks' or any packages that will include unnecessary and/or unwanted features, as stated at the [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md).

- The device sources **MUST** be in accordance with, if applicable, all the items stated at our [Maintainers Code of Conduct](https://github.com/PixelExperience/docs/blob/master/maintainers_code_of_conduct.md) related to the device source code.

- The device must be compatible with File Based Encryption (FBE). The exception to this rule is if the device shipped with Full Disk Encryption (FDE) but a proper, working bringup for FBE is in place. Encryption must be enabled by default for all Official builds. 


- The device **SHOULD NOT** have the need for a whole lot of patches, but if so is **REQUIRED**, it **MUST** be in accordance with the following listing below.
- If there are commits that are needed in repos other than the device-specific ones, they **MUST** be in accordance with our [Commit Guidelines](https://github.com/PixelExperience/docs/blob/master/commits_guidelines.md).
 - It **MUST** be necessary for the device to properly function, otherwise such changes will not be accepted. For example: Major changes towards CLO/CAF just for the sake of getting closer to CLO/CAF on the device source.
- All commits on the device side **MUST** be complying with our [Commit Guidelines](https://github.com/PixelExperience/docs/blob/master/commits_guidelines.md).
