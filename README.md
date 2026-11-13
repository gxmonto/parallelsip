# ParallelSIP

A two-line SIP softphone for Windows and Linux.

- Two SIP accounts at once, several calls, hold and swap.
- Conference calls: hold or drop one person while the others continue.
- Blind and attended transfer, redirect a ringing call.
- Contacts (CSV/JSON/vCard), call history, Do Not Disturb.
- Optional call transcription that runs entirely on your computer.
- Automatic updates.

## Install

Download the latest version from
[Releases](https://github.com/gxmonto/parallelsip/releases):

- Windows: `ParallelSIP-Installer-<version>.exe` (recommended).
- Debian/Ubuntu: `.deb` · Fedora/RHEL: `.rpm` · other Linux: `.AppImage`.

Windows may show a SmartScreen warning on first install: *More info → Run
anyway*. Each release includes `SHA256SUMS.txt` to verify downloads.

## Set up a line

Settings → Line 1: server, username, password. UDP is the usual transport.
The chips in the title bar show whether each line is registered.

One-way audio is almost always NAT: try **Public IP override**, or the TCP
transport.

## Transcription

Press **Transcribe** on a call, or turn it on automatically in Settings →
Transcription (download the Parakeet model once, ~670 MB). Audio never
leaves your computer. Transcribing a call is legally the same as recording
it; many places require everyone's consent.

## Troubleshooting

- Logs: Settings → General → *Open log folder*.
- Lines lost after sleep or a network change: *Re-register lines now*.

## Security

See [SECURITY.md](SECURITY.md).

---

This repository hosts the releases. The source code is not public.
