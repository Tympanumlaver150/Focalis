# Focalis Downloads

[简体中文](README.zh-CN.md)

Focalis is a Windows desktop workbench for digital design analysis. It brings Design hierarchy,
semantic RTL source, VCD/FST waveform viewing, Driver/Load Trace, schematic exploration, an editor,
and permissioned Agent/MCP workflows into one application.

> **Beta software:** validate the current prerelease with non-production data before relying on it
> for critical sign-off work. Report reproducible correctness or stability issues through Support.

## Download

Current version: **Focalis vA-2026.06 Beta 0.1.0**.

[Open Focalis Releases](https://github.com/DawnCarol/Focalis/releases)

Use only assets attached to the latest GitHub Release:

| Asset | Purpose |
| --- | --- |
| `focalis_vA-2026.06_x64_beta-<version>.exe` | Windows x64 installer |
| `focalis_vA-2026.06_x64_beta-<version>.exe.blockmap` | Differential update metadata |
| `latest.yml` | Automatic update metadata |
| `SHA256SUMS.txt` | Release asset integrity checks |

This repository intentionally contains no Focalis application source code. GitHub's automatically
generated source archives contain only this public release metadata and are **not** application
source packages.

## Install

1. Download the installer and `SHA256SUMS.txt` from the same Release.
2. Verify the SHA-256 checksum before running the installer.
3. Run the installer and optionally create the desktop shortcut.
4. Start Focalis and open **About Focalis** to confirm the version and Beta trial status.
5. Open **Help > User Guide** to read the version-matched offline manual installed with Focalis.

Focalis currently targets Windows 10/11 x64. Large RTL designs and waveform dumps benefit from
additional memory and local SSD space. Included examples require no separate compiler installation.

## First Evaluation

Use **Examples** and select one of the packaged designs:

- **Ibex demo system** for the fastest Design/Source/Wave/Trace walkthrough;
- **CVA6 CoreMark** for a larger hierarchy and FST workload;
- **PicoRV32 SoC** for another compact RTL and waveform example.

The recommended first path is:

```text
Load Design -> select an instance -> inspect Source -> open Dump
-> add signals to Wave -> move Cursor -> Trace Driver/Load -> open Schematic
```

## Updates And Beta Access

Use **About Focalis > Check for updates** to check the official Focalis release feed. Updates are
never installed silently while documents are dirty. Each Beta build provides a two-calendar-month
evaluation period; after it expires, that build requires a valid license. Installing a newer Beta
starts the evaluation policy declared by that version.

## Data And Network Use

RTL, filelists, waveform dumps, indexes, and workspace sessions remain local during normal Debug
and Code workflows. Network access is used only for features the user explicitly configures, such
as update checks, an AI provider, or external MCP connectivity. Do not paste API keys into issue
reports.

## Support

Before reporting a problem, record:

- full Focalis version and Windows version;
- whether the input is VCD or FST and its approximate size;
- the first actionable Design/Message diagnostic;
- minimal reproducible steps and whether an included example reproduces the issue;
- relevant task log or screenshot with private paths and RTL removed.

Use [GitHub Issues](https://github.com/DawnCarol/Focalis/issues) for sanitized, reproducible product
reports and follow `SUPPORT.md`. Security-sensitive issues must not be posted in a public issue.

## License And Notices

Focalis is distributed as closed-source software. Read this repository's `EULA.md`, `PRIVACY.md`,
`SUPPORT.md`, and `SECURITY.md` before installation. Third-party notices are installed with the
application and are available offline.
