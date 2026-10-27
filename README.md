# BadgerTV releases

This public repository distributes signed Android TV APKs, release notes and checksums. BadgerTV source is private and is never uploaded here.

No approved stable release has been published yet. Candidate builds still need real Chromecast update testing.

Once a stable release is approved, download [BadgerTV.apk](https://github.com/Roxor11/BadgerTV-Releases/releases/latest/download/BadgerTV.apk) from [Releases](https://github.com/Roxor11/BadgerTV-Releases/releases). Review its release notes and SHA256SUMS. Experimental releases are marked prerelease and are excluded from normal in-app update checks.

Initial installation requires a supported TV browser/downloader or user-driven APK transfer. Android asks you to allow installation from that source and confirm installation. Future updates appear in BadgerTV Settings under Check for Updates, with Android confirmation. ADB and a laptop are not required for routine updates.

BadgerTV uses application ID `tv.badger.app`. Updates must use the same permanent signing certificate and a higher Android version code. An older development installation signed with an Android debug key cannot accept the release certificate as an in-place update; ask the owner about migration before removing anything. Uninstalling can erase saved sign-in and settings.

The app downloads update metadata from the [public latest-release API](https://api.github.com/repos/Roxor11/BadgerTV-Releases/releases/latest), and verifies APK integrity, package, version and signing certificate. Jellyfin credentials are not sent to GitHub. Device policy or Android verification can still prevent installation. Failed/cancelled updates retain the existing app.
