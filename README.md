# Lab 01 — Two-Subnet Office LAN

Junior Network Engineer portfolio lab (Cisco Packet Tracer). A small office with
two departments, Sales and Ops, split into two /26 subnets and joined by a single
router (R1).

**Live page:** https://lab01-two-subnet-lan.vercel.app (after Vercel import)
**Course:** CompTIA A+ / Network+ study track — Miami Dade College, Enterprise Network Technology (AS)

## What this repo contains

| Path | What it is |
|------|------------|
| `index.html` | Portfolio page summarizing the lab (this is what Vercel serves) |
| `LAB01-GUIDE.txt` | Full lab guide: scenario, subnetting math, step-by-step build, verification, break/fix notes |
| `lab01.pkt` | The Packet Tracer file (open with Cisco Packet Tracer) |
| `configs/R1.txt` | Paste-ready router config |
| `configs/SW1.txt` | Paste-ready switch config for SW1 (Sales) |
| `configs/SW2.txt` | Paste-ready switch config for SW2 (Ops) |
| `configs/PC-settings.txt` | Static IP settings for all four PCs |
| `screenshots/` | Topology and ping screenshots (added after the Packet Tracer build) |

## Key facts

- Subnetting: 192.168.10.0/24 split into two equal /26 subnets (62 usable hosts each)
  - LAN-A (Sales): 192.168.10.0/26 — usable .1–.62, broadcast .63
  - LAN-B (Ops): 192.168.10.64/26 — usable .65–.126, broadcast .127
- Devices: 1x Cisco 2911 router, 2x 2960-24TT switches, 4x PCs
- Security baseline: enable secret, console password, MOTD banner, password encryption
- No static/dynamic routing needed — R1 is directly connected to both subnets

## How to open the lab

1. Install Cisco Packet Tracer.
2. Open `lab01.pkt`.
3. Follow `LAB01-GUIDE.txt` for the build steps, verification checklist, and break/fix scenarios.

## Deploy

Static site — Vercel auto-detects it (no framework preset, no build command).
Connected to GitHub: every push to `main` redeploys.
