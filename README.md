# 🦉 OFlatSnap

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OCore-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OFlatSnap** — Flatpak & Snap Sandbox Permission Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OFlatSnap — Flatpak & Snap Sandbox Permission Auditor. It provides flatpak metadata parser (system + user installs, `flatpak info --show-permissions` text exports); Override merger — global + per-app, system + user, negation (!) handling, widening detection. Built-in demo/self-test paths and severity gates help validate detections without touching production when those flags are used.

---

## ✨ Features

- Flatpak metadata parser (system + user installs, `flatpak info --show-permissions` text exports)
- Override merger — global + per-app, system + user, negation (!) handling, widening detection
- Remote auditor — gpg-verify / gpg-verify-summary, plain-HTTP URLs, credential-bearing URLs (masked)
- Sandbox-escape detection: org.freedesktop.Flatpak, host filesystem, device=all, session/system bus, portal-implementation bypass, devel/ptrace feature
- EOL runtime database (GNOME / KDE / Freedesktop)
- Snap auditor — `snap list` / `snap connections` exports, snap.yaml, snapd state.json, sideloaded (--dangerous) revisions, devmode / classic / try

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OFlatSnap                                     # interactive menu
./OFlatSnap --demo
./OFlatSnap --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled.s.Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
