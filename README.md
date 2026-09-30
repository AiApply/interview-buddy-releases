# Interview Buddy — Downloads

Official installers for **Interview Buddy**, the desktop interview assistant by [AIApply](https://aiapply.co).

This repository only hosts release files. The installed app also checks it for updates.

## Download

Open the **[latest release](https://github.com/AiApply/interview-buddy-releases/releases/latest)** and download the file for your computer:

| Your computer | File to download |
|---|---|
| Mac with Apple Silicon (M1, M2, M3, M4 or later) | `Interview Buddy-<version>-arm64.dmg` |
| Mac with an Intel processor | `Interview Buddy-<version>-x64.dmg` |
| Windows 10 or 11 (64-bit) | `Interview Buddy-<version> Setup.exe` |

Not sure which Mac you have? Choose  → **About This Mac**. "Chip: Apple M…" means Apple Silicon, "Processor: Intel…" means Intel.

The other files in a release (`.zip`, `.nupkg`, `RELEASES`) are used by the app's automatic updates and don't need to be downloaded.

## System requirements

- **macOS** 14.2 or later is recommended. macOS 13 and 14.0–14.1 are supported with limited system-audio capture.
- **Windows** 10 or 11, 64-bit.
- A microphone, and an internet connection during sessions.
- An [AIApply](https://aiapply.co) account.

## Install

### macOS

1. Open the downloaded `.dmg`.
2. Drag **Interview Buddy** into **Applications**. If macOS asks whether to replace an existing version, choose **Replace**.
3. Open Interview Buddy from Applications and sign in with your AIApply account.
4. When you start your first session, allow **Microphone** and **Screen & System Audio Recording** access. Interview Buddy uses them to transcribe you and the other speaker. macOS may ask you to reopen the app after granting screen recording.

### Windows

1. Run `Interview Buddy-<version> Setup.exe`. It installs and opens the app automatically.
2. Sign in with your AIApply account.

Windows SmartScreen may show "Windows protected your PC" for a new release. The installer is signed by AiApply Ltd; choose **More info** → **Run anyway**.

## Updates

Interview Buddy updates itself. New versions download in the background and install the next time you restart the app. Updates never interrupt a session that's in progress.

## Verifying a download

Every release is code-signed by **AiApply Ltd**. macOS builds are also notarized by Apple. Each release lists SHA-256 checksums in `SHA256SUMS.txt`:

```sh
# macOS
shasum -a 256 "Interview Buddy-<version>-arm64.dmg"
# Windows (PowerShell)
Get-FileHash ".\Interview Buddy-<version> Setup.exe" -Algorithm SHA256
```

## Uninstall

- **macOS:** quit Interview Buddy and move it from Applications to the Trash.
- **Windows:** Settings → Apps → Installed apps → Interview Buddy → Uninstall.

## Help

For questions or problems, open the profile menu at the bottom of the sidebar and choose **Feedback**, or contact AIApply support via [aiapply.co](https://aiapply.co).
