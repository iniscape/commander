# Iniscape Commander

Two-panel file manager for Linux, macOS and Windows, for people who move
files with the keyboard: two panels side by side, bars above and below,
every action a key away, in a native-grade look, light and dark.

This is a public beta: versions 0.x.y lead up to 1.0.0, which the betas
update to.

## Install

**Linux and macOS**

    curl -fsSL https://github.com/iniscape/commander/releases/latest/download/install.sh | bash

**Windows (PowerShell)**

    powershell -ExecutionPolicy Bypass -c 'irm https://github.com/iniscape/commander/releases/latest/download/install.ps1 -OutFile $env:TEMP\install.ps1; & $env:TEMP\install.ps1'

Requirements: macOS 12 or later on Apple silicon, Linux x86_64 with glibc
2.28 or later (such as Ubuntu 20.04 or RHEL 8 and newer) or Windows 10 or
11 x64.

## Uninstall

Uninstalling removes the app and its settings, log and caches.

**Linux and macOS**

    curl -fsSL https://github.com/iniscape/commander/releases/latest/download/uninstall.sh | bash

**Windows**: Settings → Apps → Installed apps → Iniscape Commander →
Uninstall, or in PowerShell

    powershell -ExecutionPolicy Bypass -c 'irm https://github.com/iniscape/commander/releases/latest/download/uninstall.ps1 -OutFile $env:TEMP\uninstall.ps1; & $env:TEMP\uninstall.ps1'

## Notes

- **Function keys on a Mac** want fn held, unless System Settings →
  Keyboard → *Use F1, F2, etc. keys as standard function keys* is on.
- **Windows 11 Smart App Control** may block a new release from starting,
  since the app is not code-signed yet, most often in the first hours
  after the release is out. Try again later.

## Privacy

Iniscape Commander does not collect, share or sell any personal data.
There is no Iniscape account, and no built-in analytics, telemetry, crash
reporting or advertising of any kind.

The app works on your files where they are. Once a day it asks github.com
whether a newer version is out, sending only its version, unless you
turn that off in Settings; an update is downloaded only when you choose
to install it. Everything else the app keeps, its settings and its log,
stays on your computer. The full statement is in the app: About →
*Privacy*.

## Reporting a bug

Open an issue with the
[bug report form](https://github.com/iniscape/commander/issues/new/choose).
It asks for the version (shown in About), your OS and the log, which is
at:

- macOS: `~/Library/Logs/Iniscape/Commander/commander.log`
- Linux: `~/.local/state/iniscape-commander/commander.log`
- Windows: `%LOCALAPPDATA%\Iniscape\Commander\commander.log`

Feature requests are welcome through the same page. They are read and
noted, then closed, as there is no public backlog. For security issues,
see [SECURITY.md](SECURITY.md).

## Changes

See [CHANGELOG.md](CHANGELOG.md).

## Licence

Copyright (c) 2026 Iniscape. All rights reserved. The Qt libraries that
come with the app are licensed under the LGPLv3; see *Licenses* in the
About dialog, which also lists the other third-party code. The licence
texts come with the app.
