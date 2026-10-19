# PlantCare Rover for Android

PlantCare Rover is the remote control for the PlantCare Rover, an ESP32-CAM plant care robot:
a live camera view, joystick or arrow-button driving, fertilizer and herbicide pumps you switch
on and off from the phone, the flashlight, and a STOP ALL button that turns everything off at once.

This repository only hosts the **Android app downloads and updates**. The source code is kept in
a private repository.

## Download

| | |
|---|---|
| **Newest release page** | [Latest release](https://github.com/adam-ctrlc/plantcare-rover-releases/releases/latest) |
| **All releases** | [Releases](https://github.com/adam-ctrlc/plantcare-rover-releases/releases) |
| **Requirements** | Android 7.0 or newer |

Not every release contains an APK: small updates are delivered inside the app (see
[Updates](#updates)). To install PlantCare Rover for the first time, use the newest release that
lists a `plantcare-rover-vX.Y.Z.apk` file under **Assets**.

## Install

1. On your Android phone, open the newest release that has an APK and tap the
   `plantcare-rover-vX.Y.Z.apk` file.
2. When the download finishes, tap the file to open it.
3. The first time, Android asks to allow installs from your browser. Tap **Settings**, switch on
   **Allow from this source**, then go back and tap **Install**.
4. Turn on the rover and join its Wi-Fi, **ESP32-CAM Robot**. If Android says the network has no
   internet, choose to stay connected (or turn off mobile data).
5. Open PlantCare Rover and tap **Take control**.

Already have PlantCare Rover? Install the new APK over it the same way; your settings stay.

## Updates

PlantCare Rover checks for a new version every time you open it while the phone has internet (the
rover's own Wi-Fi has none, so updates arrive when you're on mobile data or another Wi-Fi).
Updates are required: when one is out, an **Update required** screen lists what's new.

- **Most updates download inside the app.** Tap **Update now**, wait a few seconds, and PlantCare
  Rover restarts on the new version. Only the changed files are downloaded, with no reinstall.
- **Occasionally a new app version (APK) is needed**, when Android-level parts of the app change.
  The update screen then offers a **Download** button for the new APK; install it over the old one.

If a new version ever fails to start, PlantCare Rover goes back to the last version that worked by
itself.

## What's in a release

- `latest.json`: what the app reads to find updates (version, release notes, file list).
- `f-<hash>` files: the app's files, each named by its content hash, so phones only download
  what changed.
- `plantcare-rover-vX.Y.Z.apk`: the Android app, on releases that need one.
