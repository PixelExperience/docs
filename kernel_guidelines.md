# Kernel Guidelines:

The following aren't allowed to be added into kernel sources:

- OC/UC/UV, not mattering whether it's for display, GPU or CPU.
- Any changes regarding charging voltages.
- Magisk/App Blocker. The exception to this would be the need to block toxic modules like FDE.AI. Blocking TikTok/any similar app isn't allowed either.
- KernelSU or any other method to get superuser privileges. 
- Boeffla Wakelock Blocker or any such similar code. Wakelocks exist for a reason. However the removal of those that are harmful for the device are allowed.
- Scheduler restrictions don't apply. However, that doesn't mean you can push any crappy schedulers. The same applies to I/O, TCP Schedulers (Backports don't apply to restrictions).
- Prefer giving users fewer switches to tinker.

Some suggestions would be to:

- Prefer to use init scripts to set default values.
- Change the default tunable value in the kernel.
- Not recommend hardcoding default values.
