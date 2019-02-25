These are modules that I include as part of my special build of RattleSnakeOS.
Add the following lines to the end of your '.rattlesnakeos.toml' file.

    [[custom-prebuilts]]
      modules = [
        "Chronus","DavX5","DejaVuNlp","DynamicPinAppLock","FreedomPop",
        "GappsBrowser","GoogleVoice","LibreOfficeViewer","Maps","MozillaNlpBackend",
        "MuPDFMini","NetGuard","NetSpeedIndicator","NeutriNote","NominatimNlpBackend",
        "OpenVPN","SimpleCalendar","SkyTube","Slide","SpaRSS",
        "Syncthing","TCDrive","TCDropbox","TCWebDAV","Tasks",
        "Termux","TotalCommander","Wallabag","WiFiPrivacyPolice","YalpStore",
      ]
      repo = "https://github.com/simmule-turner/snake-apps"


# Applications for ROM

## FDroid Open-source
- [x] DavX5 - CalDAV/CardDAV synchronization (no GSF)
- [x] GappsBrowser - Sandbox for google web apps (no GSF)
- [x] LibreOfficeViewer - Microsoft Office document viewer (no GSF)
- [x] Maps - Offline OpenStreetMap navigation ()
- [x] MuPDFMini - document viewer (PDF, CBZ) (no GSF)
- [x] NetGuard - manage network access (no GSF)
- [x] NeutriNote - Note writing application (uses GSF)
- [x] Nlp - network location provider ()
- [x] OpenVPN - VPN Software (no GSF)
- [x] SimpleCalendar - Calendar application (no GSF)
- [x] SkyTube - A YouTube player ().
- [x] Slide - Companion app for reddit (no GSF)
- [x] SpaRSS - RSS reader ()
- [x] Syncthing - file synchronization
- [x] Tasks - (OpenTasks) Task manager that syncs with DavX5 (no GSF)
- [x] Termux - Terminal Emulator (no GSF)
- [x] Wallabag - Read it later app (no GSF)
- [x] WiFiPrivacyPolice - prevents leaking privacy sensitive information via Wi-Fi networks.
- [x] YalpStore - Store to download from Google Play Store (no GSF)

## (non) FDroid Open-source
- [x] Total Commander - file manager (WebDAV, Drive, TotalDrip) (no GSF)

## Free Commercial
- [x] Chronus - Screen widgets (ads) (uses GSF)
- [x] Dynamic Pin AppLock - Application locker (no ads) (uses GSF)
- [x] GoogleVoice - Google Voice (no ads) (uses GSF)
- [x] Messaging - FreedomPop application (ads) (uses GSF)
- [x] NetSpeedIndicator - Measure traffic speed (no adds) (no GSF)


***
## Configuration

1. Configure WiFi 
1. Configure microG (device registration, cloud messaging, location providers)
1. Configure FreedomPop
     - goto Settings>Network & internet>Mobile network>Advanced>Access Point Names>+
     - add an APN, FreedomPop, fp.com.attz
     - save the entry
1. Configure GoogleVoice
1. Install & configure "Keypass2Android Password Safe" from the Yalp Store
1. Configure OpenVPN
1. Install & configure "Firefox" from the Yalp Store
     - add Privacy Badger add-on
     - add uBlock Origin add-on
     - add Cookie AutoDelete add-on
     - add HTTPS Everywhere add-on
     - add Decentraleyes add-on
     - add NoScript Security Suite add-on
     - add CanvasBlocker add-on
     - add searx.me add-on
     - configure searx settings>Search>searx.me as the default
     - configure Firefox:privacy "about:config" tweaks using guide at [privacytools.io](https://www.privacytools.io/)
1. Configure rest of the applications

### Optional
1. Install "Shelter" from F-Droid Store
     - Clone "Chromium" to Work Profile
     - Install & Configure other "restricted" applications
