# TLS 1.3 Handshake — Memorize This

```
CLIENT                                                 SERVER
  |                                                       |
  |  1. ClientHello                                       |
  |  → cipher suites, random, key share (ECDHE)           |
  |------------------------------------------------------>|
  |                                                       |
  |  2. ServerHello + EncryptedExtensions + Cert          |
  |     + CertVerify + Finished                           |
  |  ← chosen cipher, random, key share, cert chain       |
  |  (everything after ServerHello already encrypted)     |
  |<------------------------------------------------------|
  |                                                       |
  |  3. Verify cert chain                                 |
  |  3. Derive shared secret via ECDHE                    |
  |  3. Send Finished (encrypted)                         |
  |------------------------------------------------------>|
  |                                                       |
  |  ← Application data (AES-GCM or ChaCha20-Poly1305) →  |
```

## Key points to recite in interviews
1. **1 round trip** (vs. 2 in TLS 1.2) — faster connections
2. **Ephemeral key exchange (ECDHE)** — provides Perfect Forward Secrecy
3. **Server authenticated** via certificate + signature over handshake transcript
4. **Symmetric session keys** derived for bulk encryption (asymmetric only for setup)
5. **Old weak stuff removed** — no static RSA, no RC4, no CBC-without-AEAD, no compression

## Common interview follow-ups
- *What's PFS and why does it matter?* — Even if the server's long-term private key is stolen years later, past sessions remain undecryptable because each used an ephemeral key.
- *Why is asymmetric used only at the start?* — It's 100–1000× slower than symmetric. We use it to bootstrap a shared symmetric key.
- *What does the certificate actually prove?* — That a trusted CA verified the server controls this domain. It does NOT prove the server is "safe" or "trustworthy" in any broader sense.
