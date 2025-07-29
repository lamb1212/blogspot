---
layout: post
title: "Late night blog edit"
date: 2025-07-23
draft: false
---
Networking Setup & Switch Integration

Deployed Linksys SRW2008 switch into network rack.

Initially couldn't detect it; changed AT&T router’s IP (from .254 to .253) to allow the switch to use its default IP (192.168.1.254).

Reconfigured DHCP range and rebooted devices accordingly.

Confirmed everything connects through the switch with proper gigabit links via patch cables (router, Blu, Cranberri).

Created an ASCII diagram of this setup.


              [ AT&T Router ]
                    |
             [ Linksys SRW2008 ]
              /       |       \
        [ Cranberri ] [ Blu ] [ Strawberri ]
         (Server)     (Kali)   (Laptop - Mobile)



Systems & Devices

Cranberri (main server):

Used for hosting services like Portainer.

Temporarily went offline during network issues; SSH'd back in and verified IP and hostname issues (showing up as "unknown" on router).

Considered renaming hostname and user accounts for clarity (strawberri@unknown...).

Strawberri (mobile/outdoor laptop):

Used Tailscale to reconnect to Cranberri.

Explored using reverse SSH tunneling to leverage tools on Blu from Strawberri while away.

Used Fedora Workstation (Plasma, then GNOME after Wi-Fi issues).

Encountered networking UI issues in Plasma; GNOME let you log in to Wi-Fi properly.

Blu (Kali box in the rack):

Considered how to use tools stored on Blu remotely without moving them to Straw.

Explored SSH reverse tunnels for accessing tools like nmap and ddgr from Straw while Blu stays on home network.

Rebooted Blu into Windows to consider interacting with iCloud and passing that access to Cran.

Access & Tunnels

Used Tailscale with MagicDNS:

Verified that name resolution works across devices (e.g., ssh cranberri, ssh strawberri).

Allowed for easier remote access to all machines from each other.

SSH Usage:

SSH'd into Cran and Blu repeatedly.

Discussed SSH chaining (SSH from Straw → Blu → back to Straw).

Ensured hostnames and usernames were consistent or clarified for smoother access.

Tools & Terminal Workflow

Ran nmap to audit your LAN and identify MAC addresses + device vendors.

Used nano for daily blog post writing:

Lost one post due to session/network interruption, looked for .save files (none found).

Reviewed local blog drafts.

Asked about Nano settings and improvements.

Started using ddgr (DuckDuckGo CLI):

Wanted to pass URLs discovered via SSH on Cran to Straw (host machine).

Discussed several methods: copying to clipboard, JSON parsing, opening URLs from terminal.

Other Technical Events

Changed router DHCP range and temporarily lost access to router UI.

Fixed keyboard layout on Straw (reassigned Fn to act as Ctrl).

Explored opening tabs on the local device while searching remotely.

Key Themes Across These Days:

Centralizing power in Blu (all tools live there) while using Straw as the mobile interface.

Building network resilience through better switch/router config.

Streamlining access via Tailscale, SSH, and hostnames.

Workflow improvement using terminal utilities, nano, and remote browser link handling.


