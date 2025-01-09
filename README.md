# uocr-gentoo-installer
An installer script to use with Gentoo's minimal install CD / admincd, for installing our Gentoo-based distro

Just boot the minimal install CD / admin cd for x86_64 (https://www.gentoo.org/downloads/), and run the script with the block device you want to install Gentoo as an argument, e.g.

```./uocr-gentoo-installer /dev/nvme0n1```

The system needs to support UEFI, have a recent x86_64 CPU (compatible with x86_64_v2 uarch level: https://en.wikipedia.org/wiki/X86-64#Microarchitecture_levels), at least 8G of RAM (although depending on the use case, you'll need at least 16GB, e.g. for the main studio pc) and at least 80G of storage (but that's for playing with VMs, just go for 128/256+ for a decent experience).

You may grab the script via wget (once network is up and running, which should happen automaticaly when you boot the install / admin CD, unless you don't have a DHCP server and use static IPs):

```wget https://raw.githubusercontent.com/UoC-Radio/uocr-gentoo-installer/refs/heads/main/uocr-gentoo-installer```

We don't install systems all the time, so chances are this becomes outdated until the next time we need to setup a system, I've been playing with it for a while and I think it can be usefull for others as well, and the major stuff should be stable-ish so here you go. If you try to use this and hit a wall, please open up an issue.
