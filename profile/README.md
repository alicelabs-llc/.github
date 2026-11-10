<div align="center">

# AliceLabs LLC

**Trust infrastructure for AI agents. Receipts, not vibes.**

[![Registry](https://img.shields.io/badge/registry-marketnow.site-00F299?style=for-the-badge&labelColor=07080f)](https://marketnow.site)
[![Stack](https://img.shields.io/badge/stack-utalabs.tech-00D1FF?style=for-the-badge&labelColor=07080f)](https://utalabs.tech)
[![Company](https://img.shields.io/badge/company-alicelabs.site-07080f?style=for-the-badge)](https://alicelabs.site)
[![Status](https://img.shields.io/website?url=https%3A%2F%2Fstatus.marketnow.site&label=status.marketnow.site&style=for-the-badge)](https://status.marketnow.site)

</div>

We build the infrastructure that answers one question: *should this agent be allowed to do that?* Identity, translation, audit and enforcement — every claim on this page links to a repo, a receipt or a spec. No security theater: if the authority can't be reached, the transaction doesn't happen (fail-closed).

## Project structure

**The stack — utalabs.tech**

| Repo | What it owns |
|------|--------------|
| [`MARKETNOW`](https://github.com/alicelabs-llc/MARKETNOW) | Trust registry & marketplace — 71,198+ MCP servers indexed, Sentinel-scanned, scores backed by verifiable receipts · [marketnow.site](https://marketnow.site) |
| [`universal-trust-adapter`](https://github.com/alicelabs-llc/universal-trust-adapter) | ATC/1.0 protocol: Ed25519-signed trust cards, RFC 8785 JCS, 10 verification controls · live x402 endpoint · conformance: `npx @marketnow/uta-conformance` |
| [`uta-ai`](https://github.com/alicelabs-llc/uta-ai) | Official agent surface: installable skills (agentskills.io), subagents, MCP servers, Claude Code plugin, live drift-check |
| [`marketnow-agent`](https://github.com/alicelabs-llc/marketnow-agent) | Universal agent plugin — Claude Code, Cursor, Grok Build, Gemini CLI, Qwen Code |
| [`marketnow-submissions`](https://github.com/alicelabs-llc/marketnow-submissions) | Public skill submissions queue — every submission Sentinel-scanned, stored and auditable |
| [`status`](https://github.com/alicelabs-llc/status) | Live status page for marketnow.site endpoints · [status.marketnow.site](https://status.marketnow.site) |

**Security tooling**

| Repo | What it owns |
|------|--------------|
| [`mcp-vault-server`](https://github.com/alicelabs-llc/mcp-vault-server) | Zero-trust key management MCP server — AES-256-GCM, circuit breaker, IAM labels |
| [`CodeAuditor`](https://github.com/alicelabs-llc/CodeAuditor) | Automated code security auditor — static analysis, vulnerability detection, report generation |
| [`burp-quicknotes`](https://github.com/alicelabs-llc/burp-quicknotes) | Structured bug-bounty report templates for Burp Suite — SSRF, IDOR, XSS, auth bypass |
| [`supabase-rls-templates`](https://github.com/alicelabs-llc/supabase-rls-templates) | Production-ready Row Level Security policies for Supabase — RBAC, multi-tenant |

**Data & GovTech**

| Repo | What it owns |
|------|--------------|
| [`ecuadorian-legal-codes`](https://github.com/alicelabs-llc/ecuadorian-legal-codes) | Machine-readable Ecuadorian legislation in JSON — COIP, COGEP, CC, CT, CRE, CNJ (3,847+ articles) |
| [`OpenSAM`](https://github.com/alicelabs-llc/OpenSAM) | Autonomous AI agent for federal contracting — SAM.gov opportunity discovery, scoring and bid automation |
| [`autotaxflow`](https://github.com/alicelabs-llc/autotaxflow) | Automated tax workflow engine for Ecuador — SRI integration, compliance automation |
| [`Rutas`](https://github.com/alicelabs-llc/Rutas) | Route management and logistics optimization engine for Ecuador and LatAm |
| [`LegalIA`](https://github.com/alicelabs-llc/LegalIA) | Legal AI suite for Ecuador and LatAm — 6-agent swarm, demandas I-IV, OCR, 3,847+ laws |

**Archived**

- `atc-spec` · `atc-verifier` — moved to [`universal-trust-adapter`](https://github.com/alicelabs-llc/universal-trust-adapter) (read-only).

Side projects (dropshipping tooling, ML demos and experiments) live in their own repos — the stack above is where active development happens.

## SLOTH — the overnight agent that hands you a receipt

[**sloth.utalabs.tech**](https://sloth.utalabs.tech) · [repo](https://github.com/eddyflores100-lang/sloth)

A 1B open-weight brain (Gemma 3 + llama.cpp) that runs on your CPU and does the boring stuff while you sleep. Every action lands on a SHA-256 hash chain, signed with Ed25519 — offline-verifiable by anyone in ~30 seconds, no account. Irreversible clicks stay human.

## Open source beyond the stack

- [**alethech**](https://github.com/eddyflores100-lang/alethech) — verifiable agent continuity: Ed25519-signed memory, hash-linked DAG, key rotation with reachability guarantee. Local-first, zero-LLM, zero-blockchain. [docs](https://alethech.alicelabs.site)
- [**sloptotal**](https://github.com/eddyflores100-lang/sloptotal) — open-source AI text detector: 23 engines, one calibrated score, every number measured on a public benchmark. [sloptotal.com](https://sloptotal.com)
- [**marketnow-memory**](https://github.com/alicelabs-llc/marketnow-memory) — persistent local memory for any MCP-compatible agent: single file, zero dependencies, no cloud, no telemetry.

## Contact

[alicelabs.site](https://alicelabs.site) · contacto@alicelabs.site · Wyoming, USA · Quito, Ecuador
