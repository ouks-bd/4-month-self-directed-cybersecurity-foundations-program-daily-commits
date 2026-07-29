# Subnetting Practice — Solutions

1. **255.255.255.192** — /26 = 24 + 2 ones; last octet = 11000000.
2. **14 usable** — /28 = 16 total − 2 (network + broadcast).
3. **192.168.1.128** — /25 splits at 128; .130 falls in the .128–.255 block.
4. **10.0.3.255** — /22 covers third-octet blocks 0–3; broadcast is .3.255.
5. **No** — /25 splits at 128; .100 is in 0–127, .200 is in 128–255.
6. **/26** — gives 62 usable hosts; /27 gives only 30.
7. **8** — /24 has 256 addresses; each /27 has 32; 256/32 = 8.
8. **192.168.10.65** — /27 boundaries are 0, 32, 64, 96; first usable in .64 block is .65.
9. **10.1.1.152** — /29 blocks of 8: ..., 144, 152, 160; .155 falls in .152 block.
10. **/29** gives 6 usable hosts (8 − 2). For a literal point-to-point link, /30 (2 usable) — unless 6 endpoints are needed.
