# Identification
## Determine OS
- Red Hat
- Debian
- BSD
- Sun OS / Solaris
- Windows
  - `winver`
  - `systeminfo`
  - `wmic os get caption`
  - `powershell "(Get-CimInstance Win32_OperatingSystem).Caption"`
- Apple
## Determine Current User
## Examine Privileges
## Is System Domain Joined?
## Check Running Services
- Red Hat
- Debian
- BSD
- Sun OS / Solaris
- Windows
  - `net start`
  - `wmic service get name,displayname,startmode`
  - `powershell "Get-Service | Where-Object { $_.Status -eq 'Running' }"`
- Apple
## Check Open Ports
- Red Hat
  - `netstat -tunlp`
- Debian
  - `netstat -tunlp`
- BSD
  - `sockstat -l`
- Sun OS / Solaris
- Windows
  - `netsh -ano`
- Apple
## Check Running Applications
# Authentication Bypass
- Cisco (Switches/Routers)
  - https://www.networkstraining.com/cisco-router-password-recovery-how-to-recover-cisco-router-lost-password/
- Cisco (ASA)
  - https://community.cisco.com/t5/security-documents/asa-password-recovery/ta-p/3126046
- Red Hat Based OS
  - RHEL 5 (GRUB)
    - https://web.mit.edu/rhel-doc/5/RHEL-5-manual/Installation_Guide-en-US/s1-rescuemode-booting-single.html
  - RHEL 6 / CensOS 6 (GRUB)
    - https://www.thegeekdiary.com/centos-rhel-6-how-to-boot-into-single-user-mode/
  - RHEL 7 / CentOS 7 (GRUB)
    - https://www.linuxtechi.com/boot-rhel-7-centos-7-server-single-user-mode/
  - RHEL 8 (GRUB and LILO)
    - http://www.src.wits.ac.za/groups/psi/linux/rhl-cg-en-8.0/s1-rescuemode-booting-single.html
  - RHEL 9? (GRUB and LILO)
    - https://www.linux.co.cr/distributions/review/2003/red-hat-9/rhl-cg/s1-rescuemode-booting-single.html
- Debian Based OS
- BSD Based OS
- Sun OS / Solaris
- Windows
  - 2000, XP, 2003, 2003 R2, Vista, 2008, 7, 2008 R2, 8, 2012, 8.1, 2012 R2, 10, 2016, 2019
    - Use Hiren's Boot CD to run Kon-Boot (32-bit OS only)
    - https://www.hirensbootcd.org/hbcd-v106/
  - XP
    - https://www.makeuseof.com/tag/5-tips-to-help-you-reset-a-forgotten-windows-xp-password/
    - Vista, 2008, 7, 2008 R2, 8, 2012, 8.1, 2012 R2, 10, 2016, 2019
- Apple
  - Mac OS X Mavericks / Mountain Lion
    - http://osxdaily.com/2011/08/24/reset-mac-os-x-10-7-lion-password/
