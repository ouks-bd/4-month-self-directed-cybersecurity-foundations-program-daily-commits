# OSI Layers — Quick Reference

Top-down mnemonic: **A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing
Bottom-up mnemonic: **P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way

| # | Layer | Examples | Attacks |
|---|-------|----------|---------|
| 7 | Application | HTTP, HTTPS, DNS, SMTP, SSH | SQLi, XSS, malicious payloads |
| 6 | Presentation | TLS, encoding | _Often combined with 7_ |
| 5 | Session | NetBIOS, RPC | Session hijacking |
| 4 | Transport | TCP, UDP | SYN flood, port scan |
| 3 | Network | IP, ICMP, routers | IP spoofing, ICMP recon |
| 2 | Data Link | MAC, switches, VLANs | ARP poisoning, MAC flooding |
| 1 | Physical | Cables, radio | Cable taps, RF jamming |
