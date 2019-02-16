These are modules that I include as part of my special build of RattleSnakeOS.
Add the following lines to the end of your '.rattlesnakeos.toml' file.

    [[custom-prebuilts]]
      modules = [
             "Chronus","CtrlKeyboard","DavX5","DejaVuNlp","FolderSync","FreedomPop","GappsBrowser",
             "GoogleVoice","HackersKeyboard","iAWriter","KeepassAndroid","LibreOfficeViewer","Maps",
             "MuPDFMini","NominatimNlpBackend","PrivacyAppLock","PrivacyBrowser","SimpleCalendar","SimpleTask","SkyTube",
             "Slide","SpaRSS","TCDrive","TCDropbox","TCWebDAV","TotalCommander","Wallabag","Yalp",
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
- [x] Wallabag - Read it later app
- [x] Yalp Store - Store to download from Google Play Store

## (non) FDroid Open-source
- [x] Simpletask - task manager (no cloudsync)
- [x] Total Commander - file manager (WebDAV, Drive, TotalDrip)

## Free Commercial
- [x] Chronus - Screen Wodget (ads)
- [x] FolderSync - Copy files between cloud services (ads)
- [x] GoogleVoice - Google Voice (no ads)
- [x] iA Writer - Markdown editor (no ads)
- [x] KeepassAndroid - password manager
- [x] Messaging - FreedomPop application (ads)
- [x] Privacy AppLock - Application locker and photo

***
## Configuration

1. Configure WiFi 
1. Configure microG (device registration, cloud messaging, location providers)
1. Configure FreedomPop (Settings>Network & internet>Mobile network>Access Point Names>+), FreedomPop, fp.com.attz, Save
1. Configure GoogleVoice
1. Restart device
1. Configure rest of the applications
