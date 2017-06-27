This repository contains PKGBUILDs from the Arch User Repository
(AUR). I have built most of these packages and uploaded them to
my personal repository.

## Add repository
I am currently hosting the packages on my website. At this time,
I have only compiled the packages on x86_64, but I will probably
also compile these for i686 and ARM architectures at some point.

To install packages from my repository, add this to your pacman.conf:

```INI
# main repository
[n1klas]
SigLevel = Required TrustedOnly
Server = https://repo.n1klas.net/arch/main/$arch

# unstable repository (for -git packages)
[n1klas-unstable]
SigLevel = Required TrustedOnly
Server = https://repo.n1klas.net/arch/unstable/$arch
```

Finally, refresh your pacman cache:

```bash
pacman -Sy
```

All commands must be executed with root privileges.
