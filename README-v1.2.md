# Android APK Reverse Engineering Lab

An educational Android security case study that explores how an APK can be inspected, modified, rebuilt, signed, and tested in a controlled emulator. The case study uses a To-Do List app to demonstrate visible, harmless changes and the security implications of APK repackaging.

## What we did

- Inspected the APK structure, manifest, resources, and decompiled code.
- Changed the displayed app name and a visible task-screen message.
- Added a visible startup popup as a controlled behavior change.
- Rebuilt and signed the modified APK with a test key.
- Installed and verified the result in the MEmu Android emulator.

## Tools

APKTool · JADX · ADB · Java JDK / keytool · MEmu Emulator · Windows 11

## Workflow

`Original APK → Static analysis → Resource/smali edits → Rebuild → Test signing → Emulator verification`

## Security lessons

The exercise shows why Android developers should consider code obfuscation, application integrity checks, secure signing, and server-side validation for security-sensitive decisions. Repackaging also changes the app's signing identity.

## Scope

This was a Group 55 academic lab exercise. Changes were limited to visible text and a harmless startup message, and testing took place in an emulator. The repository is intended to document the analysis and results. It is not an original implementation of the To-Do List app.

## Project report

See [`v1.2.pdf`](v1.2.pdf) for the methodology, screenshots, test results, and discussion. If you add the report to this repository under a different name or folder, update this link.

## Team

- Anulasha K.A.
- Abeykoon A.M.A.S.
- Anjana I.K.D.
- Perera L.M.D.

## Responsible use

Perform reverse engineering and modification only on apps you own or are authorized to analyze. Do not redistribute a modified third-party APK without the required rights.
