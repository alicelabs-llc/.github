<div align="center">

# AliceLabs LLC

**Trust infrastructure for AI agents. Receipts, not vibes.**

[![Stack](https://img.shields.io/badge/stack-utalabs.tech-B08968?style=for-the-badge)](https://utalabs.tech)
[![Registry](https://img.shields.io/badge/registry-marketnow.site-A16207?style=for-the-badge)](https://marketnow.site)
[![Company](https://img.shields.io/badge/company-alicelabs.site-6B4F3A?style=for-the-badge)](https://alicelabs.site)
[![Status](https://img.shields.io/badge/status-status.marketnow.site-5F8D4E?style=for-the-badge)](https://status.marketnow.site)

</div>

Construimos la infraestructura que responde una sola pregunta: *¿debería permitírsele a este agente hacer eso?* Identidad, traducción, auditoría y ejecución — cada afirmación enlaza a un repo, un recibo o una especificación. Sin teatro de seguridad: si la autoridad no responde, el gasto no ocurre (fail-closed).

## El stack — utalabs.tech

| Capa | Producto | Qué es | Prueba |
|---|---|---|---|
| 01 · traducción | [**UTA**](https://utalabs.tech/uta/) | 8 formatos de credenciales entran (JWT, W3C VC, A2A, X.509, ATC…), un esquema canónico sale. Verificación de 12 etapas. | [API x402](https://uta-trust-api.eddyflores100.workers.dev) — $0.01/verificación |
| 02 · identidad | [**ATC**](https://utalabs.tech/atc/) | Tarjeta de capacidades firmada con Ed25519 (ATC/1.0, RFC 8785 JCS). | 57 tarjetas vivas · revocación MNR-CRL-1.0 |
| 03 · auditoría | [**Sentinel**](https://utalabs.tech/sentinel/) | 10 capas estáticas + sandbox real: cada servidor MCP se ejecuta bajo gVisor con syscalls vigiladas 30 s. | 1.211.488 chequeos · 1.030 amenazas cazadas |
| 04 · ejecución | [**Interceptor**](https://utalabs.tech/interceptor/) | Política en runtime: bloquea `.env` y `rm -rf` aunque la tarjeta del llamador sea válida. | 5 reglas vivas · auditoría JSONL firmada |
| lado del operador | [**UTA-Shield**](https://wall.utalabs.tech) | Firewall para operadores de servidores MCP: gates de identidad, threat-intel, DLP, metering x402. 19,8 kB, cero dependencias. | [repo](https://github.com/eddyflores100-lang/uta-shield) |
| registro | [**MarketNow**](https://marketnow.site) | Registro y marketplace: skills, credenciales y dominios verificados en 68.388 servidores MCP indexados. | API MCP gratuita, 9 tools, sin registro · [status](https://status.marketnow.site) |

Spec canónica del protocolo: [alicelabs-llc/universal-trust-adapter](https://github.com/alicelabs-llc/universal-trust-adapter) — ATC/1.0 + verificador UTA, conformance en un comando (`npx @marketnow/uta-conformance`). Superficie oficial para agentes: [uta-ai](https://github.com/alicelabs-llc/uta-ai).

## SLOTH — el agente nocturno que te deja un recibo

[**sloth.utalabs.tech**](https://sloth.utalabs.tech) · [repo](https://github.com/eddyflores100-lang/sloth)

Un cerebro abierto de 1B (Gemma 3 + llama.cpp) que corre en tu CPU, hace el trabajo aburrido mientras duermes y te entrega un recibo firmado en el desayuno: cadena SHA-256 eslabón por eslabón, firma Ed25519 y verificación completa en tu navegador en ~30 segundos, sin cuenta y sin confiar en nadie. Los clics irreversibles se quedan en manos humanas: anoche rechazó 5 acciones por su cuenta.

## Código abierto más allá del stack

- [**alethech**](https://github.com/eddyflores100-lang/alethech) — continuidad verificable de agentes: memoria firmada Ed25519, DAG encadenado, rotación de llaves con garantía de alcanzabilidad. Local-first, cero LLM, cero blockchain. [docs](https://alethech.alicelabs.site)
- [**security-toolkit**](https://github.com/alicelabs-llc/security-toolkit) — 10 servidores MCP para seguridad de IA/LLM.
- [**sloptotal**](https://github.com/eddyflores100-lang/sloptotal) — detector de texto IA de código abierto: 23 motores, un puntaje calibrado, cada número medido en un benchmark público. [sloptotal.com](https://sloptotal.com)
- [**marketnow-memory**](https://github.com/alicelabs-llc/marketnow-memory) — memoria local persistente para cualquier agente compatible con MCP: un solo archivo.
- [**marketnow-submissions**](https://github.com/alicelabs-llc/marketnow-submissions) — cola pública de submissions: cada skill escaneada por Sentinel, almacenada y auditable.

## Contacto

[alicelabs.site](https://alicelabs.site) · contacto@alicelabs.site · Wyoming, USA · Quito, Ecuador
