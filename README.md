These are modules that I include as part of my special build of RattleSnakeOS.
Add the following lines to the end of your '.rattlesnakeos.toml' file.

    [[custom-prebuilts]]
      modules = [
        "Chronus","CtrlKeyboard","DavX5","DejaVuNlp","DynamicPinAppLock",
        "FolderSync","FreedomPop","GappsBrowser","GoogleVoice","Joplin","KeepassAndroid",
        "LibreOfficeViewer","Maps","MuPDFMini","NominatimNlpBackend","PrivacyBrowser",
        "SimpleCalendar","SkyTube","Slide","SpaRSS","TCDrive",
        "TCDropbox","TCWebDAV","Tasks","TotalCommander","Wallabag","Yalp",
      ]
      repo = "https://github.com/simmule-turner/snake-apps"


# Applications for ROM

## FDroid Open-source
- [x] CtrlKeyboard - Keyboard for terminal/termux
- [x] DavX5 - CalDAV/CardDAV synchronization
- [x] DejaVuNlp - Cell and Wi-Fi based network provider for UnifiedNlp
- [x] GappsBrowser - Sandbox for google web apps
- [x] LibreOfficeViewer - Microsoft Office document viewer
- [x] Maps - Offline OpenStreetMap navigation
- [x] MuPDFMini - document viewer (PDF, CBZ)
- [x] NominatimNlpBackend - backend for MapQuest's geocoding
- [x] PrivacyBrowser - A privacy web browser
- [x] SimpleCalendar - Calendar application
- [x] SkyTube - A YouTube player.
- [x] Slide - Companion app for reddit
- [x] SpaRSS - RSS reader
- [x] Tasks - Task manager that syncs with DavX5
- [x] Wallabag - Read it later app
- [x] Yalp Store - Store to download from Google Play Store

## (non) FDroid Open-source
- [x] Joplin - Note taking application
- [x] Total Commander - file manager (WebDAV, Drive, TotalDrip)

## Free Commercial
- [x] Chronus - Screen widgets (ads)
- [x] Dynamic Pin AppLock - Application locker (no ads)
- [x] FolderSync - Copy files between cloud services (ads)
- [x] GoogleVoice - Google Voice (no ads)
- [x] Messaging - FreedomPop application (ads)

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
1. Install "ProtonVPN" from the Yalp Store
1. Install "NetSpeed Indicator" from the Yalp Store
1. Restart device
1. Configure rest of the applications
