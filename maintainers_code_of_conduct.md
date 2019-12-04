# Maintainers conduct notes:

The maintainers:

1 - Mustn't insult, use hate words, do personal attacks or any action that is unacceptable towards the creation of a positive environment with the team. 

2 - Mustn't do any unofficial modifications, except if they're going to push it for acceptance on our [gerrit](https://gerrit.pixelexperience.org).
Also, a maintainer mustn't send an update to users with unmerged gerrit changes.

3 - Must upload:

3.1 - Theirs trees on [PixelExperience-Devices](https://github.com/PixelExperience-Devices) organization. The trees should fully reflect the changes when a new build is pushed for that specific device tree(s). Last but not the least, it should be fully buildable.

3.2 - Changelogs for each build. Those must be user-friendly.

4 - Must test every build before sending an OTA update to user.

5 - Must ship the Standard/Normal Edition builds monthly, while the Plus Edition builds are optional. If not possible, the reason(s) must be sent to the head administration. If not given any, maintainers will be contacted 3 times. If no answer given the maintainer will kicked without any previous warns (Take this as your already previous warn).

6 - Must keep authorship of git commits that are pushed, mandatory for all repository. Force-pushes are acceptable.

7 - If there's any relationship fights, those can be done in PM on Telegram or XDA.

8 - Mustn't add:

8.1 - Any features in their device specific packages, eg. configpanel, XiaomiParts, etc., like KCAL, force Camera API2, etc. 

Features that are device specific and are available at stock firmware, eg. Alert Slider and Offscreen gestures for some OnePlus Devices, Fingerprint Gestures and MotoActions for Motorola Devices, are allowed. 

Dirac Sound is allowed, but it must be a device's ROM stock feature or not. The same must be working fine, otherwise it can't be shipped.

8.2 - Custom build fingerprints (eg. Pixels Build fingerprints), unless the reason of having them it's bypass SafetyNet.

8.3 - Playground or anything else related to get Pixel-like features that aren't available from the ROM sources (only GoogleCamera is acceptable).

8.4 - Any Google Application that aren't available from ROM sources (again, only GoogleCamera is acceptable).

9 - Mustn't ship builds with prebuilt kernels, unless it's the only solution to make the device functional.

If any of those rules were broken, there will be an immediate action towards the maintainer
