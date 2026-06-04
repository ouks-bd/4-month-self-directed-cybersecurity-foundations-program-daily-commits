# Wireshark — Basics

## Display filters worth memorizing
| Filter | Shows |
|--------|-------|
| `http` | HTTP traffic |
| `tls.handshake` | TLS handshakes |
| `dns` | DNS queries/responses |
| `tcp.port == 443` | Traffic on port 443 |
| `ip.addr == 10.0.0.5` | Traffic to/from this IP |
| `tcp.flags.syn == 1 && tcp.flags.ack == 0` | SYN packets only |
| `frame contains "password"` | Frames containing "password" (string) |

## Workflow for analyzing a pcap
1. `Statistics → Protocol Hierarchy` — what's in this capture?
2. `Statistics → Conversations` — who's talking to whom?
3. Right-click a packet → `Follow → TCP Stream` to see a full conversation
4. Apply filters progressively to narrow down
