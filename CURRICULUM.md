---
type: catalog
kind: course
status: reference
tags: [curriculum, courses, udemy, learning-resources, defense-ai, research, ai-agents]
last_updated: 2026-06-11
active_phase: P0
date_source: "[[_Phase Config]]"
---

# Course Catalog — Rust + AI Agents Track

> [!info] Active schedule (foundations-weighted) — adopted 2026-06-08
> The course-driven **calendar is now the active forward driver** (see [[_Phase Config]] → "Active Model"). **Foundations (Python/Rust/Linux/Git) keep the primary weekly weight** until solid; the applied courses below ramp month-by-month as foundations solidify. **Foundations gate the ramp** — if they're not solid at a checkpoint, the applied track slips. The free [[Defense AI Research Queue#Phase 0 Resource Queue|foundations resources]] (Rust Book, Rustlings, Missing Semester) remain the core of the early weeks.

> [!note] CV is a light parallel on-ramp, not a jump to CV depth
> June starts a **light** OpenCV on-ramp (~2 hr/week: install → camera pipeline) alongside foundations — **not** full Phase 3. CV / PyTorch / ROS 2 *depth* still waits for foundations confidence. The month-by-month plan is the active schedule (see the calendar below + [[_Phase Config]] → "Active Model").

---

## Strategy (what changed, what didn't)

