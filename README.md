# Texel Forge Downloads

Official installers and automatic-update packages for [Texel Forge](https://texelforge.com/), a desktop toolkit for preparing textured models and images for multicolor 3D printing.

## Download Texel Forge

Open [Releases](https://github.com/TexelForge/TexelForgeReleases/releases), select a version, and expand **Assets**. Releases marked **Pre-release** are preview builds for testing, not the official launch release.

| Windows installer | Choose this for |
| --- | --- |
| `TexelForge-win-x64-Setup.exe` | Most Intel and AMD Windows PCs |
| `TexelForge-win-arm64-Setup.exe` | Native ARM64 Windows PCs |
| `TexelForge-win-x86-Setup.exe` | 32-bit Windows PCs |

Windows 10 and Windows 11 are supported. Use the installer matching your system architecture. Prefer x64 or ARM64 for large models; a 32-bit process has substantially less memory available. The installers include the required .NET runtime. The matching MSI files are available for administrative deployment.

Download an installer from **Assets**, not GitHub's **Code > Download ZIP** or the automatically generated **Source code** archives. This repository distributes releases; it does not contain the application source code.

## Try it before you buy

No payment method is required to try Texel Forge. Evaluation Mode has no time limit: import, edit, bake, repair, and preview your work. A paid license is required to export. The same installer supports evaluation and paid licenses.

No GitHub account is needed to download public releases or receive updates. Model and image processing runs locally; the updater downloads software, not your project files. License activation and periodic license validation require an internet connection.

## Automatic updates

Installed Windows builds check this repository for newer versions. You can also select **Check for updates** from the application menu. Texel Forge asks before downloading an available update, then restarts to apply it. Declining leaves the current installation unchanged. An unavailable update server does not prevent the application from opening.

Each architecture has its own update channel: `win-x64`, `win-x86`, or `win-arm64`. Preview builds can receive GitHub pre-releases; stable builds only receive stable releases. A GitHub draft is not visible to the updater.

Older builds configured before GitHub hosting was added need one manual installation of a GitHub-enabled build. They cannot discover the new location through their old placeholder update address. Loose development builds and portable copies do not automatically update.

### What are the other assets?

- `releases.win-*.json`: architecture-specific update manifests.
- `TexelForge-*-full.nupkg` (and optional delta packages): files downloaded by the updater. Do not install these manually.
- `SHA256SUMS.txt`: checksums for verifying release downloads.

These files must remain attached to the release for automatic updates to work.

## Publishing future updates

Maintainers should build and test a higher version number, create a new release, and upload the matching installers, update packages, and all three manifests before publishing it. Keep architecture channels separate. Do not overwrite an already published version or replace its signed files. A pre-release should remain marked as such until it is approved for general availability.

Only distribution artifacts belong here. Do not upload source projects, signing credentials, license keys, logs containing personal information, or customer files.

## Help

Visit [texelforge.com](https://texelforge.com/) for product information, licensing, and help. If reporting an issue here, include the app version, Windows version, architecture, and steps to reproduce it. Never include your license key or confidential project files.
