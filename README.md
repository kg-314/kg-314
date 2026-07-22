# Hi, I'm Kevin 👋

CS student at **UT Austin** who likes building things at both ends of the stack — from **page-fault handlers and CPU pipelines in C** to **full-stack analytics platforms serving real users**.

Currently a Product Management & Analytics Intern at **Capital One**, working on credit underwriting data migration in Python/SQL/Snowflake.

- 🔭 Building [**royalehistory.com**](https://royalehistory.com) — a live, multi-tenant battle-analytics platform
- ⚙️ Comfortable low in the stack: operating systems, computer architecture, and systems programming in C
- 📱 Also ship native iOS (Swift/UIKit) and modern web (Next.js/TypeScript)
- 🏆 2nd of 24 teams, Tracer FIRE DFIR Competition 2026 (Sandia National Labs)

---

## 🚀 Featured Projects

### [Royale History](https://github.com/kg-314/clash-royale-history) — Full-Stack Battle Analytics Platform
**`TypeScript` `Next.js` `PostgreSQL` `Supabase` `Vercel`** · 🌐 **[royalehistory.com](https://royalehistory.com)**

A multi-tenant Clash Royale battle-history tracker, live in production.

- 🔐 Per-user **row-level security**, authentication, and self-service data export/deletion
- 🗄️ PostgreSQL schema with **monthly-partitioned** battle tables, content-addressed deck deduplication, and **7 scheduled `pg_cron` jobs** automating partition lifecycle, account cleanup, and nightly stat aggregation
- 🔄 Node.js **ingestion worker** (GitHub Actions cron) polling the Supercell API with per-player adaptive intervals and failure tracking to stay within rate limits and free-tier quotas
- 📊 **Meta-insights engine** computing trophy-bracketed deck/card win rates with **Bayesian shrinkage**, surfaced through personalized matchup analytics and privacy-preserving leaderboards

### [Blackjack Strategy Simulation Engine](https://github.com/kg-314/blackjack_engine)
**`C`**

A stateless, reproducible blackjack engine built for parallel-safe simulation.

- 🎲 Caller-owned structs with **per-instance seeded RNG** — reproducible and safe to run in parallel
- 🔁 Play modeled as a **phase-based state machine** with a deck-injection hook enabling unit tests that assert exact outcomes (bust, dealer-to-17, 3:2 payout)
- 🧵 Core kept **allocation-free** with bounded loops and buffers, safe to embed in multi-instance drivers, surfacing errors via return codes

### [Scratchbook](https://github.com/kg-314/Scratchbook) — iOS Activity & Scrapbook App
**`Swift` `UIKit` `Firebase`** · *Team of 4*

A native iOS scrapbook app for logging activities with photos and sharing them with friends.

- 📸 Owned authentication, media upload, and navigation across **14 screens**
- ☁️ Photo capture/upload pipeline using **AVFoundation** and async `URLSession`, persisting image URLs in Firestore with user-facing failure handling
- 🩹 Eliminated retained-view-controller leaks by replacing circular segues with **unwind segues**, preventing unbounded navigation-stack growth

---

## ⚙️ Systems Programming

Coursework and projects deep in the stack — building the layers most apps sit on top of.

**Unix-Style Operating System Kernel** · `C` `x86` *(Pintos)*
- Priority scheduling, **priority donation**, and thread synchronization, using randomized Bochs timing to surface race conditions
- System calls enforcing a strict **user/kernel boundary** with user-pointer validation
- **Virtual memory** with demand paging and clock-based eviction under constrained frame allocation
- Multi-level indexed **file system** with a write-back buffer cache and fine-grained locking for concurrent access

**Computer Instruction Pipeline Emulator** · `C` `ARM64`
- **Five-stage pipelined** CPU emulator for a subset of the AArch64 ISA, with NZCV condition-flag semantics
- Resolved data and control hazards via **operand forwarding, stalling, and bubble (NOP) insertion**
- Configurable **set-associative cache** (write-back, write-allocate, LRU), validated against a reference simulator with exact hit/miss/eviction parity across traces of ~287K accesses

---

## 🧰 Tech Stack

**Languages**
![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat&logo=swift&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)

**Web & Mobile**
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![UIKit](https://img.shields.io/badge/UIKit-2396F3?style=flat&logo=apple&logoColor=white)

**Data & Infra**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat&logo=supabase&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat&logo=snowflake&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

---

## 📈 GitHub Stats

![Kevin's GitHub stats](https://github-readme-stats.vercel.app/api?username=kg-314&show_icons=true&hide_border=true&count_private=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=kg-314&layout=compact&hide_border=true)

<sub>🎓 B.S. Computer Science, The University of Texas at Austin · Expected Dec 2027</sub>
