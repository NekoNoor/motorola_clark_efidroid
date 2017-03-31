# efidroidfiles

# [EFIDroid] Device port stability checklist
- [ ] \(obvious\) do LK, UEFI, linux and recovery boot?
- [ ] does UEFI pass the same memory map as the stock bootloader?
- [ ] does UEFI pass the correct cmdline to linux kernels? (/proc/cmdline)
- [ ] does UEFI apply the correct FDT patches? (use build/tools/diffatags)
- [ ] do stock ROM's boot?(they can use custom image formats)
- [ ] does UEFI recognize the SDcard?
- [ ] does UEFI recognize the SDcard when booting from a power-off state?
- [ ] verify that booting both internal and multiboot ROM's via UEFI doesn't give more selinux denials than with the stock bootloader
- [ ] verify that recovery does work correctly (can all partitions be mounted?)
- [ ] verify that EFIDroid works in all possible configurations (bootloaders, ROM's). You must not force users to do/install anything before using EFIDroid.
