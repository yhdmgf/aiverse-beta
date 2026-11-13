# AiVerse Beta

> [中文](README.md) · English

This repository hosts the **daily beta builds of AiVerse**. Beta packages are built automatically by the CI of the main repository [yhdmgf/AiVerse](https://github.com/yhdmgf/AiVerse) at fixed times and published to this repository's [Releases](https://github.com/yhdmgf/aiverse-beta/releases), with auto-incrementing version numbers.

> ⚠️ **Not recommended for regular users.** The beta build is aimed at developers and testers who want to try new features early, and it may be unstable or even contain high-risk issues. Regular users should use the [stable release](https://aivapp.cn/download) or the preview (rc) builds in the main repository's Releases.

## What is this

- Automatically builds the latest code on the main repository's `main` branch every day at **00:00 / 06:00 / 12:00 / 18:00** Beijing time.
- Each beta package: official signature + R8 minification, package name `com.aiverse.beta`, and **it can coexist with the stable version on the same device without overwriting each other**.
- Version numbers auto-increment starting from `1.0.1`, rolling over to `2.0.0` after `1.0.99`.

## ⚠️ Before you use it (please read first)

- **For internal testing only; it does not represent the final version.**
- **Do not redistribute, repackage, upload, or share it with others, and do not use it for commercial purposes.**
- The beta build **carries a watermark** and is **excluded from in-app update checks** — it will not prompt you to upgrade, nor will it redirect you to the stable package; you need to come back to this repository manually to download a new build.
- It may be unstable: crashes, feature anomalies, and data incompatibility can all occur. **Please back up your important data yourself.**

## Choosing a package

Each Release directly ships three APKs (fixed file names, no version number) plus a usage notice. Pick one based on your device type:

| File | Suitable devices | Notes |
|------|------------------|-------|
| `AiVerse-universal-beta.apk` | Any device | Universal build with both arm + x86 images, largest in size. Prefer this if you are unsure about your device architecture |
| `AiVerse-arm64-beta.apk` | Most real devices | arm64 build for real devices, smallest in size |
| `AiVerse-x86_64-beta.apk` | Emulators | x86_64 build for emulators |

Please confirm your device architecture before installing; if you are not sure, it is recommended to install the universal build.

## Want the latest build but it's not there yet?

When a commit has just been pushed but the corresponding beta build hasn't been produced yet, you have two options:

1. **One-click trigger via web page**: open the [beta trigger page](https://aivapp.cn/trigger/) and click "Trigger Build" to queue a build on GitHub on your behalf (global rate limit: shared by everyone, at most one successful trigger per hour).
2. **Wait for the next scheduled run**: builds run automatically at 00:00 / 06:00 / 12:00 / 18:00 Beijing time.

## Stable version and feedback

- **Stable download**: [https://aivapp.cn/download](https://aivapp.cn/download)
- **Official main repository**: [yhdmgf/AiVerse](https://github.com/yhdmgf/AiVerse)
- **Feedback**: if you run into problems during testing, feel free to open an issue in the [main repository Issues](https://github.com/yhdmgf/AiVerse/issues), including the version number, reproduction steps, device model, and system version.

## Disclaimer

The beta build is provided "as is", for learning, research, and legitimate software development purposes only. Any risk or loss arising from using the beta build is borne by the user. If you do not agree with the above, please stop using and uninstall this software immediately.
