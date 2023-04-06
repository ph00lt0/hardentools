# Harden tools
List of tools for hardened operating system security 


## Android
- [GrapheneOS](https://grapheneos.org/) or [DivestOS](https://divestos.org/) for non Pixel phones
- [TrackerControl](https://trackercontrol.org/) (if not using VPN, VPN is preferred)
- [Brave](https://brave.com/)
- [Secure PDF viewer](https://play.google.com/store/apps/details?id=app.grapheneos.pdfviewer.play)
- [Secure Camera](https://play.google.com/store/apps/details?id=app.grapheneos.camera.play)
- [Duress](https://github.com/x13a/Duress) Trigger wipe on x length of PIN/password input.
- [Sentry](https://github.com/x13a/Sentry) Trigger wipe after x amount of wrong PIN/password attempts.
- [Wasted](https://github.com/x13a/Wasted) Trigger wipe after x amount of days unused.


## Windows
Configurators:
- [HardenTools](https://github.com/securitywithoutborders/hardentools)
- [privacy.sexy](https://privacy.sexy/)
- [Hard_Configurator](https://github.com/AndyFul/Hard_Configurator)
- [WindowsSpyBlocker](https://crazymax.dev/WindowsSpyBlocker/)

Induvidual settings:
- [Bitlocker](https://docs.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-device-encryption-overview-windows-10)
- [Local Security Policy (application whitelisting)](https://www.bleepingcomputer.com/tutorials/create-an-application-whitelist-policy-in-windows/)
- [Endpoint Device Control Device (external device whitelisting)](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/mde-device-control-device-installation?view=o365-worldwide)
- [Microsoft Defender Application Guard](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-application-guard/install-md-app-guard#install-application-guard)
- [Turn on network protection](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/enable-network-protection?view=o365-worldwide#powershell)
- [Enable virtualization-based protection of code integrity](https://docs.microsoft.com/en-us/windows/security/threat-protection/device-guard/enable-virtualization-based-protection-of-code-integrity#how-to-turn-on-hvci-in-windows-10)
- [Set up and use Microsoft Defender SmartScreen](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-smartscreen/microsoft-defender-smartscreen-set-individual-device)
- [Enable attack surface reduction rules](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/enable-attack-surface-reduction?view=o365-worldwide#powershell)
- [Enable firmware protection](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-system-guard/system-guard-secure-launch-and-smm-protection#windows-security-app)
- [Enable blocking of Potentionally Unwanted Applications](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/detect-block-potentially-unwanted-apps-microsoft-defender-antivirus?view=o365-worldwide#use-powershell-cmdlets-to-configure-pua-protection)
- [Use Windows Sandbox for untrusted applications](https://techcommunity.microsoft.com/t5/windows-kernel-internals-blog/windows-sandbox/ba-p/301849)

Tools:
- Use build-in Microsoft Defender, do not use any other AV
- [Veracrypt](https://veracrypt.fr) volumns, does not use TPM!
- Firefox with [arkenfox's user.js](https://github.com/arkenfox/user.js)
- [Brave](https://brave.com/)
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
- [Brave](https://brave.com/)
- [Spoof mac address](https://github.com/sunknudsen/privacy-guides/blob/master/how-to-spoof-mac-address-and-hostname-automatically-at-boot-on-macos/README.md)
- [Bluesnooze](https://github.com/odlp/bluesnooze/)
- Convert to safe(r) PDFs with [Dangerzone](https://dangerzone.rocks/)
- [MacOS Security and Privacy Guide](https://github.com/drduh/macOS-Security-and-Privacy-Guide)
- [Enable Lockdown Mode](https://images.apple.com/uk/newsroom/2022/07/apple-expands-commitment-to-protect-users-from-mercenary-spyware/)
- [Secretive](https://github.com/maxgoedjen/secretive) SSH-Keymanager
- [SAP Privileges](https://github.com/SAP/macOS-enterprise-privileges) On the fly request admin permissions and keep them disabled during normal usage. 

### Intel-based Mac
- Enable [Firmware password protection](https://support.apple.com/guide/security/firmware-password-protection-sec28382c9ca/web)
  - Generate a strong password and store it securely. 
  - Run `firmwarepasswd -setpasswd`
  - Run `firmwarepasswd -verify` to make sure you have configured your password right.
  - Run `firmwarepasswd -setmode full` to request password on each boot. `firmwarepasswd -setmode command` for change of boot disk. Do not use `-allow-oroms` unless you really have too. You can always enable this later.
  - Also make sure to run `firmwarepasswd -disable-reset-capability` to disable Apple's ability to reset your device. Nobody will be able to help you if you lose your firmware password!


## iOS/iPadOS
- [Enable Lockdown Mode](https://images.apple.com/uk/newsroom/2022/07/apple-expands-commitment-to-protect-users-from-mercenary-spyware/)
- [Use Adguard in Safari](https://apps.apple.com/us/app/adguard-adblock-privacy/id1047223162) no other browsers


## GNU/LINUX
- [Lynsis](https://cisofy.com/lynis/)
- LUKS
- [OpenSnitch](https://github.com/evilsocket/opensnitch)
- Firefox with [arkenfox's user.js](https://github.com/arkenfox/user.js)
- [Brave](https://brave.com/)
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
- Windows11_Hardening by beerisgood
