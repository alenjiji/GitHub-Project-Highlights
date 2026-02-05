# GitHub Project Highlights

Hi, I’m **Alen** — a **Software & AI Engineer** passionate about clean architecture, intelligent systems, and practical engineering.
These are my key projects showcasing depth in **AI/ML**, **systems design**, and **tooling**.

---

# **Core Skills:** Python · LLM Engineering · Clean Architecture · Systems Programming · Qt/C++ · Networking · ML Foundations

<p align="left">

  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/AI-LLM-blueviolet" />
  <img src="https://img.shields.io/badge/C++-Qt%20Widgets-00599C?logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/Networking-TCP%2FSSL-green" />
  <img src="https://img.shields.io/badge/Architecture-Clean%20Code-orange" />
  <img src="https://img.shields.io/badge/Tools-GitHub%20Actions-lightgrey?logo=githubactions" />

</p>

---

## **1. J Text Exploration Library (Foundational Architecture)**

![Python](https://img.shields.io/badge/Python-Library-blue?logo=python)

**Tech:** Python · Structured Parsing · Modular Walkers
**Repo:** [github.com/alenjiji/J](https://github.com/alenjiji/J)

* Designed and implemented the core structural exploration library for **Project J**.
* Built deterministic token-handling, structural nodes, and walkers.
* Future support planned for **A*-guided semantic traversal** (not yet implemented).
* Currently paused at a **clean, complete foundational architecture**.

**Highlights:** architecture-first design, deterministic logic, extensible framework.

Architecture Diagram
--------------------

                +--------------------------+
                |   Input Text Stream      |
                +-------------+------------+
                              |
                              v
                 +-------------------------+
                 |   Tokenizer / Parser    |
                 +-------------+-----------+
                               |
                               v
           +----------------------------------------+
           |   Structural Nodes / AST-like Model    |
           +------------------+---------------------+
                              |
                              v
                 +------------------------------+
                 |   Walkers (Deterministic)    |
                 |   - Linear Walker            |
                 |   - Branch Walker            |
                 |   - Structural Walker        |
                 +------------------------------+
                              |
                              v
       +------------------------------------------------+
       |  Future Module (Planned) — A* Semantic Walker  |
       |  *Not implemented — design-only placeholder*   |
       +------------------------------------------------+


---

## **2. Encrypted Proxy Tunnel (Real-Time Networking System)**

![Networking](https://img.shields.io/badge/Networking-Proxy%20Tunnel-green)
![Security](https://img.shields.io/badge/Security-TLS%2FAES-red)

**Tech:** Python · AsyncIO · TLS · AES · TCP
**Repo:** *(private / experimental)*

* Created a fully encrypted multi-layer proxy handling real-time CONNECT flows.
* Implemented error-handling, delegation, tunnel negotiation, and fallback logic.
* Improved speed and stability across multiple optimization phases.
* Stable operation achieved on Firefox with partial Chrome support.

**Highlights:** networking internals, security engineering, real-world debugging.

```
Encrypted Proxy Tunnel — System Flow
------------------------------------

 Client Browser
 (Chrome/Firefox)
        |
        |  CONNECT request
        v
+---------------+       Encrypted Layer       +------------------+
|  Local Proxy  |=============================>| Remote Transport |
|  (Python)     |<=============================|     Server       |
+-------+-------+                              +--------+---------+
        |                                                |
        | Decrypt / Validate                             | Forward to
        |                                                | Target Host
        v                                                v
+---------------+                              +----------------------+
| Tunnel Logic  |                              |    Target Server     |
| - Handshake   |                              | (e.g. youtube.com)   |
| - AES/TLS     |                              +----------------------+
| - Routing     |
+---------------+

Notes:
- Multi-layer encryption (AES/TLS)
- AsyncIO handles concurrency
- Chrome unstable, Firefox fully stable
```

---

## **3. DubbingTracker — Architecture-Driven Desktop Application**

![C++](https://img.shields.io/badge/C%2B%2B-Qt%20Widgets-00599C?logo=c%2B%2B)
![Architecture](https://img.shields.io/badge/Architecture-Clean%20Layers-orange)

**Tech:** C++ · Qt Widgets · Clean Architecture · GitHub Actions CI
**Repo:** *(internal work)*

* Implemented a strict **Qt-free core** with UI adapters for clean separation of concerns.
* Built core domains: ProjectManager, MarkerManager, SyncController.
* Maintained a guaranteed **40ms sync tolerance**, verified with deterministic tests.
* Refactored MainWindow to a lightweight **composition root (<150 LOC)**.
* Integrated CI gating and architecture enforcement using CMake.

**Highlights:** disciplined engineering, determinism, maintainable design.

DubbingTracker — Layered Architecture
-------------------------------------

                     +---------------------------+
                     |        UI Layer (Qt)      |
                     |  - MainWindow (composition root)
                     |  - Widgets / Controllers
                     +-------------+-------------+
                                   |
                                   |  UI Adapters
                                   v
                    +-----------------------------+
                    |     Qt Adapters Layer       |
                    |  (Connects UI → Core only)  |
                    +-------------+---------------+
                                  |
                                  v
        +-------------------------------------------------------+
        |                      Core Layer                       |
        |  - ProjectManager                                      |
        |  - MarkerManager                                       |
        |  - SyncController (40ms invariant)                     |
        |  - Autosave, Undo Systems                              |
        |  * Zero Qt dependencies                                |
        +--------------------+----------------------------------+
                             |
                             v
                   +-----------------------+
                   |  Persistence Layer    |
                   |  (Files, Serialization|
                   |        Utils)         |
                   +-----------------------+


---

## **4. Nanma-NX Media Suite**

![Python](https://img.shields.io/badge/Python-Media%20Suite-blue)
![Automation](https://img.shields.io/badge/Automation-Batch%20Tools-yellowgreen)

**Repo:** [github.com/alenjiji/Nanma-NX-Media-Suite](https://github.com/alenjiji/Nanma-NX-Media-Suite)
**Tech:** Python · Media Processing · Batch Automation

* Developed modular tools for batch media conversion and workflow automation.
* Designed components for clean extension and reusability.
* Structured for future AI-powered media integration.

**Highlights:** reliability, modular tooling, workflow efficiency.

---

## **5. Solitaire Game (Algonquin College — Co-op)**

![C#](https://img.shields.io/badge/C%23-Gameplay-blue?logo=c-sharp)
![Agile](https://img.shields.io/badge/Agile-SCRUM-purple)

**Tech:** C# · Blueprint-style logic · Agile/SCRUM
**Repo:** *(academic)*

* Contributed gameplay logic, UI flow, and sprint-based development.
* Part of a 5-member Agile team delivering iterative feature updates.

**Highlights:** gameplay logic, teamwork, iterative development.

---

## Why These Projects Matter
- AI/LLM engineering and reasoning systems
- System design with clean, modular architecture
- Networking and low-level debugging
- Cross-disciplinary work (AI + desktop apps + automation)
- Building reliable tools focused on real-world usage

---

## 📦 **Additional Mini Projects**

* Embedding-based personal search tools
* AI automation utilities
* Networking diagnostics and packet tools
* UI micro-tools for rapid prototyping

---
