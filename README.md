# Vitalii Popov

**Senior AI Product Engineer.** LLM apps (RAG, agents, evals) on React, Next.js, Node.js and TypeScript. Remote B2B contractor.

I build product features end to end: six years of React and TypeScript (data-heavy tools, editors and real-time interfaces), and since 2025 Node.js services and APIs as well. Right now I own the operator-facing app of a B2B iGaming platform from the React frontend through its NestJS BFF. Before that I built an event-driven feeds platform in Node.js and the newsroom's rich-text editor for Paris Match on Contentful. At both I ship with a coding agent (Claude Code), set up with project instructions, hooks, subagents and MCP servers.

### Porter: an LLM product, built in public

**[Porter](https://github.com/Yeezy2277/porter)** ([live](https://porter.vitaliipopov.dev)) migrates a WordPress site into Contentful. Code converts every article and proves no word was lost; Claude does only the judgement calls:

- **Structured output:** field mapping chosen from a closed menu, checked in code, approved by a person.
- **RAG:** authors and topics linked by hybrid retrieval (Voyage embeddings in pgvector plus full-text search, Reciprocal Rank Fusion). 98% correct, 96% retrieval recall on 53 hand-labelled cases.
- **An agent:** a hand-written tool-use loop with turn and cost limits that fills each entry for a human review queue.
- **Evals in CI:** golden sets, code graders and an LLM judge tested against planted flaws.

It's my own product, not a rebuild of client work, and it builds on the Contentful work above.

That client code is under NDA, so the repos below rebuild the same patterns in public. Each one is deployed and has a demo you can use without reading the code. The full list is at **[vitaliipopov.dev](https://vitaliipopov.dev)**.

### Public rebuilds of client work

| Project | What it rebuilds | Live |
|---|---|---|
| **[Podium](https://github.com/Yeezy2277/podium)** | A multi-tenant promo back office: NestJS and Prisma API with brand-level access, scheduled campaign lifecycle, React and MUI DataGrid admin. | [podium.vitaliipopov.dev](https://podium.vitaliipopov.dev) |
| **[Wire](https://github.com/Yeezy2277/wire)** | The feeds pipeline I built at Paris Match: Contentful webhooks, deduplication, a queue and an idempotent worker that writes only changed feeds. | [wire.vitaliipopov.dev](https://wire.vitaliipopov.dev) |
| **[Lumen](https://github.com/Yeezy2277/cms-blog)** | A content platform on Contentful with a typed Next.js publication, webhooks, a scheduled audit and content-model migrations. | [lumen.vitaliipopov.dev](https://lumen.vitaliipopov.dev) |
| **[Rich Text Editor](https://github.com/Yeezy2277/cms-blog/tree/main/apps/rich-text-editor)** | A PlateJS editor for Contentful rich text with a round-trip-tested transform to Contentful's document JSON. | [rte.vitaliipopov.dev](https://rte.vitaliipopov.dev/?demo=1) |
| **[Editorial Toolkit](https://github.com/Yeezy2277/cms-blog/tree/main/apps/editorial-toolkit)** | One Contentful app with seven editor tools across four locations, running against a mock CMS. | [toolkit.vitaliipopov.dev](https://toolkit.vitaliipopov.dev/?demo=1) |
| **[Pulse](https://github.com/Yeezy2277/live-ops-console)** | A real-time console for a multiplayer game, painted on canvas at 60 fps outside React's render cycle. | [pulse.vitaliipopov.dev](https://pulse.vitaliipopov.dev) |
| **[Girder](https://github.com/Yeezy2277/bim-clash-viewer)** | A browser BIM viewer in three.js with a unit-tested engine for hard and clearance clashes. | [girder.vitaliipopov.dev](https://girder.vitaliipopov.dev) |
| **[Depot](https://github.com/Yeezy2277/depot)** | The backend half of a CMS: sessions, hashed delivery tokens and a typed Postgres content model. | [depot.vitaliipopov.dev](https://depot.vitaliipopov.dev) |

### Stack

LLM apps: Anthropic API (structured output, tool use, prompt caching), RAG (embeddings, pgvector, hybrid search), agents, evals, MCP, Claude Code.

React, Next.js (App Router), TypeScript, MUI, Node.js (NestJS, Express), Contentful (App Framework, migrations, webhooks), PlateJS, Java/Spring Boot (working proficiency), GCP, GitHub Actions.

### Contact

[LinkedIn](https://www.linkedin.com/in/vitalii-popov-front-dev), [vitaliipopov.dev](https://vitaliipopov.dev)
