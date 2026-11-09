<div align="center">

<img src="https://etherimirr.github.io/profile.jpg" width="200" style="border-radius:16px" alt="Christina Jia">

<h1>Christina Yijing Jia</h1>

<p>
  <b>Distributed backend systems</b> &nbsp;·&nbsp; <b>LLM agent infrastructure</b> &nbsp;·&nbsp; <b>Computer vision</b>
</p>

<p>
  <code>M.S. Computer Engineering @ Columbia</code> &nbsp;
  <code>Dec 2026</code> &nbsp;
  <code>B.E. ECE @ UMich-SJTU JI</code>
</p>

<p>
  <a href="https://www.linkedin.com/in/christina-jia-36992b383/">
    <img src="https://img.shields.io/badge/LinkedIn-christina--jia-0A66C2?style=flat-square&labelColor=0D1117&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:yj2923@columbia.edu">
    <img src="https://img.shields.io/badge/Email-yj2923@columbia.edu-14B8A6?style=flat-square&labelColor=0D1117&logo=maildotru&logoColor=white" alt="Email">
  </a>
  <a href="https://etherimirr.github.io">
    <img src="https://img.shields.io/badge/Site-etherimirr.github.io-8B5CF6?style=flat-square&labelColor=0D1117&logo=githubpages&logoColor=white" alt="Site">
  </a>
  <a href="https://etherimirr.github.io/photography.html">
    <img src="https://img.shields.io/badge/Photography-gallery-34D399?style=flat-square&labelColor=0D1117&logo=canon&logoColor=white" alt="Photography">
  </a>
</p>

</div>

---

I work on the unglamorous half of systems: the execution layer underneath, the part that has to
stay correct when things run concurrently and for a long time. Lately that has meant LLM agents in
production, and increasingly computer vision, which is where I want to go deeper.

This past summer I was a SWE intern on **TikTok Trust &amp; Safety, Algorithm Infra**. I designed and
shipped the **Smart Analysis Agent** for the team's model evaluation platform end to end, on the company's
LangGraph and MCP agent framework. It replaced a manual loop of downloading evaluation exports, writing
up the analysis by hand, and uploading the report. In front is a React and TypeScript panel. Behind it,
quick reads run synchronously and full-dataset analysis runs as a background job in an isolated sandbox,
with per-conversation state in MongoDB so a run can be cancelled, resumed, or picked back up after a reload.

After that I led data engineering and ML at **DiyoWater** as an intern (Aug to Sep 2026), building a
Python/DuckDB ETL pipeline with LLM enrichment for 11,000+ venues at 95%+ precision and a FAISS two-tower
recommender on AWS. My research is a **Walmart-sponsored project with Arklex in Prof. Zhou Yu's lab at
Columbia** on evaluating conversational LLM agents.

<table>
<tr><td width="50%" valign="top">

**Interested in**
- Distributed systems &amp; backend infrastructure
- LLM agent tooling, evaluation, ML systems
- Computer vision: detection on the edge, diffusion, 3D

</td><td width="50%" valign="top">

**Looking for**
- 2027 New Grad SWE / ML / CV / AI Infra (start Jan 2027)
- US-based, open to relocation

</td></tr>
</table>

---

### Publications