- **Rust is the main systems-language track** — *already how this vault is built* (P0 is Python **and** Rust; [[Phase 4 — Rust Systems|P4]] is a full Rust phase). No re-architecting needed. **C++ stays light literacy / interview support only.**
- **AI agents run as a parallel track that starts early but stays THIN** — small tool-using agents over your own notes/logs/project docs before any full Multi-Agent ISR Assistant. The agents track does **not** start during P0; it rides the [[_Portfolio Ladder#Agent Specialization Additions|A1–A10 overlay]] from P4+. See the Agents Track section below.
- **Every course must produce an artifact** — a commit, note, benchmark table, demo clip, structured log, test case, or diagram. A watched course with no artifact didn't happen.

---

## The Catalog

Status: **P0-eligible** = supports the active phase now · **Gate → Pn** = activates when Phase *n* is active · `optional`.

| # | Course | Track | Activates | Phase | Portfolio project | Output artifact |
|---|--------|-------|-----------|-------|-------------------|-----------------|
| 1 | [Python for CV with OpenCV & DL](https://www.udemy.com/course/python-for-computer-vision-with-opencv-and-deep-learning/) (Portilla) | CV | Gate → P3 | [[Phase 3 — Computer Vision + Deep Learning\|P3]] | [[Project 3 — Classical OpenCV Object Detector\|Project 3]] | real-time camera/video pipeline + first detector demo |
| 2 | [PyTorch for Deep Learning Bootcamp](https://www.udemy.com/course/pytorch-for-deep-learning/) | ML | Gate → P3 (P2 prep) | [[Phase 3 — Computer Vision + Deep Learning\|P3]] | [[Project 4 — Low-False-Positive Image Classifier\|Project 4]] | training loop from scratch, dataset loader, export notes |
| 3 | [Ultimate Rust Crash Course](https://www.udemy.com/course/ultimate-rust-crash-course/) (Stocks) | Rust foundations | **P0-eligible** (optional supplement) | [[Phase 0 — Foundations\|P0]] | [[Project 0 — Joint Python + Rust CLI Pair\|Project 0]] | Rust CLI parsing detection-log lines |
| 4 | [Learn Rust by Building Real Applications](https://www.udemy.com/course/rust-fundamentals/) (Gavadinov) | Rust systems | Gate → P4 | [[Phase 4 — Rust Systems\|P4]] | [[Project 5 — Rust Dataset Validator\|Project 5]] | mission-log replay CLI / telemetry service |
| 5 | [Agentic AI Bootcamp: LangGraph + LangChain](https://www.udemy.com/course/complete-agentic-ai-bootcamp-with-langgraph-and-langchain/) (Naik) | AI agents | Gate → P4+ (overlay, thin) | Agent overlay → [[Phase 9 — Multi-Agent + Swarm\|P9]]* | ISR assistant → [[Project 13 — Multi-Agent Search Simulation\|Project 13]] | progressive ISR assistant: note → CV-log → ROS2-log → multi-agent |
| 6 | [YOLOv12: Detection, Tracking & WebApps](https://www.udemy.com/course/yolov12-custom-object-detection-tracking-webapps/) (Moin) | Detection/tracking | Gate → P3 / P6 | [[Phase 6 — Edge AI Deployment\|P6]] | [[Project 9 — Edge-Deployed YOLO Model\|Project 9]] | custom detector on your dataset + tracking + benchmarks |
| 7 | [ROS 2 for Beginners (Jazzy 2025)](https://www.udemy.com/course/ros2-for-beginners/) (Renard) | Robotics | Gate → P8 | [[Phase 8 — ROS 2 + Sensor Fusion\|P8]] | [[Project 11 — Autonomous Rover with Camera-Based Navigation\|Project 11]] | ROS2 perception node (image → detections) |
| 8 | [ROS 2 Nav2 + SLAM](https://www.udemy.com/course/ros2-nav2-stack/) (Renard) | Autonomy | Gate → P8 | [[Phase 8 — ROS 2 + Sensor Fusion\|P8]] | [[Project 15 — GPS-Denied Navigation Simulation\|Project 15]] | recon-robot sim w/ patrol/navigation + logs |
| 9 | [Embedded Rust with STM32](https://www.udemy.com/course/embedded-rust-for-absolute-beginners/) (FastBit) | Embedded Rust | Gate → P5 | [[Phase 5 — Robotics + Embedded\|P5]] | [[Project 7 — ESP32 RP2040 Embedded Rust Sensor Node\|Project 7]] | embedded Rust telemetry / sensor-driver node |
| 10 | [Mastering DSA in C & C++](https://www.udemy.com/course/datastructurescncpp/) (Bari) | C++ literacy | `optional` all-year, ≤1 hr/wk | interview support | — | C++ reading notes + interview practice notebook |
| 11 | [Embedded Systems on ARM Cortex-M3/M4](https://www.udemy.com/course/embedded-system-programming-on-arm-cortex-m3m4/) (FastBit/Nayak) | Embedded ARM/C | `optional`, only if deeper ARM/C needed | [[Phase 5 — Robotics + Embedded\|P5]] support | [[Project 7 — ESP32 RP2040 Embedded Rust Sensor Node\|Project 7]] | ARM/C reference notes (interrupts, linker/startup, faults) |
| 12 | LangChain: Agentic AI Engineering with LangChain & LangGraph (Eden Marco)† | AI agents | **Sprint** (user-scheduled)** | [[AI Agent Engineering Sprint\|Agent Sprint]] | [[Project — Aegis Research Agent\|Aegis Research Agent]] | tool-calling agent + Markdown RAG + LangGraph workflow (sprint Days 1–3, primary course) |
| 13 | LangGraph: Develop LLM powered AI agents with LangGraph (Eden Marco)† | AI agents | Sprint — Day 3 depth | [[AI Agent Engineering Sprint\|Agent Sprint]] | [[Project — Aegis Research Agent\|Aegis Research Agent]] | LangGraph workflow with ≥3 nodes + conditional branch |
| 14 | Production AI Agents with LangChain + LangGraph [2026]† | AI agents | Sprint — Day 6 depth | [[AI Agent Engineering Sprint\|Agent Sprint]] | [[Project — Aegis Research Agent\|Aegis Research Agent]] | production-readiness checklist + traced, tested agent |
| 15 | AI Engineer Agentic Track: The Complete Agent & MCP Course† | AI agents | Sprint — Day 4 depth | [[AI Agent Engineering Sprint\|Agent Sprint]] | [[Project — Aegis Research Agent\|Aegis Research Agent]] | MCP mapping note + minimal MCP server/client exercise |
| 16 | AI Agents Bootcamp: Build with LangChain, RAG & ANY LLM 2025† | AI agents | Sprint — Days 1–2 alternate | [[AI Agent Engineering Sprint\|Agent Sprint]] | [[Project — Aegis Research Agent\|Aegis Research Agent]] | alternate-angle agent + RAG reps (only if artifact differs from #12's) |

\* **Phase 9 is MARL** (PettingZoo/MAPPO) — academically distinct from LLM agents. Course #5 (LangGraph) feeds the *applied* ISR-assistant **overlay**; [[Project 13 — Multi-Agent Search Simulation|Project 13]] covers the MARL side. See Agents Track below.

\*\* **Sprint courses (#12–16)** activate only when the one-week [[AI Agent Engineering Sprint]] is explicitly scheduled (windows in the module note; calendar default is the Dec 2026+ "Agent sprint" slot below). #12 is the primary; #13–16 are pull-sections-as-needed support. Overlap with #5 (Naik) is real — skim-skip, don't re-watch.

† URLs pending — add at enrollment time (titles/instructors from the user's course list, 2026-06-11).

---

## AI Agents — parallel track (early but thin)

Rides the existing [[_Portfolio Ladder#Agent Specialization Additions|A1–A10 overlay]] + the Agent Specialization Overlay in [[Defense AI Curriculum - Phase Map]]. Reconciled with P0 discipline:

- **P0–P3:** zero LLM-agent work. Reach for FSM / behavior-tree fundamentals first; the [[Phase 0 Evidence Log]] stays Python/Rust/Linux/Git only.
- **P4+ (overlay):** course #5 feeds small, typed, replayable agents over *your own* notes/logs/project docs — structured outputs and an eval harness before any multi-agent system.
- **Post-grad KL sprint:** the full Multi-Agent ISR Assistant lands **Mar 2027** — see [[Kuala Lumpur Reset]] and [[_Portfolio Ladder#Post-Grad KL Sprint (Jan–May 2027)]].

Progression for course #5's artifacts: project-note assistant → CV-log summarizer → ROS2-log assistant → full multi-agent ISR workflow (with human-approval gates).

**One-week intensive option:** [[AI Agent Engineering Sprint]] — the concrete spec for the calendar's **Dec 2026+ "Agent sprint"** slot. Courses #12–16 feed it; the capstone is [[Project — Aegis Research Agent]] (research-domain sibling of A2). It may pull earlier only by explicit decision at a Sunday review (candidate windows in the module note) — **foundations gate the ramp**, and the thin-track rules above stay in force until that decision.

---

## Weekly Allocation (active — foundations-weighted)

> Active now. **Foundations get the primary block** each week; the applied tracks below are the parallel allocation that grows as foundations solidify. The CV on-ramp starts at ~2 hr/week. (Source: course-DB revised allocation.)

| Track | School-term target | KL-reset sprint target | Output |
|-------|-------------------:|----------------------:|--------|
| Computer vision / PyTorch | 4–6 hr | 8–10 hr | detector, metrics, dataset, benchmarks |
| Rust systems | 3–4 hr | 5–6 hr | log parser, replay CLI, telemetry tool |
| AI agents | 2–3 hr | 4–5 hr | tool-using agent, structured outputs, eval harness |
| ROS 2 / robotics | 2–4 hr (once started) | 6–8 hr | ROS2 node, Nav2 sim, logs |
| C++ literacy | 0–1 hr | 1 hr | read/modify small ROS2 snippets |

The **KL-reset sprint** column ties to [[Kuala Lumpur Reset]] (Jan–May 2027 build window).

---

## Course Rules

- **Rust replaces C++ as the main systems-language investment** (already the vault's stance). C++ = reading ROS2 code + passing interviews only; it should not dominate the year.
- **AI agents start early but stay thin** — build small agents over notes/logs/docs before attempting the full Multi-Agent ISR Assistant.
- **Every course must create an artifact** — repo commit, technical note, benchmark table, demo clip, structured log, test case, or architecture diagram.
- **No generic chatbots** — agent work serves ISR summarization, project review, log analysis, test generation, or human-approved mission workflows.
- **No more YOLO courses** — one custom YOLO course (#6) + your own dataset is enough.
- **One source per week** — finish before adding another (mirrors the [[Defense AI Research Queue]] rule).

---

## Skills → Résumé Keywords (earn honestly)

Wire each finished course's *artifact* to the keyword bank in [[Career - Fall 2026 Overview]]. No keyword on the résumé without a repo, note, or metric behind it.

| Course | Keywords earned (only with an artifact) |
|--------|------------------------------------------|
| #1 OpenCV | Python, OpenCV, computer vision, CNN training, model debugging |
| #2 PyTorch | PyTorch, training loops, autograd, ONNX export, model architecture |
| #3 Ultimate Rust | Rust, ownership, borrowing, error handling, cargo |
| #4 Real Rust Apps | Rust CLIs, systems programming, practical Rust patterns, file I/O |
| #5 Agentic AI | agentic AI, LLM tool use, structured outputs, LangGraph, multi-agent orchestration |
| #6 YOLOv12 | YOLO, object detection, tracking (Bot-SORT/ByteTrack), edge inference |
| #7 ROS 2 Beginners | ROS 2, node communication, launch files, sensor integration |
| #8 ROS 2 Nav2 | ROS 2, Nav2, SLAM, autonomous navigation, sensor fusion, path planning |
| #9 Embedded Rust | embedded Rust, ARM Cortex-M, Embassy, firmware, real-time systems |
| #10 DSA C/C++ | C++, data structures, algorithms (literacy/interview only) |
| #11 ARM Cortex-M | ARM embedded, C, embedded debugging, hardware drivers (support only) |
| #12–13 Marco LangChain/LangGraph | LangChain, LangGraph, RAG, vector databases, agent memory, tool calling |
| #14 Production Agents | agent evaluation, tracing (LangSmith), FastAPI/Docker agent deployment |
| #15 Agent & MCP | MCP, tool schemas, plugin-style integrations |
| #16 Agents Bootcamp | breadth reps only — no separate keyword without a distinct artifact |

---

## The month-by-month calendar (active schedule, foundations-weighted)

> Adopted 2026-06-08 as the active forward driver. Foundations keep the primary weight in the early months; applied work ramps as they solidify (**foundations gate the ramp**). Authoritative copy: [[_Phase Config]] → "Active Model".

| Month | Author's main course | Parallel track | Author's output |
|---|---|---|---|
| Jun 2026 | OpenCV | Ultimate Rust Crash Course | camera pipeline + Rust log-parser prototype |
| Jul 2026 | PyTorch | LangGraph (light) + Learn Rust by Building Real Apps | training workflow + simple project-note agent |
| Aug 2026 | PyTorch + YOLOv12 | Rust log tooling + agent structured outputs | custom detector + structured detection logs |
| Sep 2026 | ROS 2 for Beginners | agent CV-log summarizer + Rust mission-log CLI | ROS2 perception node + log summarizer |
| Oct 2026 | ROS 2 Nav2 | agent retrieval over project docs/logs | recon-robot sim + searchable logs |
| Nov 2026 | ROS 2 Nav2 / Embedded Rust | agent evaluation harness | mission demo + initial ISR assistant tests |
| Dec 2026+ | Embedded Rust / Agent sprint (spec: [[AI Agent Engineering Sprint]]) | C++ literacy only if needed | Multi-Agent ISR Assistant + embedded/edge telemetry |

---

## Links
- [[Defense AI Research Queue]] · [[_Research Index]] · [[Current Week]]
- [[Defense AI Curriculum — MOC]] · [[Defense AI Curriculum - Phase Map]] · [[_Portfolio Ladder]]
- [[Phase 0 — Foundations]] · [[Phase 3 — Computer Vision + Deep Learning]] · [[Phase 4 — Rust Systems]] · [[Phase 5 — Robotics + Embedded]] · [[Phase 8 — ROS 2 + Sensor Fusion]] · [[Phase 9 — Multi-Agent + Swarm]]
- [[Kuala Lumpur Reset]] · [[Career - Fall 2026 Overview]] · [[_Phase Config]]
