# Raj Kushwaha

Backend engineer who builds systems meant to run in production, not just demo well. Currently deepening into distributed systems, cloud infrastructure, and applied AI engineering.

[Featured projects ↓](#featured-engineering-projects)

## Engineering Snapshot

- **Role** — Backend Engineer, Full Stack Engineer, GenAI Developer
- **Focus** — Backend systems, distributed architecture, AI-powered applications
- **Background** — Computer Science Engineering student

## Currently Engineering

- Designing REST APIs with clear authentication and authorization boundaries
- Studying distributed systems patterns — caching, service boundaries, message-driven communication
- Building AI-powered applications with LangChain, RAG pipelines, and vector databases
- Learning containerized deployment workflows — Docker, AWS, GitHub Actions CI/CD

## Engineering Principles

- An API's contract gets designed before its implementation exists.
- Code is read far more than it's written — clarity is a feature, not an afterthought.
- Performance work starts with a measurement, not a guess.
- A task done manually more than twice becomes a script.
- Complexity earns its place only after the problem has justified it.
- A system that degrades predictably beats one that's merely fast.
- Documentation ships with the code, not after it.

## Featured Engineering Projects

### BlitzCore AI — Real-Time AI Chat Application

**Problem** — A raw chat interface needed to hold up under real usage: consistent message state, live typing feedback, and properly rendered AI output.

**Stack** — React, Redux Toolkit, Socket.IO, react-markdown + remark-gfm

**Architecture** — Feature-sliced Redux structure with a custom `useChat` hook wrapping the Socket.IO layer, behind a dashboard UI built around a consistent dark, glass-panel visual system.

**Engineering decisions** — Chat state isolated into its own Redux slice rather than colocated with UI state, keeping the socket layer swappable from the components that consume it.

**Interesting challenge** — A typing indicator that never cleared, traced to a missing `setLoading(false)` inside a `finally` block — async cleanup needs a guaranteed exit path, not just a happy-path handler. A second bug, a mismatch between `"ai"` and `"assistant"` role keys breaking message rendering, was found the same way: reasoning through state transitions rather than guessing.

**Repository** — link to be added

---

### E-Cell RGPV — Entrepreneurship Cell Website *(contributor)*

**Problem** — The events and gallery pages needed to feel like a living site, not a static brochure.

**Stack** — Next.js, React, Tailwind CSS

**Architecture** — An `EventsTimeline` component connecting event cards through SVG bezier paths in a zigzag layout; a canvas-based 3D tag cloud (`TagCloud3D`) using Fibonacci sphere distribution for even point spacing, with drag-to-rotate and scroll-to-zoom; a gallery with category filters and a bento grid, backed by a lightbox that supports keyboard navigation and respects reduced-motion settings.

**Interesting challenge** — Distributing tags evenly across a sphere without clustering at the poles, solved with Fibonacci sphere sampling, then layering in interaction (drag, zoom, hover) without breaking accessibility for users who need reduced motion.

**Repository** — link to be added

---

### AI Multi-Agent Orchestration System *(in progress)*

**Problem** — Exploring whether a single natural-language prompt can be decomposed and routed to specialized AI agents instead of handled by one generic assistant.

**Stack** — Node.js, Express, MongoDB (Mongoose)

**Architecture** — Planner, Frontend Dev, Backend Dev, and Reviewer agent roles; JWT + bcrypt authentication; `Team` and `TeamMember` schemas with embedded member arrays and role management.

**Status** — Authentication and data modeling are in place; agent orchestration logic is still being built out.

---

### Also Building

- **AI Resume Analyzer** — an AI-powered application for evaluating resumes.
- **Real-Time Bus Tracking System** — a real-time location tracking application.

*(Case studies for these will expand once repositories are linked.)*

## Engineering Toolkit

**Languages** — C++, JavaScript, TypeScript, Python

**Backend** — Node.js, Express.js, REST APIs, JWT, Socket.IO, Microservices

**Frontend** — React, Next.js, Tailwind CSS

**Databases** — MongoDB, PostgreSQL, Redis

**Cloud & DevOps** — Docker, AWS, GitHub Actions, CI/CD, Linux

**AI** — LangChain, LangGraph, Google Gemini API, OpenAI API, RAG, Vector Databases

## System Thinking

```
Client (React)
      │
      ▼
REST / Socket Gateway
      │
      ▼
Auth Middleware (JWT)
      │
      ▼
Business Logic
      │
      ├──► Redis Cache
      │
      ▼
Database (MongoDB / PostgreSQL)
```

## GitHub Activity

<img src="https://github-readme-stats.vercel.app/api?username=rajkushwaha-01&show_icons=true&hide_border=true&theme=default" width="49%" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rajkushwaha-01&layout=compact&hide_border=true&theme=default" width="49%" />

## Competitive Programming

750+ problems solved across DSA practice, 250+ of them on LeetCode — worked consistently rather than in bursts.

## Open Source

Interested in contributing to open-source projects, particularly backend tooling and AI infrastructure. Not yet a maintainer or regular contributor — a deliberate next step, not a current claim.

## Connect

[GitHub](https://github.com/rajkushwaha-01) · [LinkedIn](https://www.linkedin.com/in/raj-kushwaha-a703a1390)
