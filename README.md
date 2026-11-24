[🇹🇷 TR](./README.tr.md)

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset=".github/assets/insurup-logo-dark.svg"><img src=".github/assets/insurup-logo.svg" alt="InsurUp" width="360"></picture></p>

# InsurGateway Tunnel desktop app `Stable`

This repository holds no source code, only the InsurGateway Tunnel desktop app release files (Windows, macOS, Linux) that InsurUp's release pipeline publishes.

## Install

### Windows

- Per-user, no administrator needed: https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest/download/igw-tunnel-user-win-x64-Setup.exe
- Machine-wide, service and tray, needs an administrator: https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest/download/igw-tunnel-win-x64-Setup.exe

### macOS

[Latest release page](https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest): the `.pkg` installer or the portable `.zip` (`osx-arm64`, `osx-x64`).

### Linux

[Latest release page](https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest): the AppImage `InsurGateway.Tunnel-linux-x64.AppImage`.

## Updates

Installed apps update themselves from the latest release here: the per-user Windows install through its own updater, macOS and Linux through Velopack. The machine-wide Windows install is updated together with the service.

## Integrity

The Windows update package `igw-tunnel-desktop-win-x64.zip` and the macOS and Linux update packages (`*-full.nupkg`) carry a `.sig`, an ECDSA P-256 signature that the updater verifies before it applies a package. Windows files have a `.sha256`; macOS and Linux files have none.

<details>
<summary>Check the SHA-256 by hand</summary>

Files in the same folder. The hash values must match.

### Windows

```powershell
(Get-FileHash .\igw-tunnel-user-win-x64-Setup.exe -Algorithm SHA256).Hash
Get-Content .\igw-tunnel-user-win-x64-Setup.exe.sha256
```

</details>

## Contact

https://www.insurup.com
