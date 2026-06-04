# Diagrams

Save draw.io exports here as both `.drawio` (source) and `.png` (preview).

## Target weekend diagram
Build a corporate network with:
- Internet → edge router → NGFW
- DMZ subnet (web server, reverse proxy)
- Internal firewall behind DMZ
- VLANs: Workstations (10), Servers (20), IoT (30)
- VPN concentrator feeding internal firewall
- Label every link with allowed protocols/ports
