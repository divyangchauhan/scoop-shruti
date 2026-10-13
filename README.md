# Scoop bucket for Shruti

Shruti is a Windows dictation app with local speech recognition. This bucket
installs the stable x64 portable release, version `1.0.1.0`, matching the published
[Microsoft Store package](https://apps.microsoft.com/detail/9N39R62TTCPS).
The experimental transcript-quality branch is not part of this package.

```powershell
scoop bucket add shruti https://github.com/divyangchauhan/scoop-shruti
scoop install shruti/shruti
```

Start Shruti from its Start menu shortcut or run `shruti`. Windows 10 build 19041
or later is required. Download a speech model in the app before dictation.
Audio and transcription stay on the PC. Settings and models use
`%LOCALAPPDATA%\Shruti`; uninstalling the portable app leaves that data available.
Closing the window keeps Shruti in the tray. Use Exit Shruti to stop it.

The portable executable is unsigned. The Microsoft Store edition uses Store
signing and updates. Both distributions use app version `1.0.1.0`.

```powershell
scoop uninstall shruti
```

The manifest pins a versioned GitHub ZIP and its SHA256. Update it only after
confirming the matching version is published in Microsoft Store. There is no
automatic update to an experimental or not-yet-published Store version.

Source and releases: [divyangchauhan/Shruti](https://github.com/divyangchauhan/Shruti).
