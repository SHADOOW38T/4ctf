<p align="center">
  <img src="https://6lj.github.io/4ctf/logo.png" alt="4ctf logo" width="128" height="128" />
</p>

<h1 align="center">4ctf</h1>

<p align="center">
  <strong>Four teams. One clock.</strong><br />
  A four-track cybersecurity training &amp; competition platform
</p>

<p align="center">
  <a href="https://4ctf.com"><img src="https://img.shields.io/badge/Live-4ctf.com-00c853?style=for-the-badge&logo=vercel&logoColor=white" alt="Live 4ctf" /></a>
</p>

<p align="center">
  <a href="https://4ctf.com"><strong>Live → 4ctf.com</strong></a>
  ·
  <a href="https://github.com/6lj">MyßGitHub</a>
</p>

---

## Live

The landing is live at **[https://4ctf.com](https://4ctf.com)**.

---

## What is 4ctf?

**4ctf** is a cybersecurity training and competition platform built around four tracks:

| Track | Focus |
| --- | --- |
| **Red** | Offensive labs on **Kali Linux** |
| **Blue** | Defense with **ELK** (Elasticsearch · Logstash · Kibana) SIEM |
| **Purple** | Secure coding & patches |
| **Grey** | Beginner / mixed on-ramp |

---

## Features

### Four tracks

- **Red** — Isolated offensive labs in browser **Kali Linux**
- **Blue** — SIEM views, IR reports, forensics on **ELK** stack
- **Purple** — Vulnerable-app review and patch submit
- **Grey** — Guided rooms and low-stakes XP for newcomers

### Capture rooms & CTF

- Solo, team, classroom, and arena room modes
- Dynamic flags (HMAC + nonce) — no plaintext flags stored
- Hints with XP deductions; AI never leaks flags or credentials
- Classroom pause for instructors; reconnect until lab TTL

### 1v1 Arena (hero)

- Timed match: **Red on Kali Linux** vs **Blue on ELK**
- Shared clock, live WebSocket timer / alerts / scores
- Red scoring: authorized in-lab objectives only
- Blue scoring: IoC regex patterns + AI report rubric
- Matchmaking by skill band; isolation + TTL cleanup after each match

### Labs & sandboxes

- Per-session sandboxed labs with mandatory **TTL** purge
- Network isolation — no lateral movement, no public-internet abuse path
- Lab heartbeats, warn / stop / purge lifecycle
- Capacity queue with live status when providers are full

### Learning & events (roadmap)

- Course rails per track
- Pro-style certifications tied to proctored rooms
- Tournaments with prize pools
- Flywheel: learn → compete → certify → recruit

### Landing (live now)

- Countdown launch page at [4ctf.com](https://4ctf.com)
- Waitlist signup
- AI chat (Ask AI) + message-the-developer inbox
- Spam guards: honeypot, fill-time, rate limits, disposable email block

---

## Technical features

| Area | Stack / capability |
| --- | --- |
| **Red labs** | Browser **Kali Linux** images (OCI) |
| **Blue labs** | **ELK** stack — Elasticsearch, Logstash, Kibana (Render) |
| Edge | Cloudflare Workers — TLS, WAF, DDoS, geo routing |
| Control plane | Node.js — auth, rooms, flags, match engine, WebSockets, AI proxy |
| Database | Turso (LibSQL) — flags, matches, telemetry, scores |
| Realtime | WebSockets — timer snapshots, scores, lab status |
| Flags | HMAC + nonce; one-shot consume; never in WS payloads |
| AI | DeepSeek proxy — hints + Blue report judging; schema-only output |
| Auth (planned) | Argon2id, rate limits, lockout audit |
| Ops | Lab reaper cron, TTL jobs, audit log, retention policies |

---

## Brand

<p align="center">
  <img src="https://6lj.github.io/4ctf/logo.png" alt="4ctf four-square mark" width="96" height="96" />
</p>

Four upright squares — Red · Blue · Purple · Grey — on a clean white field.

---

## Developer

**Mohammed Al-Abyah** — Security Engineer · Riyadh  - **Mohammed Maarouf** — SOC Analyst 

- Portfolio: [q5.qa](https://q5.qa/)
- CV: [q5.qa/cycv.pdf](https://q5.qa/cycv.pdf)  --[Mohammed_Maarouf_CV 2.pdf](https://Mohammed_Maarouf_CV.2.pdf)
- GitHub: [@6lj](https://github.com/6lj) 
- Email: [dev@q5.qa](mailto:dev@q5.qa)

---

<p align="center">
  <sub>4ctf · Four teams. One clock.</sub>
</p>
