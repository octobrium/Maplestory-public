# MapleSky

A MapleStory v83 private server — pre-Big Bang nostalgia.

## How to Play

1. **Add an antivirus exclusion first** — see [Windows Defender / Antivirus](#windows-defender--antivirus) below. If you skip this, your antivirus will delete the game client before you can run it.
2. **Download** the latest client from [Releases](https://github.com/octobrium/Maplestory-public/releases)
3. **Extract** to any folder (e.g. `C:\Nexon\MapleStory`)
4. **Run** `MapleSky-WINDOW.exe`
5. **Register** at the login screen — pick any username and password, your account is created automatically

## Windows Defender / Antivirus

**Your antivirus will flag the game client as a virus. It is not a virus.** This is a false positive that affects every MapleStory private server — MapleRoyals, MapleLegends, and even [Nexon's own official client](http://maplestory.nexon.net/news/24299/known-issue-anti-virus-false-detections) have all dealt with this.

### Why this happens

The v83 MapleStory client (2008) uses old anti-cheat protection (HackShield/Themida) that wraps the executable in obfuscated code. Modern antivirus heuristics see this obfuscation pattern and flag it as malware — the same techniques that old anti-cheat used to prevent tampering are now indistinguishable from what actual malware uses to hide itself.

On top of that, private server clients are modified (the server IP is patched into the binary) and unsigned — there's no code-signing certificate telling Windows "a verified publisher made this." The official Nexon client is signed with Nexon's certificate, which is why it usually gets a pass. Private servers can't sign with Nexon's certificate because they're not Nexon.

This is not unique to MapleSky. Every v83 private server distributes functionally identical binaries and every one of them triggers the same antivirus warnings. MapleRoyals has [multiple](https://royals.ms/forum/threads/whitelist-mapleroyals-client-from-antivirus-software.211674/) [forum](https://mapleroyals.com/forum/threads/making-mapleroyals-an-exception-in-windows-defender.103839/) [threads](https://royals.ms/forum/threads/setting-exception-for-mapleroyals.243951/) about this exact issue.

### How to fix (Windows Defender)

Do this **before extracting** the download. If you already extracted and the .exe disappeared, you'll need to re-extract after adding the exclusion.

1. Open **Windows Security** (search "Windows Security" in Start)
2. Go to **Virus & threat protection**
3. Scroll down to **Virus & threat protection settings** → click **Manage settings**
4. Scroll down to **Exclusions** → click **Add or remove exclusions**
5. Click **Add an exclusion** → **Folder** → select the folder where you'll extract the game (e.g. `C:\Nexon\MapleStory`)
6. Now extract the .7z and the .exe will not be deleted

### Other antivirus software

If you use a third-party antivirus (Avast, Norton, Kaspersky, etc.), add the game folder to your antivirus exclusion/whitelist. The exact steps vary by product — search "[your antivirus name] add folder exclusion."

## Server Info

| | |
|---|---|
| **Version** | v83 (Pre-Big Bang) |
| **Rates** | 3x EXP / 2x Meso / 3x Drop / 5x Boss / 3x Quest |
| **Multi-client** | Unlimited |
| **Classes** | All v83 explorers |
| **HP Washing** | Allowed |
| **Inventory** | Starts at 24, scales +12 per 20 levels (max 96 at lv120) |
| **Storage** | 48 slots, free (no fees) |
| **NX** | Vote NX (utility) + Donor Points (permanent cosmetics) |

## Features

- **Godly items** — 10% chance for dropped equips to get bonus stats
- **Party quest level caps removed** — all major PQs uncapped
- **Solo expeditions** — Zakum, Horntail, etc. soloable
- **Full Holy Symbol** — works without party EXP sharers
- **Free storage** — 48 slots, no store/retrieve fees
- **Classic Maple Island** — vanilla tutorial experience
- **4/4/4/4 starting stats** — early-GMS AP allocation

## Troubleshooting

- **Game client disappeared after extracting:** Your antivirus deleted it. See [Windows Defender / Antivirus](#windows-defender--antivirus) above.
- **Game crashes on launch:** Right-click `MapleSky-WINDOW.exe` → Properties → Compatibility → check "Run in compatibility mode" → select Windows XP SP3
- **Can't connect:** Server may be offline. Check Discord for status.
- **Black screen:** Try running as Administrator

## Requirements

- Windows 10 or 11
- No other MapleStory installation needed — the download includes everything
