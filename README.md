<p align="center">
  <img src="MKG Cybersecurity Solutions Logo No Background.png" alt="MKG Cybersecurity Solutions Logo" width="400">
</p>

# 🛡️ **Project Indygo**
> **The Official Multi-Architecture Tactical Operating System by MKG Cybersecurity Solutions - Lightweight, Privacy, Cybersecurity**

---

## 📖 Project Description

**Project Indygo** is a next-generation, security-hardened operating system designed natively for both **ARM64** platforms (such as the Raspberry Pi 5, and Radxa Rock 5B) and **AMD64 (x86_64)** hardware (laptops, desktop workstations, and server infrastructure).

Engineered from the ground up by **MKG Cybersecurity Solutions**, Project Indygo eliminates the traditional friction between volatile anti-forensic privacy and persistent, heavy-duty offensive security. It serves as a unified, zero-telemetry operational environment built specifically for red-team operators, security auditors, and privacy-conscious engineers.

Project Indygo is architected around three core proprietary engines:

* **Project Indygo Core Hardening (Zero-Trace Architecture):** Proactive kernel-level memory sanitization, automated hardware-level address spoofing, and strict enforcement of zero diagnostic telemetry to guarantee complete operational stealth.
* **Tactical Execution Suite:** A fully integrated, high-performance offensive security platform featuring direct raw-socket injection drivers, SDR (Software Defined Radio) sub-systems, and custom hardware audit capabilities.
* **Persistent Trust Engine:** An AES-XTS encrypted environment optimized for daily development, communications, and long-term research, built to withstand physical capture and digital analysis without sacrificing daily usability.

---

## 🏛️ System Tiers & Target Platforms

Project Indygo features tailored profiles to adapt to different hardware capabilities and deployment needs, guaranteeing stability on low-resource targets as well as maximum throughput on high-performance rigs:

### 🚀 Operational Profiles

| Profile Tier | Primary Focus | Storage Model | Memory Overhead | Target Environments |
| :--- | :--- | :--- | :--- | :--- |
| **`Indygo Daily`** | Clean Development & Secure Comms | Persistent (LUKS AES-XTS) | Very Low (~350 MB) | Daily Workstation / Field Laptop |
| **`Indygo Tactical`** *(Default)* | Full Penetration Testing Suite | Persistent (LUKS AES-XTS) | Low (~450 MB) | Red Team Audits / Physical Assessments |
| **`Indygo Ephemeral`** | Maximum Anonymity & Anti-Forensics | Volatile (100% RAM / Amnesic) | Medium (~800 MB) | High-Risk Operational Reconnaissance |

### 💻 Hardware Architecture Support

* **ARM64 Embedded (Raspberry Pi 5, Radxa Rock 5B):** Low-overhead ARM64 architecture optimized for single-board computers, custom field hardware, and portable diagnostic rigs.
* **AMD64 Standard (x86_64 Workstations & Field Laptops):** Full binary compatibility for x86_64 platforms, leveraging multi-core CPU optimizations and hardware-accelerated cryptanalysis. **(COMING SOON!)**

---

## ⚙️ Technical Core & Hardening Features

### 🔐 Kernel & Low-Level Hardening
* **Custom Kernel Tree:** Custom-compiled Linux kernel configured with proactive memory sanitization flags (`init_on_alloc=1`, `init_on_free=1`, `page_poison=1`) to prevent Use-After-Free and Heap exploitation.
* **Custom Wireless & Hardware Patches:** Out-of-the-box support for raw packet injection (`mac80211`), extended USB Wi-Fi chipsets (Alfa, TP-Link), SDR devices, and custom hardware diagnostics.
* **Restricted Kernel Logs:** Strict restriction of `dmesg` access to unprivileged users (`kernel.dmesg_restrict=1`) and disabled kexec mechanisms to block runtime kernel hot-patching.

### 🌐 Network Anonymization & Perimeter Defense
* **Automated MAC & Hostname Randomization:** Cryptographically randomized hardware MAC addresses and transient hostnames generated on every link-up event.
* **Default Network Isolation:** Zero exposed listening ports by default (`netstat` / `ss` verification clean on boot). Network services must be explicitly enabled by the operator.
* **Automated Traffic Routing & Killswitch:** Configurable default routing through encrypted VPN interfaces or Tor networks, enforced by low-level `nftables` rules that drop all non-tunneled outbound traffic upon connection drop.

### 🛡️ Anti-Forensics & Data Protection
* **LUKS AES-XTS Storage Encryption:** Full disk encryption leveraging AES-256 in XTS mode with high-count Argon2id key derivation.
* **Volatile Session Wiping:** `Indygo Ephemeral` mode runs entirely in volatile system RAM, executing automatic memory scrubbing routines upon system shutdown or media removal.
* **Metadata Sanitization Pipelines:** Deep integration of CLI and GUI metadata removal tools (`MAT2`) directly into the file manager workflow for rapid EXIF and document cleaning.

---

## 💻 Environment & Operational UX

* **Desktop Environment:** Minimalist, performance-oriented **XFCE** desktop with composition effects disabled to maintain sub-millisecond input response times and minimal battery drain on field devices.
* **Terminal Environment:** Pre-configured **ZSH** environment featuring syntax highlighting, auto-suggestions, and context-aware status prompts, paired with lightweight GPU/CPU-accelerated terminal emulators.
* **Toolchain Ready:** Pre-seeded with complete toolchains for network enumeration, wireless auditing, web app assessment, reverse engineering, and hardware communication protocols.

---

## 📄 License & Transparency

Project Indygo is released as free and open-source software under the **[GNU General Public License v3.0 (GPLv3)](LICENSE)**.

### Our Commitment
At **MKG Cybersecurity Solutions**, we believe that real security depends on absolute source code transparency, community verification, and zero hidden telemetry.

* **Open Architecture:** Full auditability of build scripts, kernel patches, and configurations.
* **No Telemetry:** Zero diagnostics, metrics, or telemetry sent to external servers.
* **Community Freedom:** Free to use, adapt, and distribute for security professionals and enthusiasts worldwide.

---

## 🤝 Contact & Enterprise Support

Maintained and developed by **MKG Cybersecurity Solutions**.

* **Issues & Contributions:** Feel free to open an Issue or Pull Request on this GitHub repository.
* **Direct Inquiries:** For commercial partnerships, custom enterprise builds, or integration inquiries, contact us at: **`mkg.cybersecurity@protonmail.com`**
