# Kernel Guidelines:

The following aren't allowed to be added into kernel sources:

- OC/UC/UV, not mattering whether it's for display, GPU or CPU.
- Any changes regarding charging voltages.
- Magisk/App Blocker without the need to block toxic modules like FDE.AI. Blocking TikTok/any similar app isn't allowed either.
- Boeffla Wakelock Blocker. Wakelocks exists for a reason. The removal of those that are harmful for the device is allowed.
- Scheduler restrictions don't apply. However, that doesn't mean we don't look/care about all the possible crappy schedulers you pushed. The same applies to I/O, TCP Schedulers (Backports don't apply to restrictions).
- Prefer giving users fewer switches to tinker.

Some suggestions would be to:

- Prefer to use init scripts to set default values.
- Change the default tunable value in the kernel.
- Not recommend hardcoding default values.
