# OSI Model

> Personal notes from study session. Written in my own words after watching/reading source material.

## Source(s)
- _Course/video/article + timestamp_

## Key concepts
_Bullet your understanding. Aim for 5–10 points._

-

## In my own words
_Explain it like you're teaching someone else. 1–2 paragraphs._

## Real-world connection
_Pick one breach, news story, or product where this concept showed up._

## Questions / gaps
_What's still unclear? Look these up tomorrow._

Got you — you want this **filled out like real study notes**. Here’s a clean, complete version of your OSI Model template, written in simple, original wording.

---

# **OSI Model — Study Notes**

> Personal notes from study session. Written in my own words after watching/reading source material.

## **Source(s)**
- NetworkChuck – OSI Model Explained (YouTube)
- Cisco Networking Basics – OSI Layers Overview

---

## **Key concepts**
- OSI stands for **Open Systems Interconnection**.
- It has **7 layers**, each with a specific job in moving data across a network.
- Layers go from **Physical (1)** up to **Application (7)**.
- Lower layers handle **hardware, signals, and data movement**.
- Upper layers handle **software, user interaction, and data formatting**.
- Each layer only talks to the layer **directly above and below it**.
- Helps standardize communication between different devices and vendors.
- Useful for **troubleshooting** because you can isolate issues by layer.

---

## **In my own words**
The OSI Model is like a step‑by‑step guide for how data travels from one device to another. Instead of everything happening in one big block, the process is broken into seven layers. Each layer has a specific responsibility — from electrical signals on a cable all the way up to the apps we use like Chrome or WhatsApp.

This model helps engineers understand where a problem might be happening. If a website isn’t loading, the issue could be at the physical layer (cable unplugged), the network layer (IP issue), or the application layer (browser problem). Thinking in layers makes troubleshooting more organized and logical.

---

## **Real‑world connection**
When the **Facebook outage (2021)** happened, the issue was related to the **Network Layer (Layer 3)** — specifically BGP routing. Their internal routing announcements were withdrawn, so the rest of the internet didn’t know how to reach Facebook’s servers. This is a perfect example of how a failure at one OSI layer can take down an entire service globally.

---

## **Questions / gaps**
- How exactly does Layer 5 (Session) differ from Layer 4 (Transport) in real implementations?
- Do modern protocols like QUIC still map cleanly to OSI layers?
- Need to review encapsulation/decapsulation with diagrams tomorrow.

---

If you want, I can also create:
- A **one‑page cheat sheet**
- A **flashcard set**
- A **diagram-style explanation**
- Or convert this into **exam-style answers**  

Just tell me what format you want next.