# Kernel Guidelines:

The following aren't allowed to be added into kernel sources:

- OC/UC/UV, not mattering if it's for display, GPU or CPU.
- Any changes regarding charging voltages.
- Magisk/App Blocker without the need to block toxic modules like FDE.AI. Blocking TikTok/any similar app isn't allowed either.
- Boeffla Wakelock Blocker. Wakelocks exists for a reason. The removal of such ones that are harm for the device is allowed.
- Scheduler restrictions doesn't apply, however that doesn't mean we don't look/care about all possible crappy schedulers you pushed. The same applies for I/O, TCP Schedulers (Backports don't apply to restrictions).
- Prefer giving users less switches to tinker.

Some suggestions would be to:

- Prefer to use init scripts to set default values.
- Changing the default tunable value in the kernel.
- Hardcoding default values isn't recommended.
