<div align="center">

<h1>Christina Yijing Jia</h1>

<p>
  <b>Distributed backend systems</b> &nbsp;·&nbsp; <b>LLM agent infrastructure</b>
</p>

<p>
  <code>M.S. Computer Engineering @ Columbia</code> &nbsp;
  <code>Dec 2026</code> &nbsp;
  <code>B.E. ECE @ UMich–SJTU JI</code>
</p>

<p>
  <a href="https://www.linkedin.com/in/christina-jia-36992b383/">
    <img src="https://img.shields.io/badge/LinkedIn-christina--yijing--jia-0A66C2?style=flat-square&labelColor=0D1117&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:yj2923@columbia.edu">
    <img src="https://img.shields.io/badge/Email-yj2923@columbia.edu-14B8A6?style=flat-square&labelColor=0D1117&logo=maildotru&logoColor=white" alt="Email">
  </a>
  <a href="https://etherimirr.github.io">
    <img src="https://img.shields.io/badge/Site-etherimirr.github.io-8B5CF6?style=flat-square&labelColor=0D1117&logo=githubpages&logoColor=white" alt="Site">
  </a>
</p>

</div>

---

I work on the unglamorous half of systems: the execution layer underneath, the part that has to
stay correct when things run concurrently and for a long time.

This summer I was a SWE intern on **TikTok Trust &amp; Safety — Algorithm Infra**, on the async execution
layer behind a safety-model evaluation platform. I re-architected a synchronous SSE path into
MongoDB-backed durable tasks — a 15-minute ceiling became 3-hour jobs — and extended a **Go DAG
engine** with async triggers, which is how I ended up tracking a production concurrency deadlock
across parallel SG/US runs.

<table>
<tr><td width="50%" valign="top">

**Interested in**
- Distributed systems &amp; backend infrastructure
- Low-latency and deterministic execution
- LLM agent tooling, ML systems

</td><td width="50%" valign="top">

**Looking for**
- 2027 New Grad SWE / ML / AI Infra (start Jan 2027)
- US-based, open to relocation

</td></tr>
</table>

---

### Selected work

| | Project | The hard part | Stack |
|---|---|---|---|
| ⚡ | **[mbook](https://github.com/etherimirr/mbook)** | Deterministic limit order book. O(1) dense tick ladder over a preallocated slab, nothing allocated on the hot path, replay verified by a digest over the ordered fill stream. | `C++17` `CMake` |
| 🔒 | **An-agent** *(private)* | Multi-agent assistant on the Claude Code SDK. Five-layer memory (procedural → working → episodic → semantic → persona), and a read-only digital twin with three-layer prompt-injection defense. | `Python` `SQLite/FTS5` `ChromaDB` |
| 🧭 | **[cs-interview-coach](https://github.com/etherimirr/cs-interview-coach)** | Local-first, sub-millisecond FST search over 140+ knowledge cards, with FSRS spaced repetition across five navigation views. | `Rust` `Tauri` `SvelteKit` |
| 📮 | **[gmail-digest](https://github.com/etherimirr/gmail-digest)** | Rules-first triage across several inboxes. The optional LLM pass must quote the email for every judgment it makes — no unsourced verdicts. | `Python` `Discord API` |
| 🎬 | **[xhs-bilibili-distill](https://github.com/etherimirr/xhs-bilibili-distill)** | One distillation pipeline, two source adapters: transcript + scene-detected key frames + structured report. | `Python` `FFmpeg` |
| 📊 | **[portfolio-insights-generator](https://github.com/etherimirr/portfolio-insights-generator)** | Transaction analytics with LLM-assisted insight generation and what-if scenario modeling. | `Python` `Streamlit` `pandas` |

---

### Stack

**Languages**&nbsp;
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&labelColor=0D1117&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&labelColor=0D1117&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&labelColor=0D1117&logo=cplusplus&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-DEA584?style=flat-square&labelColor=0D1117&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&labelColor=0D1117&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-E76F00?style=flat-square&labelColor=0D1117&logo=openjdk&logoColor=white)

**Distributed &amp; backend**&nbsp;
![gRPC](https://img.shields.io/badge/gRPC-2E7D8F?style=flat-square&labelColor=0D1117&logo=trpc&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-2E7D8F?style=flat-square&labelColor=0D1117&logo=apachekafka&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-2E7D8F?style=flat-square&labelColor=0D1117&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2E7D8F?style=flat-square&labelColor=0D1117&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-2E7D8F?style=flat-square&labelColor=0D1117&logo=amazonwebservices&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-2E7D8F?style=flat-square&labelColor=0D1117&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-2E7D8F?style=flat-square&labelColor=0D1117&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-2E7D8F?style=flat-square&labelColor=0D1117&logo=redis&logoColor=white)

**ML systems**&nbsp;
![PyTorch](https://img.shields.io/badge/PyTorch-7C3AED?style=flat-square&labelColor=0D1117&logo=pytorch&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-7C3AED?style=flat-square&labelColor=0D1117&logo=nvidia&logoColor=white)
![TensorRT](https://img.shields.io/badge/TensorRT-7C3AED?style=flat-square&labelColor=0D1117&logo=nvidia&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-7C3AED?style=flat-square&labelColor=0D1117&logo=meta&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude_SDK-7C3AED?style=flat-square&labelColor=0D1117&logo=anthropic&logoColor=white)

---

<div align="center">

<a href="https://github.com/etherimirr">
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=etherimirr&show_icons=true&hide_border=true&hide_title=true&include_all_commits=true&count_private=true&theme=transparent&icon_color=14B8A6&text_color=8B949E&hide=issues" alt="stats">
</a>
<a href="https://github.com/etherimirr">
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=etherimirr&layout=compact&hide_border=true&hide_title=true&langs_count=6&theme=transparent&text_color=8B949E" alt="languages">
</a>

</div>
