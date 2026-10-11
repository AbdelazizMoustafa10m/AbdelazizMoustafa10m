# Abdelaziz Abdelrasol

AI engineer at Vector Informatik in Stuttgart. I work on CAPLot, an AI coding agent for CAPL and CANoe, and on the evaluation, observability and deployment tooling around it. Before that I spent five years on embedded software, most of it automotive bootloaders.

[Blog](https://abdelaziznotes.com) · [LinkedIn](https://www.linkedin.com/in/abdelaziz-abdelrasol-aabab1b0/) · abdelazizmoustafa63@gmail.com

## At Vector

**CAPLot**, a coding agent for CAPL and CANoe. I designed its multi-agent workflow: a main implementation agent, a scout agent that searches the CAPL documentation, and an advisor agent the main agent consults on harder tasks. I also wrote its two agent skills, one for CAPL coding knowledge and one for using the CANoe compiler CLI. With them, the task compilation rate went from 53% to 100%. I've also extended the benchmark items and evaluation metrics.

**vRAGmate**, a microservice-based enterprise RAG system.

- Built the Langfuse trace retention and export service: async workflows, state and checkpoint management, Azure Blob Storage, Helm deployment and tests.
- Cut data-provider HTTP calls by 50–100x with batching and write-behind reporting, which ended the server overload during large operations.
- Moved 5+ services from local clients to a shared Python package with common utilities and CLI tooling.
- Led the architecture for a management UI covering access tokens, role assignments and namespaces. I compared four designs and wrote the C4 diagrams, ADRs and Kubernetes deployment plan.

## Open source

- [orchcore](https://github.com/AbdelazizMoustafa10m/orchcore) ([PyPI](https://pypi.org/project/orchcore/)): an async Python library that runs AI coding agent CLIs (Claude, Codex, Gemini, Copilot, OpenCode) as subprocesses in DAG-based phase pipelines. It normalizes their five JSONL stream formats into one event model and handles rate-limit recovery, checkpoint resume and clean shutdown.
- [planora](https://github.com/AbdelazizMoustafa10m/planora): a CLI and Textual TUI where one agent writes an implementation plan, other agents audit it in parallel, and the planner revises it over several rounds.
- [skills-for-agents](https://github.com/AbdelazizMoustafa10m/skills-for-agents): the agent skills I use with Claude Code and Codex CLI.
- [Raven](https://github.com/AbdelazizMoustafa10m/Raven) (Go): takes a PRD through task breakdown, implementation, multi-agent review, fixes and a pull request.
- [Harvx](https://github.com/AbdelazizMoustafa10m/Harvx) (Go): packages a repository into a context document for LLMs, with token budgeting and secret redaction.

## Writing

My most recent post is [Stop Letting LLMs Orchestrate Your AI Agents](https://abdelaziznotes.com/posts/stop-letting-llms-orchestrate-your-ai-agents). It compares interactive and headless agent orchestration using failure data from four multi-agent systems.

## Embedded work

| Company | Years | Work |
|---|---|---|
| Vector | 2023–2025 | Feature owner for Flash Bootloader (FBL) and On-the-Fly Reprogramming (OFR) in the Mercedes-Benz AP2 project |
| Bosch | 2022–2023 | HSM integration and deliveries with the BEST tool, through T&S |
| Valeo | 2021–2022 | Bootloaders for RH850, TriCore and ARM MCUs; Porsche ECU downgrade protection to VW requirements |
| EL-Araby Group | 2020 | Firmware for SHARP refrigerators and TOSHIBA vacuum cleaners on Renesas MCUs |

Some older C drivers are still here, for the [ATmega32A](https://github.com/AbdelazizMoustafa10m/ATmega32A-Device-Drivers) and the [TM4C123](https://github.com/AbdelazizMoustafa10m/TM4C123-Interface).

## Tools I use

Python (FastAPI, Pydantic, asyncio), TypeScript, C, CAPL. Langfuse, MLflow, OpenTelemetry. PostgreSQL, Qdrant, Redis, RabbitMQ. Docker, Helm, GitLab CI, Azure. CANoe, CAN, bootloaders, OFR and OTA, ASPICE.
