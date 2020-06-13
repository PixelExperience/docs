# Maintainers conduct notes:

The maintainers:

1 - MUST NOT get involved in arguments or resort to insults, or use hateful words, personal attacks or any other verbal or nonverbal action that is considered detrimental towards the creation of a positive environment for the team.  

2 - MUST upload:

2.1 - All theirs device sources on [PixelExperience-Devices](https://github.com/PixelExperience-Devices) organization. It goes without saying that these should be fully buildable. Using external repos for build releases aren't allowed, unless they're from LineageOS/TheMuppets and Sony Open Devices Project (SODP) organizations. Exceptions may be open if only it's a really big need.

2.2 - Changelogs for each build. These MUST be user-friendly, simplifying the changes for the average user who aren't aware of things like Safetynet or color calibration, but would like to know what has changed since the last update. 

3 - MUST test every build before sending an OTA update to users. Each build must be thoroughly vetted by the maintainer before it is released, and all hardware and software functionalities MUST be tested before a build is released. Releasing untested builds can (and will) lead to your maintainership being revoked.

4 - MUST ship the Standard/Normal Edition builds monthly while shipping the Plus Edition builds is optional. If this is not possible, the reason(s) must be sent to the PE Administration. In the absence of any explanation, a maintainer will be contacted thrice. If there is no satisfactory answer or the administration does not receive a reply, the maintainer will be kicked without any prior warning. 

5 - MUST maintain authorship of git commits that are pushed, this is a mandatory requirement for ALL repositories. Force-pushes are acceptable, but try to keep them to a minimum.

6 - In the event of any disagreements between maintainers, sort them out via direct messages on Telegram or XDA. Do not take your fights to our chats, approach the administration if you want something sorted out quickly. The same is valid for our public chat. "We don't do this here".

7 - MUST NOT add:

7.1 - Any features in their device specific packages, eg. configpanel, XiaomiParts, etc., like KCAL, force Camera API2, etc.

Features that are device specific and are available in stock firmware, eg. Alert Slider and Offscreen gestures for some OnePlus Devices, Fingerprint Gestures and MotoActions for Motorola Devices, are allowed.

Dirac Sound or any audio enhancer is allowed, but it MUST be a device's ROM stock feature, or else it's not allowed. The same must be working fine; otherwise, it can't be shipped.

7.2 - Playground or anything else related to getting Pixel-like features that aren't available from the ROM sources - only GoogleCamera and ARCore are acceptable. 

7.3 - Any Google applications that aren't available from ROM sources - again, only GoogleCamera is acceptable, but please ensure that you use a reliable source and that the device has proper support for them.

7.4 - Any stock firmware camera app. Once again GoogleCamera still acceptable as per se.

8 - MUST NOT ship builds with prebuilt kernels, unless it's the only solution to make the device functional.

9 - MUST NOT do any heavy software modification that may lead to Magisk working properly. If possible, recommend to users to stop using Magisk if it's not working properly.

10 - If maintainer of an A/B partition or a dynamic partition device, then you MUST NOT ship TWRP prebuilt. Instead of TWRP, the maintainer MUST ship the AOSP Recovery available by us.

If any of these rules are broken, the administration will take direct action against the maintainer without prior warning.
