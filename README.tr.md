<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset=".github/assets/insurup-logo-dark.svg"><img src=".github/assets/insurup-logo.svg" alt="InsurUp" width="360"></picture></p>

# InsurGateway Tunnel desktop app `Stable`

Bu repoda kaynak kod yoktur, yalnızca InsurUp'ın yayın hattının yayımladığı InsurGateway Tunnel masaüstü uygulaması yayın dosyaları (Windows, macOS, Linux) bulunur.

## Kurulum

### Windows

- Kullanıcı başına, yönetici gerekmez: https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest/download/igw-tunnel-user-win-x64-Setup.exe
- Makine geneli, servis ve tepsi, yönetici gerekir: https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest/download/igw-tunnel-win-x64-Setup.exe

### macOS

[Son sürüm sayfası](https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest): `.pkg` yükleyicisi ya da taşınabilir `.zip` (`osx-arm64`, `osx-x64`).

### Linux

[Son sürüm sayfası](https://github.com/InsurUp/insurgateway-tunnel-desktop-release/releases/latest): AppImage `InsurGateway.Tunnel-linux-x64.AppImage`.

## Güncellemeler

Kurulu uygulamalar kendilerini buradaki son sürümden günceller: Windows kullanıcı başına kurulum kendi güncelleyicisiyle, macOS ve Linux Velopack ile. Windows makine geneli kurulum servisle birlikte güncellenir.

## Bütünlük

Windows güncelleme paketi `igw-tunnel-desktop-win-x64.zip` ile macOS ve Linux güncelleme paketleri (`*-full.nupkg`) bir `.sig` taşır: güncelleyicinin paketi uygulamadan önce doğruladığı ECDSA P-256 imzası. Windows dosyalarında `.sha256` vardır; macOS ve Linux dosyalarında yoktur.

<details>
<summary>SHA-256'yı elle denetle</summary>

Dosyalar aynı klasörde. Özet değerleri aynı olmalıdır.

### Windows

```powershell
(Get-FileHash .\igw-tunnel-user-win-x64-Setup.exe -Algorithm SHA256).Hash
Get-Content .\igw-tunnel-user-win-x64-Setup.exe.sha256
```

</details>

## İletişim

https://www.insurup.com
