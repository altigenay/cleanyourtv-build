# CleanYourTV launcher builds

Builds of the launcher from [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) (MIT). The project publishes source only, so this builds it.

A GitHub Actions workflow checks for a new upstream release once a day. When one appears, it builds `launcher/` at that tag, verifies the APK's signing certificate, and publishes a release here with the APK and `latest.json` (version, file, SHA-256, size).

App Pull&Push reads `latest.json` to install or update the launcher on a TV. The APKs are signed with the same key as the copies it installed before, so they install as updates.

All credit for the launcher goes to the CleanYourTV authors; see their repository for the licence, documentation and the debloat tools.
