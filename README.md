# Redline

Themes, plugins and Chrome extensions for the Steam client on Windows, with a store built in and a safety net
under everything you install.

Redline is a fork of [Millennium](https://github.com/SteamClientHomebrew/Millennium): it runs Millennium's
themes and plugins, and adds what we missed when using it every day.

**[Download the latest version](https://github.com/GFocacetti/redline/releases/latest)** · [Website](https://red-line.dev) · [Ko-fi](https://ko-fi.com/T6U429QJ67)

> Redline is in beta (versions 0.x). It is used every day on Steam's stable and beta clients, but expect rough
> edges, and please report what you find.

## Features

### A store inside Steam

Plugins and themes are installed from Redline's own settings, with a picture, a description, the author and the
license of each one. Every plugin points to its author's own GitHub release, and Redline checks its size and
SHA-256 before installing it; nothing is re-hosted. The list is public:
[redline-catalog](https://github.com/GFocacetti/redline-catalog).

### Chrome extensions, without a separate plugin

Paste a Chrome Web Store link, or pick one of the recommended extensions: Redline downloads it from Google and adds
it to Steam's browser. Augmented Steam, SteamDB, ProtonDB, HowLongToBeat, uBlock Origin Lite and more work on the
Store and Community pages, also in the in-game overlay. Extensions see your Steam login, so features that need it
(owned games, wishlist) work as in Chrome. Popups and options open from a puzzle button in Steam's address bar,
which can be hidden.

### A safety net

- **Safe mode:** if Steam doesn't start after you install, update or turn on a plugin, theme or extension, Redline
  undoes that change at the next start and tells you why. If that isn't enough, it starts without plugins and
  theme, so Steam always opens.
- **Back to the previous version:** Redline keeps the version you were using when it updates, and can go back to
  it, or to any other release, from the Updates page.
- **Signed updates:** updates are installed only if they carry Redline's signature.
- **Diagnostic report:** one zip with the logs, crash reports and versions, to send when asking for help.

### And more

- Works on Steam's stable and beta clients, in desktop mode and in Big Picture.
- Updates itself in the background (or tells you, if you prefer).
- Quick CSS for your own tweaks, Redline's own look or your theme's colours on its pages.
- Translated into every language Steam offers.

## Installing

1. Download `RedlineSetup-<version>.exe` from the [latest release](https://github.com/GFocacetti/redline/releases/latest).
2. Run it and follow the steps. If Millennium is installed, the setup explains what it replaces and what it keeps
   (your plugins and themes stay).
3. Start Steam. Redline's settings are in Steam's menu, under **Redline**.

**Requirements:** Windows 10 or 11, 64-bit, with Steam installed.

### "Windows protected your PC"

When you run the setup, Windows may show this blue SmartScreen window. Choose **More info**, then **Run anyway**.

It is normal for a small project like Redline, and it is not about anything found in the file. SmartScreen warns
about every program that is new and not yet downloaded by many people, unless its author pays every year for a
code-signing certificate. Redline doesn't have one (yet), so the warning will show up for a while after each
release, until Windows gets to know it.

What you can check instead:

- **Every release links its [VirusTotal](https://www.virustotal.com) scan**: the setup and the update package,
  checked by more than 60 antivirus engines before they are published.
- **Updates are signed**: Redline installs an update only if it carries Redline's own signature, so a file changed
  by anyone else is refused.
- The setup and the update package are only published here, on this repository's Releases page.

## Privacy

Redline doesn't collect anything about you, and it never will: no telemetry, no statistics, no accounts, nothing
sent to us. It's a choice made for your safety and for ours as its developers: what isn't collected can't be lost,
leaked or misused.

The only connections it makes are the ones you'd expect: GitHub (Redline's updates and the store's list), the
plugin and theme authors' repositories when you install something from the store, and the Chrome Web Store when you
install an extension. The plugins, themes and extensions you install are made by their own authors and may connect
to their own services, as they would anywhere else. The diagnostic report is created only when you ask for it and
stays on your computer until you decide to send it to someone.

## Support

- Report a problem: [open an issue](https://github.com/GFocacetti/redline/issues), with the diagnostic report
  (Settings → General → Troubleshooting → Open logs) if you can.
- Like Redline? You can support it on [Ko-fi](https://ko-fi.com/T6U429QJ67).

## Source code and licenses

Redline's own code is not published. It is built on open-source software, listed with its licenses in
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md); among them Millennium (MIT) and its plugin SDK (LGPL-2.1),
whose modified source is published at [redline-sdk](https://github.com/GFocacetti/redline-sdk).

Redline is not affiliated with Valve, Steam or the Millennium project.
