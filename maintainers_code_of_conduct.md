# Maintainers conduct notes:

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://tools.ietf.org/html/rfc2119).

The maintainers:

- **MUST NOT** get involved in arguments or resort to insults, or use hateful words, personal attacks or any other verbal or nonverbal action that is considered detrimental towards the creation of a positive environment for the team.  

- **MUST** upload:

  - All theirs device sources on [PixelExperience-Devices](https://github.com/PixelExperience-Devices) organization. It goes without saying that these should be fully buildable. Using external repos for build releases aren't allowed, unless they're from LineageOS/TheMuppets organization(s). Exceptions may be open if only it's absolutely necessary.

  - Changelogs for each build. These MUST be user-friendly, simplifying the changes for the average user who aren't aware of things like Safetynet or color calibration, but would like to know what has changed since the last update. 

- **MUST** test every build before sending an OTA update to users. Each build must be thoroughly vetted by the maintainer before it is released, and all hardware and software functionalities MUST be tested before a build is released. Releasing untested builds can (and will) lead to your maintainership being revoked.

- **MUST** ship the Standard/Normal Edition builds monthly while shipping the Plus Edition builds are optional. If this is not possible, the reason(s) must be sent to the PE Administration. In the absence of any explanation, a maintainer will be contacted thrice. If there is no satisfactory answer or the administration does not receive a reply, the maintainer will be kicked without any prior warning. 

- **MUST** maintain authorship of git commits that are pushed, this is a mandatory requirement for ALL repositories. Force-pushes are acceptable, but try to keep them to a minimum.

- **MUST** be active in the development during the maintainship of the device they are responsible for, whether this being a main maintainer or a co-maintainer. If this is not possible, the reason(s) must be sent to the PE Administration. In the absence of any explanation, the member, whether a maintainer or a co-maintainer, will be kicked without any prior warning. Contributions on the ROM side will be taken in consideration in case they are needed.

- In the event of any disagreements between maintainers, sort them out via direct messages on Telegram or XDA. Do not take your fights to our chats, approach the administration if you want something sorted out quickly. The same is valid for our public chat. "We don't do this here".

- **MUST NOT** add:

  - Exclude packages (A.K.A RemovePackages) that includes any package provided by the ROM side without any prior approval from the administration.

  - Any sort of script that will remove any package provided by the ROM side without any prior approval from the administration.

  - Any features in their device specific packages, eg. configpanel, XiaomiParts, etc., like KCAL, force Camera API2, etc.

    Features that are device specific and are available in stock firmware, eg. Alert Slider and Offscreen gestures for some OnePlus Devices, Fingerprint Gestures and MotoActions for Motorola Devices, are allowed.

    Dirac Sound or any audio enhancer is allowed, but it MUST be a device's ROM stock feature, or else it's not allowed. The same must be working fine; otherwise, it can't be shipped.

  - Playground or anything else related to getting Pixel-like features that aren't available from the ROM sources - only GoogleCamera and ARCore are acceptable. 

  - Any Google applications that aren't available from ROM sources - again, only GoogleCamera is acceptable, but please ensure that you use a reliable source and that the device has proper support for them.

  - Any stock firmware app. Once again GoogleCamera is acceptable per se, so is the camera app from the stock firmware itself, only, if fully functional.

- **MUST** use the same device common-tree if a device is already using the same repository. Different branches are not allowed. In case the maintainer doesn't want to use the same common-tree, the only option remaining will be to fully decommonize the device in question. The same goes for the vendor repositories.

- **MUST NOT** enable the Always On Display in case the device has a LCD panel.

- **MUST**, for kernels, follow our [Kernel Guidelines](https://github.com/PixelExperience/docs/blob/master/kernel_guidelines.md).

- About Magisk, the maintainers **MUST NOT**:

  - Do any heavy software modification that may lead to Magisk working properly. If possible, recommend to users to stop using Magisk if it's not working properly.

  - Do any modifications that may lead to Magisk not work, as per the [Kernel Guidelines](https://github.com/PixelExperience/docs/blob/master/kernel_guidelines.md).

- If you're a maintainer of an A/B partition or a dynamic partition device, you **MUST NOT** ship TWRP prebuilt. Instead, the maintainer **MUST** ship the AOSP Recovery made available by us.

- About proprietary files, the maintainers **MUST**:

  - Have a working proprietary files list and extraction script that inherits the global extraction script (located in tools/extract-utils) in their device tree (or device tree dependencies).

  - Use only the script generated vendor repositories for build.

  - Specify the source of any un-pinned (default) proprietary files.

  - Pin any proprietary files not sourced from the default specified source and have a short comment specifying their source. 

- About Translations, the maintainers **MUST**:

  - Move all required strings for any custom packages for device (XiaomiParts, OnePlus Settings, Doze) in [devicesettings](https://github.com/PixelExperience/packages_resources_devicesettings) repository.

- About Sepolicy Rules, the maintainers **MUST NOT**:

  - Ignore Sepolicy Neverallows.

  - Allow write access to generic directory/file/prop labels (With some exceptions).

If any of these rules are broken, the administration will take direct action against the maintainer without prior warning.
