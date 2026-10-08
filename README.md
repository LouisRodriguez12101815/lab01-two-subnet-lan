# Lab 01 - Two-Subnet Office LAN

Cisco Packet Tracer lab for the Junior Network Engineer portfolio.
A single 2911 router routes between two /26 subnets (Sales and Ops), each
served by a 2960 access switch, with static addressing, secured device
access, and a documented break/fix pass.

- Live page: deployed on Vercel (see repo connection)
- Full lab guide: [LAB01-GUIDE.txt](LAB01-GUIDE.txt)
- Packet Tracer file: [lab01.pkt](lab01.pkt)

## Contents

| Path | What it is |
|------|------------|
| `index.html` | Portfolio page deployed to Vercel |
| `LAB01-GUIDE.txt` | Full lab guide (scenario, subnetting, configs, checklist) |
| `lab01.pkt` | Packet Tracer file |
| `configs/` | Paste-ready device configs + PC IP settings |
| `screenshots/` | Topology and verification screenshots (add from Packet Tracer) |

## Skills demonstrated

- Subnetting 192.168.10.0/24 into two equal /26 subnets (62 usable hosts each)
- Star topology with straight-through cabling (and when crossover applies)
- IOS CLI: hostname, enable secret, console login, banner, SVI, default gateway
- Verification with show commands, ping, traceroute, ARP/MAC tables
- CompTIA 7-step troubleshooting method applied to four break/fix scenarios

## Deploy

Static site: repo root is served directly (index.html). Vercel framework
preset: Other. No build command, no environment variables.
