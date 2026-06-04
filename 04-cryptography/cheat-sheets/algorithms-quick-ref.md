# Crypto Algorithms — Quick Reference

## Symmetric (same key both ways — fast)
| Algorithm | Status | Notes |
|-----------|--------|-------|
| AES-128/256-GCM | ✅ Use | Modern default, authenticated |
| ChaCha20-Poly1305 | ✅ Use | Fast on mobile/no AES hardware |
| AES-CBC | ⚠️ With separate MAC only | Padding oracle risk if naive |
| AES-ECB | ❌ Don't | Leaks patterns |
| 3DES, RC4, DES | ❌ Don't | Broken/deprecated |

## Asymmetric (key pair — slow, used for key exchange + signatures)
| Algorithm | Status | Notes |
|-----------|--------|-------|
| RSA 3072+ | ✅ Use | 2048 OK for now, 3072 forward-safe |
| ECDSA P-256, P-384 | ✅ Use | Smaller, faster than RSA |
| Ed25519 | ✅ Use | Modern signing, safe defaults |
| RSA < 2048 | ❌ Don't | |

## Hashing
| Algorithm | Status | Notes |
|-----------|--------|-------|
| SHA-256, SHA-3 | ✅ General use | |
| BLAKE2/3 | ✅ Fast alt | |
| Argon2 | ✅ Passwords | Preferred for password storage |
| bcrypt, scrypt | ✅ Passwords | Also fine |
| SHA-1 | ❌ Broken | Practical collision (SHAttered) |
| MD5 | ❌ Broken | Collisions trivial |

## Post-Quantum (NIST standardized 2024)
| Algorithm | Purpose |
|-----------|---------|
| ML-KEM (Kyber) | Key encapsulation |
| ML-DSA (Dilithium) | Digital signatures |
| SLH-DSA (SPHINCS+) | Hash-based signatures (conservative) |
