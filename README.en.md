**English** | [中文](README.md)

<div align="center">

# TermX

**A desktop SSH workspace built for modern ops**

Terminal · Monitoring · Files · Snippets — all in one window

[![Free](https://img.shields.io/badge/personal-free%20forever-success?style=flat-square)](#license--free-use)
[![Non-Commercial](https://img.shields.io/badge/non--commercial-important?style=flat-square)](#license--free-use)
[![Data Local](https://img.shields.io/badge/data-local-informational?style=flat-square)](#data-security)
[![Website](https://img.shields.io/badge/website-termx.cn-4f7cff?style=flat-square)](https://termx.cn/)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2B-0078D4?style=flat-square)](#download)
[![Version](https://img.shields.io/badge/version-1.0.27-24292e?style=flat-square)](../../releases)
[![QQ Group](https://img.shields.io/badge/QQ%20group-1095707034-EB1923?style=flat-square)](#community)

[Website](https://termx.cn/) · [Download latest](../../releases) · [Free for personal use · No commercial use](#license--free-use) · [QQ Group 1095707034](#community)

</div>

<img src="doc/screenshots/01-home.png" alt="TermX main interface">

---

## Why TermX

The real pain of day-to-day server operations isn't any single command — it's **tool-switching**. A terminal here, a monitoring dashboard there, an SFTP client somewhere else, command snippets scattered across sticky notes. TermX brings these capabilities together in a single desktop app, so you can see and act on everything within one screen.

- **All-in-one workspace** — Terminal, SFTP, monitoring, and snippets collaborate on the same screen; no more window juggling
- **Production-ready** — Real-time performance monitoring tunnels through your existing SSH session; no agent to install on the server
- **Keyboard-first workflow** — The command palette (<kbd>Ctrl</kbd>+<kbd>P</kbd>) reaches every action without leaving the keyboard
- **Chinese-first** — UI, docs, and community are Chinese-first, matching how Chinese ops teams actually work
- **Local-first data** — Aside from update checks, no network traffic; everything stays on your machine
- **Free forever for personal use** — No feature gates, no ads, no in-app purchases

---

## Core Features

### Multi-Pane Terminal

Splitting isn't just splitting — it's carving one session into multiple independent workspaces. Watch logs while debugging processes, run a deployment while watching metrics, compare production and staging output — all terminals share one window with draggable divider ratios, and each shell keeps its own history, current directory, and tab-completion context.

- Multiple tabs + arbitrary horizontal / vertical split combinations
- Full Unicode / CJK / 256-color rendering; select to copy, right-click to paste
- Customizable color schemes, fonts, line height, cursor style, scrollback
- Command history and command suggestions
- File paths and URLs auto-detected as clickable links

### Real-Time Performance Monitoring

Once an SSH session is established, the monitoring panel starts collecting key system metrics immediately. All data flows through the existing SSH channel — **zero footprint on the server, no agent required**.

- **System info** — OS, kernel version, hostname, IP, architecture, boot time, uptime
- **CPU** — Overall usage + per-core usage (dozens of cores supported), 1 / 5 / 30 minute trend curves, peak / lowest core highlighted
- **Memory** — Physical memory + Swap usage and ratio
- **Disk** — Partition mount points, capacity, read/write IO rates
- **Network** — Per-NIC throughput, TCP connection count
- **Processes** — Top N processes, sortable by CPU / memory

### SFTP File Browser

A graphical remote file manager that saves you from `cd` / `ls` / `rm` drudgery. Drag a file from Windows Explorer to upload; the status bar shows live transfer progress.

- Dual-pane layout: remote file tree on the left, current directory listing on the right
- Full operations: upload, download, create, delete, rename, change permissions
- Four-column file details: name, size, permission bits, modification time
- Drag-to-upload: drop files straight from the local file explorer
- Transfer queue: expand the bottom status bar to see live progress

### Command Snippet Library

Save long, complex commands as reusable snippets, organize them by scenario, and insert them into the current terminal with one click. New hires start productive immediately with the team's accumulated library.

- Custom categories (Ops / Install / Web / Other — extensible without limit)
- Each snippet carries: title, description, command body, tags
- Full-text search: title + command body + tags
- Quick-insert into the current cursor position via the bottom status bar
- Common team commands become a knowledge asset

### Command Palette

Press <kbd>Ctrl</kbd>+<kbd>P</kbd> to summon the quick-action entry. Fuzzy search, keyboard navigation, every operation without a mouse click.

- Covers: session management, terminal management, splits, appearance, settings, theme switching, reconnect, SFTP open, and more
- Customizable keybindings
- Instant filtering as you type; press <kbd>Enter</kbd> to execute

### Multi-Server Management

The left sidebar unifies all your server configurations. From one server to dozens, all manageable in one place.

- Server grouping and search
- Recent-connection quick access
- One-click reconnect for dropped sessions
- Credentials encrypted at rest

---

## Screenshots

<table>
  <tr>
    <td width="50%" align="center"><b>Main Interface · Four Modules on One Screen</b></td>
    <td width="50%" align="center"><b>Multi-Pane Workflow</b></td>
  </tr>
  <tr>
    <td width="50%"><img src="doc/screenshots/01-home.png" alt="Main interface"></td>
    <td width="50%"><img src="doc/screenshots/02-multi-pane.png" alt="Multi-pane"></td>
  </tr>
  <tr>
    <td width="50%" align="center"><b>Command Palette</b></td>
    <td width="50%" align="center"><b>SFTP File Browser</b></td>
  </tr>
  <tr>
    <td width="50%"><img src="doc/screenshots/03-command-palette.png" alt="Command palette"></td>
    <td width="50%"><img src="doc/screenshots/04-sftp.png" alt="SFTP"></td>
  </tr>
  <tr>
    <td width="100%" align="center" colspan="2"><b>Snippet Management</b></td>
  </tr>
  <tr>
    <td width="100%" colspan="2"><img src="doc/screenshots/05-snippets.png" alt="Snippets"></td>
  </tr>
</table>

---

## License & Free Use

### Free Forever for Personal Use

TermX's promise: **personal and non-commercial use is free forever**. No feature limits, no ads, no in-app purchases, no time limits.

<table>
  <tr>
    <th width="60%" align="left">Use Case</th>
    <th width="20%" align="center">Allowed</th>
    <th width="20%" align="center">Price</th>
  </tr>
  <tr>
    <td>Personal learning, self-study, managing your own servers</td>
    <td align="center">Yes</td>
    <td align="center">Free forever</td>
  </tr>
  <tr>
    <td>Education, classroom demos, student labs</td>
    <td align="center">Yes</td>
    <td align="center">Free forever</td>
  </tr>
  <tr>
    <td>Open-source maintainers, internal ops for non-profits</td>
    <td align="center">Yes</td>
    <td align="center">Free forever</td>
  </tr>
  <tr>
    <td>Internal enterprise ops, day-to-day company office use</td>
    <td align="center"><b>No</b></td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td>Commercial services, paid projects, SaaS integration</td>
    <td align="center"><b>No</b></td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td>Resale, redistribution, bundled packaging</td>
    <td align="center"><b>No</b></td>
    <td align="center">—</td>
  </tr>
</table>

### Our Commitments to Free Users

- **No ads** — A clean UI with zero commercial interruptions
- **No data sales** — Your server credentials, command history, and file contents stay local and are never uploaded
- **No gated features** — Terminal, monitoring, SFTP, snippets, multi-server management — all free
- **No forced sign-up** — Download and use; no account required

> For enterprise licensing or custom development, reach out via the [website](https://termx.cn/) or QQ group.

---

## Data Security

Data is the lifeblood of an ops tool. TermX is built on one principle: **your data belongs to you, with minimal network activity and maximal locality**.

### Local Storage · Never Leaves Your Machine

The following data is stored entirely in your local data directory and **never uploaded to any server**:

- Server credentials (passwords, private keys) — stored encrypted
- Session list and server configurations
- Command snippet library and command history
- SFTP bookmark paths and browse history
- Monitoring collection config
- UI settings, themes, keybindings

### Network Activity · Only This

Throughout the entire runtime of TermX, the only outbound network call is:

> **Update check on startup** — Requests `termx.cn/api` to compare versions and prompt for new releases

Other than this, TermX does not communicate with termx.cn or any third-party server while running. You can disable "Auto-check for updates" in **Settings → General** to make the app fully offline.

### SSH Encryption · End-to-End

- All terminal commands, SFTP file transfers, and monitoring data flow over standard SSH-encrypted channels
- Data travels directly from your machine to the target server, **passing through no intermediate node**
- No agent required on the server side — zero footprint

### Credential Protection

- Passwords and private keys are encrypted at rest; never written to disk in plaintext
- Never logged; never included in error stacks or reports

### Controllable Uninstall

- Uninstall removes only program files; the user data directory requires manual cleanup
- Your data is always in your hands — migrate, back up, or destroy on your terms

---

## Long-Term · Continuously Polished

TermX is not a "ship and forget" project — it's a product under long-term, sustained investment. Here is where we are:

### Our Commitments

- **Stable release cadence** — Continuous iteration: monthly patch releases for bugs and UX, quarterly major releases for new features
- **User-driven development** — QQ group feedback and GitHub Issues are the highest priority; high-frequency requests go straight onto the roadmap
- **Cross-platform roadmap** — Windows is stable and usable today; macOS / Linux clients are on the plan
- **Community co-creation** — An open feedback channel; we shape the product together with frontline ops engineers and backend developers

### On the Roadmap

- GPU-accelerated terminal rendering for significantly lower CPU usage in high-output scenarios
- Cloud sync for command snippets (end-to-end encrypted, optional)
- Multi-server batch execution — fan one command out to dozens of machines in parallel
- Built-in Docker / Kubernetes resource views
- Built-in text editor — edit remote files without opening SFTP
- Theme marketplace and color-scheme import / export
- Visual configuration for SSH jump hosts / tunnel port forwarding
- Native macOS and Linux clients

### Release Cadence in Practice

Since launch, TermX has maintained a steady iteration rhythm. Every update is pushed directly to all users via in-app auto-update — you don't need to check manually; new versions land on the day they ship.

---

## Download

Get the latest installer from the [Releases](../../releases) page:

<table>
  <tr>
    <td width="50%" valign="middle">
      <b>TermX-Setup-1.0.27-x64.exe</b><br>
      <sub>Windows 10 1809+ / Windows 11 (x64) · ~84 MB</sub>
    </td>
    <td width="50%" align="right" valign="middle">
      <a href="../../releases">Go to Releases →</a>
    </td>
  </tr>
</table>

Or visit [termx.cn](https://termx.cn/) for the latest version and product information.

### Installation Steps

1. Double-click `TermX-Setup-1.0.27-x64.exe` to launch the installer wizard
2. Follow the wizard: Welcome → License Agreement → Install Directory → Data Directory → Install → Finish
3. The app starts automatically after installation; thereafter launch it from the Start menu or desktop shortcut
4. On first launch, add your first server to get started

> Installation does not require administrator privileges. The default install path is in your user directory; uninstall leaves no system residue.

---

## Quick Start

<table>
  <tr>
    <th width="50%" align="left">Task</th>
    <th width="50%" align="left">How</th>
  </tr>
  <tr>
    <td><b>Add a server</b></td>
    <td>"+ New Session" in the left sidebar, or <kbd>Ctrl</kbd>+<kbd>P</kbd> → "New Session"</td>
  </tr>
  <tr>
    <td><b>Connect</b></td>
    <td>Double-click the session card; the right-side monitoring panel starts collecting automatically</td>
  </tr>
  <tr>
    <td><b>Open SFTP</b></td>
    <td>Inside a session, click "Open SFTP Browser" on the path bar</td>
  </tr>
  <tr>
    <td><b>Split the pane</b></td>
    <td><kbd>Ctrl</kbd>+<kbd>P</kbd> → "Split Horizontal" or "Split Vertical"</td>
  </tr>
  <tr>
    <td><b>Save a snippet</b></td>
    <td>"+ Manage" on the bottom status bar to open the snippet manager</td>
  </tr>
  <tr>
    <td><b>Keyboard shortcut cheat sheet</b></td>
    <td><kbd>Ctrl</kbd>+<kbd>P</kbd> opens the command palette; every shortcut is reachable</td>
  </tr>
</table>

---

## Community

<table>
  <tr>
    <td width="50%" align="center" valign="middle">
      <h3>Official Website</h3>
      <p><a href="https://termx.cn/">termx.cn</a></p>
      <p>Product info · Download center · Licensing inquiries</p>
    </td>
    <td width="50%" align="center" valign="middle">
      <h3>QQ Group · 1095707034</h3>
      <img src="doc/screenshots/qq-group.jpg" width="180" alt="QQ group QR code"><br>
      <sub>Scan to join · or search the group number in QQ</sub>
    </td>
  </tr>
</table>

Joining the QQ group gets you:

- First-hand version release notifications and change notes
- Troubleshooting and Q&A directly from the developer
- Feature suggestions go straight onto the product roadmap
- Discuss ops best practices with peers

---

## Feedback

- **Bugs and feature requests**: [File an Issue](../../issues), including version, reproduction steps, screenshots, and logs
- **Licensing / enterprise customization**: Visit the [website](https://termx.cn/) contact page
- **Join the group**: QQ Group **1095707034**

---

<div align="center">

**TermX** · [termx.cn](https://termx.cn/) · QQ Group 1095707034

**Free forever for personal use · No commercial use · Local-first data · Long-term updates**

</div>
