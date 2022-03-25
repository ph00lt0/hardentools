# Harden tools
List of tools for hardened operating system security 


## Android
- [GrapheneOS](https://grapheneos.org/) or [DivestOS](https://divestos.org/) for non Pixel phones
- [TrackerControl](https://trackercontrol.org/) (if not using VPN, VPN is preferred)
- [Mull Browser](https://f-droid.org/en/packages/us.spotco.fennec_dos/)
- [Bromite](https://www.bromite.org/)
- [Secure PDF viewer](https://play.google.com/store/apps/details?id=app.grapheneos.pdfviewer.play)
- [Secure Camera](https://play.google.com/store/apps/details?id=app.grapheneos.camera.play)


## Windows
- [HardenTools](https://github.com/securitywithoutborders/hardentools)
- [privacy.sexy](https://privacy.sexy/)
- [WindowsSpyBlocker](https://crazymax.dev/WindowsSpyBlocker/)
- Bitlocker
- [Veracrypt](https://veracrypt.fr) volumns, does not use TPM!
- [NetLimiter](https://www.netlimiter.com/)
- [Local Security Policy](https://www.bleepingcomputer.com/tutorials/create-an-application-whitelist-policy-in-windows/)
- [Windows Defender Application Control management](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/)
  - [Deploy WDAC using Group Policy](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/deploy-windows-defender-application-control-policies-using-group-policy) for individuals
  - [Deploy WDAC using script](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/deployment/deploy-wdac-policies-with-script)
  - [Deploy WDAC using MDM](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/deploy-windows-defender-application-control-policies-using-intune) for businesses
  - [Deploy WCAC using MEMCM](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/deployment/deploy-wdac-policies-with-memcm) for businesses
- Firefox with [arkenfox's user.js](https://github.com/arkenfox/user.js)
- Convert to safe(r) PDFs with [Dangerzone](https://dangerzone.rocks/)


## MacOS
- [Dylib Hijack Scanner](https://objective-see.com/products/dhs.html)
- [KextViewr](https://objective-see.com/products/kextviewr.html)
- [OverSight](https://objective-see.com/products/oversight.html) or [MicroSnitch](https://www.obdev.at/products/microsnitch/index.html)
- [RansomWhere?](https://objective-see.com/products/ransomwhere.html)
- [BlockBlock](https://objective-see.com/products/blockblock.html)
- [Netiquette](https://objective-see.com/products/netiquette.html)
- [ReiKey](https://objective-see.com/products/reikey.html)
- [TaskExplorer](https://objective-see.com/products/taskexplorer.html)
- [KnockKnock](https://objective-see.com/products/knockknock.html)
- [LuLu](https://objective-see.com/products/lulu.html) or [LittleSnitch](https://www.obdev.at/products/littlesnitch/index.html)
- [privacy.sexy](https://privacy.sexy/)
- [Lynsis](https://cisofy.com/lynis/)
- [Santa](https://santa.dev)
- Firefox with [arkenfox's user.js](https://github.com/arkenfox/user.js)
- [Spoof mac address](https://github.com/sunknudsen/privacy-guides/blob/master/how-to-spoof-mac-address-and-hostname-automatically-at-boot-on-macos/README.md)
- [Bluesnooze](https://github.com/odlp/bluesnooze/)
- Convert to safe(r) PDFs with [Dangerzone](https://dangerzone.rocks/)
- [MacOS Security and Privacy Guide](https://github.com/drduh/macOS-Security-and-Privacy-Guide)

### Intel-based Mac
- Enable [Firmware password protection](https://support.apple.com/guide/security/firmware-password-protection-sec28382c9ca/web)
  - Generate a strong password and store it securely. 
  - Run `firmwarepasswd -setpasswd`
  - Run `firmwarepasswd -verify` to make sure you have configured your password right.
  - Run `firmwarepasswd -setmode full` to request password on each boot. `firmwarepasswd -setmode command` for change of boot disk. Do not use `-allow-oroms` unless you really have too. You can always enable this later.
  - Also make sure to run `firmwarepasswd -disable-reset-capability` to disable Apple's ability to reset your device. Nobody will be able to help you if you lose your firmware password!


## GNU/LINUX
- [Lynsis](https://cisofy.com/lynis/)
- LUKS
- [OpenSnitch](https://github.com/evilsocket/opensnitch)
- Firefox with [arkenfox's user.js](https://github.com/arkenfox/user.js)
- Convert to safe(r) PDFs with [Dangerzone](https://dangerzone.rocks/)
- [Linux Hardening Guide](https://madaidans-insecurities.github.io/guides/linux-hardening.html)
- [Encrypted SWAP](https://wiki.archlinux.org/title/Dm-crypt/Swap_encryption) or [ZRAM](https://wiki.archlinux.org/title/Swap#zram-generator)


## Resources:
- Privacy Guides
- Reddit privacy community
- GrapheneOS communities
- Privacy Guides series by Sun Knudsen
- Github
- Stack Exchange
- The Privacy, Security, and OSINT Show by IntelTechniques
