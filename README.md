# 🛡️ CERTI-FIKA | Cryptographic Trust Node
**Status:** Operational // Production-Ready
**Classification:** Professional Credential Verification

### 0x01 Overview
Certi-fika is a decentralized-inspired credential wallet designed to eliminate certificate fraud. It enables professional entities to verify academic and technical certifications through immutable cryptographic fingerprints without requiring a centralized database query.

### 0x02 Technical Architecture
- **Encryption:** `HMAC-SHA256` hashing for credential integrity.
- **Protocol:** Implementation of Verifiable Credentials (VC) logic.
- **Storage:** Local-first encrypted storage with DID (Decentralized Identifier) mapping.
- **Payload:** Optimized Base45 QR encoding for ultra-low latency scanning (<150ms).

### 0x03 Verification Flow
1. **Hash Generation:** Metadata (Serial + Date + Issuer) is salted and hashed.
2. **QR Embedding:** The hash is embedded into a compact QR code.
3. **Validation:** The scanner performs a local hash-match against the public key registry to confirm authenticity.

### 0x04 Deployment
Managed via GitHub Pages. Zero-dependency footprint for maximum security and loading speed.
