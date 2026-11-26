MediaHub TV 0.1 — Android Studio source prototype
Open this folder in Android Studio, install SDK 35 and use JDK 17 / Gradle 8.9. Sync project, then Build > Build APK(s). No Gradle wrapper is bundled; use a local Gradle 8.9 installation or generate wrapper with gradle wrapper --gradle-version 8.9.
APK expected at app/build/outputs/apk/debug/app-debug.apk after successful build.
Install using adb install -r app-debug.apk (after pairing/connecting TV).
M3U: enter authorized playlist URL. Direct: enter HLS/M3U8 or MP4 URL. Xtream: enter server base URL and credentials; imports get.php playlist, not full API.
Prototype only: not compiled or tested here. No EPG, SMB, Stash, Jellyfin, recording or full localization. Credentials and URLs stored in private preferences without encryption; use test credentials only. HTTP enabled for LAN compatibility; prefer HTTPS. Large playlists may be slow. No channels bundled.
