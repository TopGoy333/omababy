# Omabloat - Omarchy Plugin

**This repository is now an official Omarchy plugin.**

🔗 [View on GitHub](https://github.com/TopGoy333/omababy)

[![Omarchy Plugin](https://img.shields.io/badge/Omarchy-Plugin-blue.svg)](https://plugins.omarchy.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

This is an **Omarchy plugin** for safe debloating and Steam setup. We love Linux!
I am learning as I go — most of the coding is done with a little help from AI,
and the rest by me — so these guides are written for people who are learning too.

## 📦 What This Plugin Does

- **Find Bloat** ([`find-omarchy-bloat.sh`](find-omarchy-bloat.sh)) - Read-only scan to detect bloatware before/after setup
- **Install Steam** ([`install-steam.sh`](install-steam.sh)) - Guided Steam installation with ProtonPlus support for better game compatibility
- **Debloat Safely** ([`debloat-omarchy.sh`](debloat-omarchy.sh)) - Safe, reversible cleanup with guard lists and audit mode

## 🚀 Quick Start (For Users)

```bash
chmod +x find-omarchy-bloat.sh install-steam.sh debloat-omarchy.sh
./find-omarchy-bloat.sh                  # FIRST: baseline before installing apps
./install-steam.sh                       # Install Steam with guided setup
./debloat-omarchy.sh --audit             # LAST: review what could be cleaned
```

## 🎯 The First-and-Last Rule

[`find-omarchy-bloat.sh`](find-omarchy-bloat.sh) is the bookend of a full
setup: run it **first** (before installing apps) and **last** (after everything
is set up and cleaned). It never changes anything — it only reports.
[`debloat-omarchy.sh`](debloat-omarchy.md) is the cleanup tool, and its default
mode is read-only too.

## What is in here

- [`find-omarchy-bloat.sh`](find-omarchy-bloat.sh) — read-only bloat detector; first and last step.
- [`install-steam.sh`](install-steam.sh) — guided Steam install plus ProtonPlus explanation.
- [`steam-setup.md`](steam-setup.md) — the beginner flow, with a tree of every branch.
- [`debloat-omarchy.sh`](debloat-omarchy.md) — safe, reversible cleanup with a guard list.

## Quick commands

```bash
chmod +x find-omarchy-bloat.sh install-steam.sh debloat-omarchy.sh
./find-omarchy-bloat.sh                  # FIRST: baseline
./install-steam.sh --check               # read-only
./install-steam.sh                       # guided install (asks first)
./install-steam.sh --with-protonplus     # also offer ProtonPlus
./find-omarchy-bloat.sh                  # LAST: compare with the baseline
./debloat-omarchy.sh --audit             # read-only cleanup review
```

Nothing here removes anything without telling you first. Back up your config
before big changes, and remember: we love the idea of teaching people how to
use their own software and open source!
