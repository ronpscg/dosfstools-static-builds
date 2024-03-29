# Some dosfstools static prebuilts (linked with glibc)

## Context/Motivation:
Get some important filesystem working tools that busybox does not implement into your ramdisk, easily.
The relevant tools are `fsck.fat`, `fatlabel` and `mkfs.fat`

## Objectives:
Do the same things in the e2fsprogs repo / videos for dosfstools.
- (cross-)Build dosfstools from source code - STATICALLY
- Discuss some annoying configuration issues with autotools
- Discussing common (g)libc issues when you try to just build with your distro tools and autotools
- (cross)-chroot for testing - and discussing what warnings should worry you or what
- reasoning why this entire presentation is a bad practice and you should use build systems and not build things yourself ;-)

## Why does this repo exist?
- Used in the pscg_debos and the pscg_busyboxos examples, useful for others as well
- I sometimes need some tools (fsck.fat, fatlabel, mkfs.fat) as some of the ramdisk/minimal root file system work, and this comes handy

## More info about the why and demonstration of the how (i.e. how to build the resulting binaries)
Short explanations in youtube:
- https://www.youtube.com/watch?v=_F7wJxUteCE
