# A Post-Quantum Resistant Lightweight Key Authentication and Exchange Protocol for Smart Home Environments

Formal verification artifacts (Scyther model and verification results) for a hybrid post-quantum authentication and key exchange protocol designed for resource-constrained smart home environments.

---

## 📄 Manuscript Information

**Journal:** IEEE Access  

**Authors**  
- Jinseob Kim  
- Naryun Woo  
- Jihyeon Ryu (Corresponding Author)  

**Affiliation**  
School of Computer and Information Engineering  
Kwangwoon University  
Seoul, Republic of Korea  

---

## 🔐 Research Overview

Smart home systems are increasingly exposed to **Harvest Now, Decrypt Later (HNDL)** attacks due to the long-term threat of quantum computing.  
To address this issue, we propose a **hybrid post-quantum authentication and key exchange protocol** that balances quantum resistance with lightweight performance.

- **ML-KEM (NIST PQC standard)** is applied to user–gateway communication over external networks.
- **Pre-shared symmetric keys** are used for gateway–device communication within internal networks (e.g., Wi-Fi, Zigbee).
- The design reduces PQC overhead while maintaining post-quantum security guarantees.

### Key Contributions

- Formal verification using **ProVerif** and **Scyther**
- 62–78% reduction in communication cost compared to existing PQC-based protocols
- 75–90% computational performance improvement over ECC-based methods

---

## 🧪 Formal Verification

This repository includes:

- `pq_lightweight_aka_smarthome_scyther.spdl`  
  → Scyther protocol source code

- `scyther_verification_results.png`  
  → Verification output showing satisfied security claims

The Scyther analysis validates secrecy, authentication, agreement, and synchronization properties under the Dolev–Yao adversary model.

---

## 🛠 Tools Used

**Scyther** (symbolic security protocol verification)

Cite:  
C. J. F. Cremers, *Scyther: Semantics and Verification of Security Protocols*,  
Ph.D. dissertation, Eindhoven University of Technology, 2006.

---

## 📌 Notes

- This repository contains **formal verification models only**.
- Executable implementation code is included.

---

## 📬 Contact

For academic inquiries or questions regarding the formal verification model, please contact:

📧 mercy1234@kw.ac.kr  

For technical issues, bug reports, or model-related discussions, please submit a GitHub Issue in this repository.
