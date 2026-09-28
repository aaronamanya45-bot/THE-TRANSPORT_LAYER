# Transport Layer Presentation — Group 4

**The Transport Layer: End-to-End Communication**

Reliable delivery · Multiplexing · Flow control · TCP & UDP

Course: CSC1101 | Institution: Uganda Christian University | Group: 4 | Date: September 2026

---

## Overview

This repository contains a presentation on **The Transport Layer (Layer 4)** of computer networking, created by **Group 4** for **CSC1101** at **Uganda Christian University**.

The presentation explains how the Transport Layer enables true end-to-end communication between programs running on different devices, covering the two main protocols — **TCP** and **UDP** — along with their responsibilities, differences, and real-world applications.

---

## Group Members

| Name |
|------|
| Amanya Aaron |
| Arinaitwe Simon |
| Ampumuza Esther |
| Kisige Damella |
| Nakamya Rehema |
| Winyi Joel Melvin |

---

## Presentation Contents

| # | Section | Description |
|---|---------|-------------|
| 01 | Introduction | What the Transport Layer is, its position between Network and Application layers, and its end-to-end focus |
| 02 | How Data Travels | Full message journey from sender app to network to receiver app, including segmentation, IP addressing, framing, and reassembly |
| 03 | Responsibilities | Five core jobs: segmentation, reassembly, error control, flow control, and port addressing |
| 04 | TCP | Reliable, connection-oriented delivery; sequence numbers, acknowledgments, retransmission, and the 3-way handshake |
| 05 | UDP | Fast, lightweight, connectionless delivery; minimal overhead and best-use cases |
| 06 | Comparison | When to use TCP vs UDP, with examples (web, email, downloads, streaming, gaming, VoIP) |
| 07 | Ports & Multiplexing | How port numbers let multiple apps share one internet connection; well-known, registered, and dynamic port ranges |
| 08 | Why It Matters | Real-world impact on Netflix, YouTube, Gmail, Zoom, WhatsApp, and web browsing |
| 09 | Summary | Key takeaways: Layer 4 as the bridge, five main jobs, TCP reliability, UDP speed, and protocol choice |

---

## Key Concepts

### The Transport Layer (Layer 4)

- Sits between the **Network Layer (IP)** and the **Application Layer**
- First layer providing **true end-to-end communication** between programs
- Cares about the **final destination process**, not just the next hop

### Five Core Responsibilities

1. **Segmentation** — breaking large messages into smaller segments
2. **Reassembly** — restoring segments in correct order at the destination
3. **Error Control** — checksums and retransmission (TCP)
4. **Flow Control** — sliding window mechanism to prevent flooding
5. **Port Addressing** — identifying the correct application (e.g., 80 for HTTP, 443 for HTTPS)

### TCP (Transmission Control Protocol)

- Connection-oriented (3-way handshake: SYN, SYN-ACK, ACK)
- Reliable, ordered delivery with acknowledgments and retransmission
- Flow and congestion control
- **Best for:** websites, email, file downloads, banking

### UDP (User Datagram Protocol)

- Connectionless, "fire-and-forget"
- Only 8-byte header, no acknowledgments or retransmits
- **Best for:** live video/audio, online gaming, VoIP, DNS queries

### Port Ranges

| Range | Type | Examples |
|-------|------|----------|
| 0 – 1023 | Well-Known | 80 (HTTP), 443 (HTTPS), 22 (SSH), 53 (DNS), 25 (SMTP) |
| 1024 – 49151 | Registered | Vendor/application services |
| 49152 – 65535 | Dynamic/Ephemeral | Temporary client-side ports |

---

## Real-World Examples

| Service | Protocol | Why |
|---------|----------|-----|
| Netflix / YouTube (streaming) | UDP | Speed over perfection |
| Gmail / Outlook | TCP | Every email must arrive complete and ordered |
| Zoom / WhatsApp (media) | UDP | Real-time conversation continues if packets drop |
| Web Browsing | TCP | Every part of the page must arrive correctly |

---

## Key Takeaways

1. **Layer 4 is the bridge** — connects IP packets to applications
2. **Five main jobs** — segmentation, reassembly, error control, flow control, port addressing
3. **TCP = Reliable** — connection-oriented, ordered, retransmission
4. **UDP = Fast** — connectionless, lightweight, ideal for real-time
5. **Choice matters** — modern services succeed by picking the right protocol

---

## Repository Structure

    Transport-Layer-Presentation/
    │
    ├── README.md
    ├── Transport_Layer_Clean.pptx
    └── assets/
        └── (images and diagrams)

---

## Course Information

| | |
|---|---|
| Course | CSC1101 |
| Institution | Uganda Christian University |
| Group | Group 4 |
| Date | September 2026 |

---

## License

This project is for **academic purposes** as part of CSC1101 coursework at Uganda Christian University.

---

**Thank You!**

Made with love by Group 4 · CSC1101 · Uganda Christian University
