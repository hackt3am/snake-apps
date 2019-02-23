These are modules that I include as part of my special build of RattleSnakeOS.
Add the following lines to the end of your '.rattlesnakeos.toml' file.

    [[custom-prebuilts]]
      modules = [
        "AnySoftKeyboard","AnySoftKeyboardSSH","Chronus","DavX5","DejaVuNlp",
        "DynamicPinAppLock","Firefox","FolderSync","FreedomPop","GappsBrowser","GoogleVoice",
        "Joplin","LibreOfficeViewer","Maps","MuPDFMini","NetSpeedIndicator",
        "NominatimNlpBackend","ProtonVPN","SimpleCalendar","SkyTube",
        "Slide","SpaRSS","TCDrive","TCDropbox","TCWebDAV",
        "Tasks","TotalCommander","Wallabag","Yalp",
      ]
      repo = "https://github.com/simmule-turner/snake-apps"


# Applications for ROM

## FDroid Open-source
- [x] AnySoftkeyboard - Keyboard for terminal/termux (no GSF))
- [x] DavX5 - CalDAV/CardDAV synchronization (no GSF)
- [x] DejaVuNlp - Cell and Wi-Fi based network provider for UnifiedNlp ()
- [x] GappsBrowser - Sandbox for google web apps (no GSF)
- [x] LibreOfficeViewer - Microsoft Office document viewer (no GSF)
- [x] Maps - Offline OpenStreetMap navigation ()
- [x] MuPDFMini - document viewer (PDF, CBZ) (no GSF)
- [x] NominatimNlpBackend - backend for MapQuest's geocoding ()
- [x] SimpleCalendar - Calendar application (no GSF)
- [x] SkyTube - A YouTube player ().
- [x] Slide - Companion app for reddit (no GSF)
- [x] SpaRSS - RSS reader ()
- [x] Tasks - (OpenTasks) Task manager that syncs with DavX5 (no GSF)
- [x] Wallabag - Read it later app (no GSF)
- [x] Yalp Store - Store to download from Google Play Store (no GSF)

## (non) FDroid Open-source
- [x] Joplin - Note taking application (uses GSF)
- [x] Firefox - Web browser (uses GSF)
- [x] Total Commander - file manager (WebDAV, Drive, TotalDrip) (no GSF)

## Free Commercial
- [x] Chronus - Screen widgets (ads) (uses GSF)
- [x] Dynamic Pin AppLock - Application locker (no ads) (uses GSF)
- [x] FolderSync - Copy files between cloud services (ads) (uses GSF)
- [x] GoogleVoice - Google Voice (no ads) (uses GSF)
- [x] Messaging - FreedomPop application (ads) (uses GSF)
- [x] NetSpeedIndicator - Measure traffic speed (no adds) (no GSF)
- [x] ProtonVPN - VPN software (no ads) (no GSF)


***
## Configuration

1. Configure WiFi 
1. Configure microG (device registration, cloud messaging, location providers)
1. Configure FreedomPop
     - goto Settings>Network & internet>Mobile network>Advanced>Access Point Names>+
     - add an APN, FreedomPop, fp.com.attz
     - save the entry
1. Configure GoogleVoice
1. Install "Keypass2Android Password Safe" from the Yalp Store
1. Configure "Firefox" 
     - add user.js (local) or [user.js](https://github.com/pyllyukko/user.js/blob/master/user.js) (privacy tweaks) to /data/data/org.mozilla.firefox/files/mozilla/XXXXXXXX.your_profile_name
     - add Privacy Badger add-on
     - add uBlock Origin add-on
     - add Cookie AutoDelete add-on
     - add HTTPS Everywhere add-on
     - add Decentraleyes add-on
     - add NoScript Security Suite add-on
     - add searx.me add-on
     - configure searx settings>Search>searx.me as the default
1. Configure rest of the applications
