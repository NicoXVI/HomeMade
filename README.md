<div align="center">

[![Status](https://img.shields.io/badge/status-experimental-orange.svg)]()
[![License](https://img.shields.io/badge/license-MIT-blue.svg)]()
[![Language](https://img.shields.io/badge/language-agnostic-success.svg)]()
# 🔥 HomeMade PNG Encryption Method

</div>


### 🚀 Little Overview
It's technically encrypted. Don't ask how, don't ask why, just learn the process.

---

### 🛠️ Architecture

| Phase | Operation | Technical Description |
| :---: | :--- | :--- |
| **01** | `BYTE CONVERSION` | transforms into a stream of bytes. |
| **02** | `XOR CIPHER` | xor 8 bytes at a time with the correct key. |
| **03** | `BYTE PERMUTATION` | reorder blocks of `8 bytes` using a fixed sequence. |
| **04** | `BIT INVERSION` | flip every $0 \to 1$ and $1 \to 0$ |

---

### 📦 Quick Start

```text
[ Raw Input ] ──> ( 1. Bytes ) ──> ( 2. XOR Key ) ──> ( 3. Permute ) ──> ( 4. Invert ) ──> [ Ciphertext ]
```

### ❓ Common Questions

- **Why process data in 8-byte blocks?**
  - **A:** Grouping bytes into fixed-size blocks allows for efficient permutation patterns and ensures predictable memory alignment during transformations.
- **And for the decryption?**
  - **A:** Simply reverse the pipeline workflow by running the exact operations backward through the inverse sequence.
---

> [!WARNING]
> I take no responsibility for any misuse or damage caused by the application of this method...

---

<div align="center">
  <sub>Built by Alice</sub>
</div>