**TaskMap: Task-Conditioned LLM Adaptation in a Shared Orthogonal Basis**<br>
Second author. Accepted to **WSDM 2027 Findings**. [Code](https://github.com/liangwen12year/TaskMap)

---

### Research interests and reading

- **Agent evaluation and user simulation.** How to tell whether a tool-calling agent is actually getting better.
- **Parameter-efficient and multi-task adaptation.** Where interference between tasks comes from and how to contain it.
- **World models.** What the state should be, and how to predict it without generating every pixel.
- **On-device inference.** Decoding is a memory problem, so capacity and bandwidth decide what runs locally.
- **Vision on the edge and in 3D.** Detection under a 5W budget, reconstruction, diffusion.

Paper notes live in [reading-notes](https://github.com/etherimirr/reading-notes), with longer pages on [world models](https://etherimirr.github.io/reading-notes/world-models/) and [running large models locally](https://etherimirr.github.io/reading-notes/local-inference/).

---

### Selected work

| | Project | The hard part | Stack |
|---|---|---|---|
| 📄 | **[TaskMap](https://github.com/liangwen12year/TaskMap)** | Task-conditioned LLM adaptation where each task is a set of coefficients in shared fixed orthogonal bases. Second author, WSDM 2027 Findings. | `PyTorch` `PEFT` `Qwen2.5` |
| 🛠️ | **[durable-agent-runner](https://github.com/etherimirr/durable-agent-runner)** | An analysis agent that survives its own failures. LangGraph state machine over MCP tools, on a task runner with leased workers, fencing tokens and checkpointed steps. A worker killed mid-run on a 2M-row file is replaced and finished steps are not repeated. | `Python` `LangGraph` `MCP` `React` `TypeScript` |
| 🧗 | **[rcri-climbing-route-recognition](https://github.com/etherimirr/rcri-climbing-route-recognition)** | Real-time climbing route ID on a Jetson Nano, built with one teammate. Three-stage YOLOv8 pipeline (mAP50 0.825 on holds), ONNX to TensorRT FP16, 12 FPS for the detection stage and 5 FPS for the full pipeline at 5W, plus an A* beta solver. | `PyTorch` `TensorRT` `Jetson` |
| ⚡ | **[mbook](https://github.com/etherimirr/mbook)** | Deterministic limit order book. O(1) dense tick ladder over a preallocated slab, nothing allocated on the hot path, replay verified by a digest over the ordered fill stream. | `C++17` `CMake` |
| 🔒 | **Nightwatch** *(private)* | Multi-agent assistant on the Claude Code SDK. Five-layer memory (procedural, working, episodic, semantic, persona), and a read-only digital twin with three-layer prompt-injection defense. | `Python` `SQLite/FTS5` `ChromaDB` |
| 🧭 | **[cs-interview-coach](https://github.com/etherimirr/cs-interview-coach)** | Local-first, sub-millisecond FST search over 140+ knowledge cards, with FSRS spaced repetition across five navigation views. | `Rust` `Tauri` `SvelteKit` |
| 🗺️ | **[atlas-of-wonders](https://github.com/etherimirr/atlas-of-wonders)** | Interactive travel atlas in one static HTML file: d3-geo map, per-trip diaries, venue markers recovered by running OCR over my own photos. [Live](https://etherimirr.github.io/atlas-of-wonders/). | `d3-geo` `Vision OCR` `Vanilla JS` |
| 🧙 | **Desk Companions** *(private)* | 3D anime desktop pets for macOS: image to mesh (Hunyuan3D), auto-rigged, animated with three.js inside a transparent always-on-top WKWebView; calendar reminders, file shelf, screen snipping from the right-click menu. | `Swift` `three.js` `Hunyuan3D` |
| 📮 | **[gmail-digest](https://github.com/etherimirr/gmail-digest)** | Rules-first triage across several inboxes. The optional LLM pass must quote the email for every judgment it makes, no unsourced verdicts. | `Python` `Discord API` |

More on the [site](https://etherimirr.github.io#projects): a TLA+-verified distributed lock, an LLM-orchestrated quant system, a Pinyin AAC badge for ASD children on a Raspberry Pi, and an in-browser [facial profile analyzer](https://github.com/etherimirr/facial-profile-analyzer).

---

### Stack

**Languages**&nbsp;
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&labelColor=0D1117&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&labelColor=0D1117&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&labelColor=0D1117&logo=cplusplus&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-DEA584?style=flat-square&labelColor=0D1117&logo=rust&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&labelColor=0D1117&logo=swift&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&labelColor=0D1117&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-E76F00?style=flat-square&labelColor=0D1117&logo=openjdk&logoColor=white)

**Distributed &amp; backend**&nbsp;
![gRPC](https://img.shields.io/badge/gRPC-2E7D8F?style=flat-square&labelColor=0D1117&logo=trpc&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-2E7D8F?style=flat-square&labelColor=0D1117&logo=apachekafka&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-2E7D8F?style=flat-square&labelColor=0D1117&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2E7D8F?style=flat-square&labelColor=0D1117&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-2E7D8F?style=flat-square&labelColor=0D1117&logo=amazonwebservices&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-2E7D8F?style=flat-square&labelColor=0D1117&logo=mongodb&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-2E7D8F?style=flat-square&labelColor=0D1117&logo=duckdb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-2E7D8F?style=flat-square&labelColor=0D1117&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-2E7D8F?style=flat-square&labelColor=0D1117&logo=redis&logoColor=white)

**ML &amp; vision**&nbsp;
![PyTorch](https://img.shields.io/badge/PyTorch-7C3AED?style=flat-square&labelColor=0D1117&logo=pytorch&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-7C3AED?style=flat-square&labelColor=0D1117&logo=nvidia&logoColor=white)
![TensorRT](https://img.shields.io/badge/TensorRT-7C3AED?style=flat-square&labelColor=0D1117&logo=nvidia&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-7C3AED?style=flat-square&labelColor=0D1117&logo=opencv&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLOv8-7C3AED?style=flat-square&labelColor=0D1117&logo=yolo&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-7C3AED?style=flat-square&labelColor=0D1117&logo=meta&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude_SDK-7C3AED?style=flat-square&labelColor=0D1117&logo=anthropic&logoColor=white)

---

### Off the clock

Photography (Canon R6 Mark II, [gallery](https://etherimirr.github.io/photography.html)), bouldering, mapping my trips into the [atlas](https://etherimirr.github.io/atlas-of-wonders/), and drawing pixel worlds.
