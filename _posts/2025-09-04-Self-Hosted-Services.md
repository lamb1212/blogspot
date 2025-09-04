---
layout: post
title: "September Update."
date: 2025-09-04
draft: false
---

---

# 🖥️ Homelab & Server Progress Journal

### 🔹 Early Setup (ThinkCentre M79 → “cranberri”)

* Installed **Ubuntu Server** and made it the homelab core.
* Added **Tailscale**, making cranberri the **exit node** for secure remote access.
* Began hosting personal files and experiments.

---

### 🔹 Self-Hosting & Services

* **Notes & Knowledge Base**

  * Originally planned Hugo for blog posts, but switched to **GitHub Pages**.
  * Use **Obsidian vault** as the main writing/notes hub.
  * Push blog posts & notes → GitHub Pages (static site).
  * **lazygit** became your go-to tool for managing repos.

* **Monitoring**

  * Set up **Prometheus + Node Exporter + Grafana** for server metrics.
  * Added **alerting** and metrics tracking (including Tailscale exit node status).

* **File Storage**

  * Looked into **Nextcloud** as an alternative to iCloud for syncing Obsidian vaults. (Not yet fully in production, but considered as a future replacement.)

---

### 🔹 Hardware & Storage

* Received a **free 1TB HDD** and added it to cranberri.
* Configured persistence with **fstab**.
* Experimented with **rsync** for music and media sync (hit some album art duplication quirks, which you debugged).

---

### 🔹 Other Devices & Projects

* **ThinkPad L490 (Kali Linux, KDE/Wayland)**

  * Explored its role in your homelab.
  * Looked into patch cables and other uses.

* **Strawberri (secondary system)**

  * Installed **Minecraft** (via PolyMC).
  * Ran your own **Minecraft server** for fun.
  * Learned in-game console and function key shortcuts.

---

### 🔹 Misc Projects & Learning

* **Blogging/Publishing**

  * Retired Hugo theme experiments → fully moved to **GitHub Pages**.
  * Plan for a **second GitHub Pages site** dedicated to documenting the homelab.

* **Python practice**

  * Small projects: calculator, character creator, yes/no logic handling.

* **Music & Typing**

  * Experimented with **Bitwig (Flatpak on Fedora)**.
  * Tried **termtypr** typing trainer from GitHub.

---

### 🔹 Networking / Cloud Concepts

* Learned **cloud fundamentals**:

  * On-demand self-service, resource pooling, elasticity, etc.
  * Difference between **SaaS, PaaS, IaaS**.
  * What an **SLA** really means (not a security concept).
* Researched **Internet peering (AMS-IX)** → understood how it reduces ISP reliance by giving direct routes between trusted networks.

---

✅ **Current State (as of now):**

* **cranberri** = exit node, metrics collector, notes + publishing hub.
* **GitHub Pages** = main way you publish blog posts (Hugo retired).
* **Obsidian vault + iCloud** = current workflow (with Nextcloud as a possible future switch).
* Expanding hardware with extra storage & considering Proxmox for virtualization.

---

