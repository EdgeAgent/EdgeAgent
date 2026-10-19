<p align="center">
  <img src="assets/edge-profile-banner.png" alt="EDGE | AGENCY — AI systems and automation engineering" width="100%" />
</p>

<h1 align="center">Kevin Doherty</h1>
<h3 align="center">AI Systems Engineer &amp; Automation Architect · EDGE | AGENCY</h3>

<p align="center">
  <a href="https://edgeagency.pro">Portfolio</a> ·
  <a href="https://github.com/EdgeAgent?tab=repositories">GitHub Projects</a> ·
  <a href="https://edgeagency.pro">Contact</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AI%20Systems-Agent%20%26%20Multi--Agent-ff6b35?style=for-the-badge&logo=openai&logoColor=white" alt="AI systems and multi-agent" />
  <img src="https://img.shields.io/badge/Automation-n8n%20%7C%20MCP-ff8a3d?style=for-the-badge&logo=n8n&logoColor=white" alt="n8n and MCP automation" />
  <img src="https://img.shields.io/badge/Engineering-APIs%20%7C%20Developer%20Tools-18b8d4?style=for-the-badge&logo=github&logoColor=white" alt="APIs and developer tools" />
</p>

I build production AI and automation systems. My work connects agents, APIs, and business operations across **multi-agent orchestration, n8n workflows, MCP servers, developer productivity tools, and full-stack applications**—with a focus on clear interfaces, bounded actions, and systems people can understand and operate.

I’m interested in **AI Automation Engineer, Solutions Engineer, and Developer Productivity Engineer** roles. I bring product-minded engineering from problem framing through implementation, integration, and documentation.

## Technology toolkit

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI" />
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white" alt="n8n" />
  <img src="https://img.shields.io/badge/MCP-Tool%20Integrations-ff6b35?style=flat-square" alt="Model Context Protocol" />
  <img src="https://img.shields.io/badge/Cloud-Infrastructure-18b8d4?style=flat-square&logo=icloud&logoColor=white" alt="Cloud infrastructure" />
  <img src="https://img.shields.io/badge/Chrome-Extensions-4285F4?style=flat-square&logo=googlechrome&logoColor=white" alt="Chrome extensions" />
  <img src="https://img.shields.io/badge/Full--Stack-Product%20Engineering-20232A?style=flat-square&logo=visualstudiocode&logoColor=white" alt="Full-stack development" />
</p>

**Core strengths:** agent and workflow architecture · REST APIs and webhooks · MCP tool interfaces · human-in-the-loop controls · secure browser tooling · service integration · CI/CD · technical documentation.

## Selected work

| Project | Overview | Stack / focus |
| --- | --- | --- |
| [JARVIS Department Agent](https://github.com/EdgeAgent/jarvis-department-agent) | FastAPI agent service with bounded department managers, approval gates, n8n contracts, and local voice-response support. | Python · FastAPI · AI agents · n8n |
| [EDGE Automation Portfolio](https://github.com/EdgeAgent/edge-automation-portfolio) | 73+ categorized n8n workflow blueprints covering lead generation, real estate, e-commerce, content, service, and integrations. | n8n · APIs · webhooks · workflow design |
| [Flagship n8n Automations](https://github.com/EdgeAgent/EDGE-AGENCYAutomations-n8n) | Documented examples for AI-assisted content, executive assistance, video workflows, and SDR lead qualification. | n8n · OpenAI · SaaS integrations |
| [GHL Pro MCP](https://github.com/EdgeAgent/ghl-pro-mcp) | MCP server connecting AI tools to GoHighLevel CRM workflows and analytics. | MCP · APIs · CRM |
| [Client API Vault Relay](https://github.com/EdgeAgent/client-api-vault-relay-chrome-extension) | Manifest V3 extension with a locally encrypted API vault, exact-origin approval, and source-attributed provider discovery. | TypeScript/JavaScript · Chrome · security |
| [API Scout](https://github.com/EdgeAgent/api-scout) | Local-first catalog and CLI for discovering free APIs and free-tier LLM providers. | Developer tooling · APIs · local-first |

## System design

I favor clear boundaries over opaque “magic”: an explicit entry point, a scoped orchestrator, narrowly defined agent and tool capabilities, and an approval checkpoint where actions need human judgment. Integrations use stable contracts, and logs capture outcomes for debugging and handoff.

<p align="center">
  <img src="assets/ai-automation-architecture.png" alt="AI automation architecture: entry points, orchestration, AI agents and MCP tools, business systems, approval, and observability" width="100%" />
</p>

<details>
<summary><strong>Architecture source (Mermaid)</strong></summary>

```mermaid
flowchart LR
  subgraph INPUT["01 · Entry points"]
    EVT[User request / event]
    UI[App / browser extension]
    WH[Webhook / schedule]
  end
  subgraph CONTROL["02 · Orchestration"]
    API[Python / TypeScript service]
    N8N[n8n workflow]
    GATE{Approval gate}
  end
  subgraph INTEL["03 · AI & tools"]
    AGENT[Scoped AI agent]
    MCP[MCP server]
    APIX[External APIs]
  end
  subgraph OPS["04 · Operations"]
    SYS[Business systems]
    OBS[Logs · outcomes · retries]
  end
  EVT --> API
  UI --> API
  WH --> N8N
  API <--> N8N
  API --> AGENT
  N8N --> AGENT
  AGENT --> MCP
  MCP --> APIX
  APIX --> SYS
  AGENT --> GATE
  GATE -->|Approved| APIX
  GATE -->|Review| EVT
  API --> OBS
  N8N --> OBS
  APIX --> OBS
```
</details>

## Getting started with the projects

- **n8n workflows:** clone the [portfolio](https://github.com/EdgeAgent/edge-automation-portfolio), select a workflow under `workflows/`, import its JSON into n8n, configure the required credentials in n8n’s credential manager, then test with representative data before activation.
- **Flagship automations:** clone [EDGE-AGENCYAutomations-n8n](https://github.com/EdgeAgent/EDGE-AGENCYAutomations-n8n), choose a documented workflow, import the JSON, configure only its required integrations, and validate triggers and approval steps before enabling production runs.
- **Agent service:** use the [JARVIS Department Agent README](https://github.com/EdgeAgent/jarvis-department-agent) for environment setup and local run instructions; it documents the service-specific requirements.

Keep secrets in environment configuration or the platform’s credential store—never in committed workflow exports. Validate API permissions, failure handling, and review gates in a test environment before connecting live systems. Project-specific runtime and deployment instructions remain authoritative in each repository.

## Engineering principles

**Inspectable by default.** I aim to make capabilities, assumptions, and system boundaries visible. Practical delivery means a reproducible setup, scoped integrations, useful error handling, clear docs, and appropriate human review—not just an impressive demo.

---

<p align="center"><sub>EDGE | AGENCY · Practical AI systems, thoughtful automation, better developer workflows.</sub></p>
