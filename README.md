# Ghost AI

A real-time collaborative workspace for designing system architectures. Describe your system in plain English, watch an AI agent build it live on a shared canvas, refine it with your team, and export a complete technical specification.

## How It Works

1. **Sign in** — Secure authentication via Clerk.
2. **Create a project** — Start a new architecture workspace or invite collaborators to an existing one.
3. **Prompt the AI** — Describe what you're building ("Design a real-time multiplayer platform with a microservices backend").
4. **Watch it build** — Google Gemini generates nodes and edges live on the shared canvas while your team watches.
5. **Refine together** — Drag nodes, edit labels, change colors, add edges, and see changes sync to all connected users in real-time.
6. **Generate specs** — One click converts your diagram into a detailed Markdown technical specification.
7. **Download** — Export specs as files for documentation, architecture reviews, or implementation.

## Tech Stack

- **Next.js 16** + **React 19** + **TypeScript** — Full-stack app with server/client boundaries and type safety.
- **Tailwind CSS v4** + **shadcn/ui** — Dark-themed, accessible component library.
- **Clerk** — Authentication and user management.
- **Prisma 7** + **PostgreSQL** — Relational database for projects, collaborators, and metadata.
- **Liveblocks** — Real-time synchronization: nodes, edges, cursors, presence, and avatars.
- **React Flow** + **@xyflow/react** — Interactive, resizable canvas with smart node/edge rendering (rectangle, cylinder, hexagon, circle, diamond, pill).
- **Trigger.dev** — Durable background tasks for AI generation and spec conversion.
- **Google Gemini 2.0** (via @ai-sdk/google) — LLM powering both architecture generation and spec synthesis.
- **Vercel Blob** — Storage for canvas snapshots and generated Markdown specs.

## Use Cases

- **Startup CTO** — Quickly validate system architecture with the team before a sprint without manual whiteboarding or tools.
- **Architecture Review** — Generate consistent, detailed technical specs from agreed-upon diagrams for compliance or onboarding.
- **Microservices Design** — Prototype service boundaries, data flows, and integrations collaboratively.
- **DevOps Planning** — Design CI/CD pipelines, infrastructure topology, and deployment strategies visually.
- **Documentation Automation** — Convert visual designs into Markdown specs automatically, reducing manual documentation overhead.
- **Multi-team Collaboration** — Real-time presence, cursors, and live AI feedback enable distributed teams to design together.
- **API & Integration Design** — Map out external services, webhooks, and data flows on a shared canvas.
- **Learning & Training** — Teach architecture patterns by importing starter templates and letting AI explain designs step-by-step.
