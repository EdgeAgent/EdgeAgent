<div align="center">

# EdgeAgent

### Building practical AI systems for people who need control, portability, and real-world reliability.

I build tools at the intersection of **local LLMs, autonomous workflows, human oversight, automation, and spatial computing**.

[Explore the portfolio](#featured-work) · [View the project map](#portfolio-map) · [Visit Edge Agency](https://edgeagency.pro)

</div>

---

## Portfolio map

The work is organized around one question: **how do we make powerful software understandable and useful to the person responsible for the outcome?**

<div align="center">

![Edge Agency portfolio map: local AI, spatial computing, automation, governance, and TraceForge](https://raw.githubusercontent.com/EdgeAgent/EdgeAgent/main/assets/edge-portfolio-map.svg)

</div>

## Featured work

These are the public repositories that best represent the current portfolio.

| Project | What it explores | Status |
|---|---|---|
| **[Awesome Generative AI 1000](https://github.com/EdgeAgent/awesome-generative-ai-1000)** | A curated catalogue of 1,000 game-changing AI and software frameworks organized for the future of generative AI. | Open collection |
| **[EDGE Agency Automation Portfolio](https://github.com/EdgeAgent/edge-automation-portfolio)** | A portfolio of 73+ n8n workflows covering lead generation, real estate, e-commerce, content, customer service, and integrations. | Open portfolio |
| **[EDGE Agency AI Governance](https://github.com/EdgeAgent/EDGE-AGENCY-AI-Governance)** | Practical governance materials for building AI systems with clearer boundaries, review paths, and operational accountability. | Open framework |
| **[n8n Automations](https://github.com/EdgeAgent/n8n-automations)** | A public automation workspace for reusable workflow experiments and integrations. | Public workspace |
| **[RELAY — Agent Swarm Protocol](https://github.com/EdgeAgent/relay-protocol)** | A compact, versioned message dialect for fast, safe communication between specialist agents inside n8n. | Design-ready framework |

## Private studio builds

Some of the most active product work remains private while it is being validated. **[ModelDock USB](https://github.com/EdgeAgent/modeldock-usb)** is a local LLM command center for inspectable business workflows, approval gates, audit logs, recovery controls, and portable execution. **[TraceForge](https://github.com/EdgeAgent/traceforge)** is an auditable AI framework for Ontario industrial sectors, with structured inference, confidence thresholds, human review, and traceable decisions.

## Featured project: ModelDock USB

[![ModelDock USB](https://img.shields.io/badge/Studio%20build-ModelDock%20USB-06b6d4?style=for-the-badge&logo=github)](https://github.com/EdgeAgent/modeldock-usb)

**ModelDock USB** is a local LLM command center for autonomous business workflows—with humans in control. It turns plain-language requests into inspectable workflows, routes work through specialist agents, pauses for approval when risk matters, and preserves an operational audit trail.

![ModelDock USB architecture: local model runtime, workflow planner, human approval desk, live monitoring, audit trail, and emergency stop](https://raw.githubusercontent.com/EdgeAgent/EdgeAgent/main/assets/modeldock-architecture.png)

| Built for | What it provides |
|---|---|
| **Local-first operators** | Offline execution, USB-local JSON persistence, loopback model health checks |
| **Cross-platform workflows** | Windows, macOS, and Linux launchers with USB-root-relative paths |
| **Human oversight** | Approval gates, audit logs, pause/resume, retries, timeouts, and emergency stop |
| **Model operators** | Platform-aware model discovery, read-only file scanning, and local setup validation |

### Why it matters

Most agent demos optimize for a successful answer. ModelDock optimizes for the operating loop around the answer: **start safely, inspect progress, review sensitive actions, recover from failure, and keep control**.

### Start here

```bash
git clone https://github.com/EdgeAgent/modeldock-usb.git
cd modeldock-usb
pnpm install
pnpm check
pnpm test
pnpm dev
```

→ **[Read the ModelDock USB README](https://github.com/EdgeAgent/modeldock-usb#readme)**

## Featured framework: RELAY

[![RELAY](https://img.shields.io/badge/Framework-RELAY-22d3ee?style=for-the-badge&logo=n8n&logoColor=white)](https://github.com/EdgeAgent/relay-protocol)

**RELAY** is a compact communication layer for an internal agent swarm. It is designed for the place where broad interoperability standards are not the bottleneck: one operator’s own n8n workflows, where messages need to be fast, inexpensive, versioned, and easy to audit.

The protocol uses a fixed positional envelope—`v|FROM|TO|INTENT|REF|PAYLOAD`—with a shared codebook for agent roles, intents, stages, and task types. Instead of repeating verbose JSON keys, agents exchange compact payloads such as `L:4471,S:82,ACT:CALL`. **HERALD** translates the wire format into readable logs and dashboards, while unknown codes fail safely through `ESC` and human review.

![RELAY agent swarm protocol architecture: SCOUT, QUALIFIER, COLDPEN, SHEPHERD, LEDGER, HERALD, operator dashboard, and safe human escalation](https://raw.githubusercontent.com/EdgeAgent/EdgeAgent/main/assets/relay-architecture.png)

| Protocol principle | What it provides |
|---|---|
| **Fixed envelope** | Predictable parsing with minimal repeated tokens across every message. |
| **Live codebook** | Versioned n8n Data Table shared by every agent and workflow. |
| **Compact payloads** | Short key-value pairs and enums for lead, task, and workflow state. |
| **Human translation** | HERALD turns compact messages into readable operational records. |
| **Safe fallback** | Unsupported versions or intents emit `ESC` rather than guessing. |

### Example message

```text
1|SC|CP|REQ|482|L:4471,S:82,ACT:CALL
```

→ **SCOUT** requests **COLDPEN** to act on lead `4471`, scored at `82%`, with a follow-up call as the next action.

### Why it matters

RELAY does not try to replace cross-vendor standards such as A2A. It occupies a narrower, practical layer: a cheap and predictable internal dialect for a known swarm, with a translation and escalation boundary that keeps the system understandable to its operator.

## What I am focused on

I am exploring how local models and agentic systems can become dependable operating tools rather than isolated demos. The work is centered on portable execution, transparent state, safety boundaries, and interfaces that make autonomy understandable to the person responsible for the outcome.

| Principle | Meaning in practice |
|---|---|
| **Local when possible** | Keep sensitive workflows close to the operator and make cloud use explicit. |
| **Human at the boundary** | Automation can prepare and coordinate; people decide when consequences matter. |
| **Inspectable by default** | Every meaningful action should have a status, a reason, and an audit trail. |
| **Portable by design** | A useful tool should not depend on one machine, one vendor, or one fragile setup. |
| **Honest about readiness** | Host validation, failure recovery, and security work matter more than a polished demo. |

## Connect with the work

Start with the public **[Visionary3D Studio](https://github.com/EdgeAgent/visionary3d-studio)**, explore the spatial work in **[SPLATwalk](https://github.com/EdgeAgent/SPLATwalk)**, or browse the automation catalogue in **[EDGE Agency Automation Portfolio](https://github.com/EdgeAgent/edge-automation-portfolio)**. Issues and pull requests are welcome when they improve operator control, reproducibility, accessibility, security, or cross-platform reliability.

<div align="center">

**Local models. Human oversight. Portable operations.**

</div>

## References

[1]: https://github.com/EdgeAgent/modeldock-usb "ModelDock USB repository"
[2]: https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-github-profile/about-your-profile-readme "GitHub profile README documentation"
