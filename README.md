These are modules that I include as part of my special build of RattleSnakeOS.
Add the following lines to the end of your '.rattlesnakeos.toml' file.
***
The below are the commands used to execute the build process.
```
rattlesnakeos-stack.exe deploy - deploy .rattlesnakeos.toml
rattlesnakeos-stack.exe build start --force-build - force a build
rattlesnakeos-stack.exe build list - list running builds
```
***

    [[custom-patches]]
    patches = ["00002-microg-sigspoof.patch"]
    repo = "https://github.com/RattlesnakeOS/microg"

    [[custom-prebuilts]]
    modules = ["GmsCore","GsfProxy","FakeStore","com.google.android.maps.jar"]
    repo = "https://github.com/RattlesnakeOS/microg"

    [[custom-patches]]
    patches = [
        "00001-global-internet-permission-toggle.patch",
        "00002-global-sensors-permission-toggle.patch",
        "00003-disable-menu-entries-in-recovery.patch",
        "00004-increase-default-maximum-password-length.patch",
        "00006-do-not-require-strong-auth-on-regular-time-interval.patch",
        "00007-enable_randomize_mac_dev_option.patch",
    ]
    repo = "https://github.com/RattlesnakeOS/community_patches"

    [[custom-prebuilts]]
    modules = [
           "DejaVuNlp","FreedomPop",
           "GoogleVoice","MozillaNlpBackend","NDocs",
           "NetGuard","NetSpeedIndicator","NominatimNlpBackend","OpenKeychain",
           "OpenVPN","SimpleCalendar",
           "TCDrive","TCWebDAV","TCWiFi","Termux",
           "TotalCommander","WiFiPrivacyPolice",
    ]
    repo = "https://github.com/simmule-turner/snake-apps"


# Applications for ROM

## FDroid Open-source
- [x] NetGuard - manage network access (no GSF)
- [x] Nlp - network location provider (unknown)
- [x] OpenKeychain - OpenPGP encryption (no GSF)
- [x] OpenVPN - VPN Software (no GSF)
- [x] Simple Calendar - Calendar application (no GSF)
- [x] Termux - Terminal Emulator (no GSF)
- [x] Wi-Fi Privacy Police - prevents leaking privacy sensitive information via Wi-Fi networks.

## (non) FDroid Open-source
- [x] Total Commander - file manager (Google Drive, WebDAV, WiFi) (no GSF)

## Free Commercial
- [x] Google Voice - Google Voice (no ads) (uses GSF)
- [x] Messaging - FreedomPop application (ads) (uses GSF)
- [x] NDocs - PDF/Office document viewer (uses GSF)
- [x] NetSpeed Indicator - Measure traffic speed (no ads) (no GSF)

***
## Configuration

1. Configure WiFi 
1. Configure microG (device registration, cloud messaging, location providers)
1. Configure FreedomPop
     - goto Settings>Network & internet>Mobile network>Advanced>Access Point Names>+
     - add an APN, FreedomPop, fp.com.attz
     - save the entry
1. Configure "GoogleVoice"
1. Configure "Total Commander"
     - create directory /storage/emulated/0/Documents/data
     - copy configuration files from gdrive://Notes/* to above directory
     - configure applications using this configuration.
1. Install & configure "KeePass DX" from the F-Droid Store
1. Install & configure "Conversations" from the F-Droid Store
1. Configure "NetGuard"
     - configure ad blocking (Optional -- refresh the host file to pickup new additions)
          - Enable Settings>Advanced options>Filter traffic.
          - Enable Settings>Advanced options>Block domain names.
          - Settings>Backup>Download hosts file.
     - configure SOCKS5 vpn (Settings>Advanced options>SOCKS5)
          - Server name: 109.201.154.251 or 46.166.190.172 or nslookup proxy-nl.privateinternetaccess.com
          - Port number: 1080
          - User name: socks-user
          - Password: socks-password
      - configure DNS (Settings>Advanced options>VPN DNS)
           - 9.9.9.9
           - 149.112.112.112
1. Configure DNS (no logging) Setting>Network & internet>Advanced>Private DNS>Private DNS provider hostname
     - add "dns9.quad9.net" and press save
1. Configure the rest of the applications

### Optional
1. Install "Shelter" from F-Droid Store
     - Clone "Chromium" to Work Profile
     - Install & configure other "restricted" applications
       - "Brave Browser" - Yalp Store
       - "Magic Earth" - Yalp Store
       - "Slide" - F-Droid Store
       - "SkyTube" - F-Droid Store
       - "Wallabag" - F-Droid Store
