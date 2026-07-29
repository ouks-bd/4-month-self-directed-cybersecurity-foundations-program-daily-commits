# nmap — Cheat Sheet

> Only use against systems you own or have authorization for.

## Most-used flags
| Flag | Meaning |
|------|---------|
| `-sS` | SYN scan (default, fast, needs root) |
| `-sT` | Full TCP connect (no root needed, noisier) |
| `-sU` | UDP scan |
| `-sV` | Service/version detection |
| `-O` | OS detection |
| `-A` | Aggressive: OS + version + scripts + traceroute |
| `-p-` | All 65535 ports |
| `-p 1-1000` | Port range |
| `-T4` | Faster timing template (1–5) |
| `-oA name` | Output all formats (normal, XML, grepable) |
| `--script` | NSE scripts (e.g. `--script vuln`) |

## Common recipes
```bash
# Quick host discovery
nmap -sn 192.168.1.0/24

# Top 1000 ports, service detection
nmap -sV target

# Full port scan, aggressive
sudo nmap -p- -A -T4 target

# Vuln scripts
nmap --script vuln target
```
