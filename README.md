# Atlas — Collaborative Knowledge & Productivity Platform

Portfolio-grade, Notion + Obsidian + Trello inspired app with:
- 📝 Block-based note editor
- ✅ Tasks & databases (table, kanban, calendar)
- 🌐 Realtime collaboration (multi-cursor, comments, presence)
- 🔗 Knowledge graph (links + backlinks + graph view)
- 🤖 AI assistant (summarize, tag, Q&A over workspace)
- 📦 Offline-first with JSON/ZIP export & import

---

## 🚀 Tech Stack

**Frontend**
- React + Vite + TypeScript
- TailwindCSS + shadcn/ui
- TipTap (editor)
- Dexie (IndexedDB) for offline
- D3.js / Cytoscape.js (graph)

**Backend**
- FastAPI (REST + WebSockets)
- SQLAlchemy / SQLModel + Alembic
- JWT Auth + Argon2 password hashing
- Redis (cache, queues)
- Postgres (Neon/Supabase free)

**Collaboration**
- Yjs (CRDTs) + y-websocket
- Presence & comments
- Role-based permissions (Owner/Editor/Viewer)

**AI**
- sentence-transformers (local embeddings)
- Qdrant (vector DB)
- RAG pipeline (retrieve → answer with citations)
- Summarize, auto-tag, rewrite tools

**Search**
- Meilisearch (Docker local, fast indexing)

**Infra / CI/CD**
- Docker Compose (local dev)
- GitHub Actions (lint, test, build)
- Vercel (frontend hosting, free)
- Cloudflare Tunnel (backend demo, free)

---

## 📅 Roadmap Checklist

### Phase A — Local-first MVP (Weeks 1–2)
- [ ] Scaffold monorepo (`apps/web`, `apps/server`, `packages/shared`, `docs`)
- [ ] React + Vite + TS frontend
- [ ] TailwindCSS + shadcn/ui setup
- [ ] TipTap editor: paragraph, heading, todo, code
- [ ] Local JSON storage (`workspace.json`)
- [ ] Dexie (IndexedDB) offline cache
- [ ] Export/Import (JSON/ZIP)
- [ ] Dark/light toggle
- [ ] Keyboard shortcuts

### Phase B — Server Backbone & DB (Weeks 3–4)
- [ ] FastAPI backend scaffold
- [ ] SQLite (dev) → Postgres (Neon/Supabase free)
- [ ] Alembic migrations
- [ ] JWT auth (register/login/refresh)
- [ ] REST APIs: Workspaces, Pages, Tasks, Members
- [ ] Meilisearch integration + indexing worker
- [ ] File uploads (local disk)

### Phase C — Realtime Collaboration (Weeks 5–6)
- [ ] Yjs integration for CRDT editing
- [ ] WebSocket server for sync
- [ ] Presence (multi-cursor, avatars)
- [ ] Persist `ydoc_blob` snapshots to DB
- [ ] Comments + mentions
- [ ] Roles/permissions (Owner, Editor, Viewer)

### Phase D — Knowledge Graph & Databases (Weeks 7–8)
- [ ] Backlinks (reverse links)
- [ ] Relation model (typed links between pages)
- [ ] Graph view (D3.js / Cytoscape.js)
- [ ] Database pages: Table, Kanban, Calendar
- [ ] Filters & queries (e.g., tasks due today)
- [ ] Page templates

### Phase E — AI Assistant & RAG (Weeks 9–10)
- [ ] Chunk + embed notes (sentence-transformers)
- [ ] Qdrant (local or free cloud) for vector storage
- [ ] RAG pipeline: retrieve → answer with citations
- [ ] Inline AI tools: Summarize, Auto-tag, Rewrite
- [ ] Auto-suggest backlinks

### Phase F — Polish & Demo (Weeks 11–12)
- [ ] Page export → Markdown, PDF
- [ ] Full workspace export → ZIP (JSON + MD + attachments)
- [ ] Accessibility (a11y) & performance passes
- [ ] CI/CD with GitHub Actions (lint/test/build/docker)
- [ ] Docs in `/docs`: Feature matrix, API docs, diagrams
- [ ] Record 2–3 min demo video (show collab, graph, AI Q&A)

---

## 🎯 Final Deliverables
- [ ] Clean README with screenshots, diagrams, badges
- [ ] Architecture diagram + sequence diagram
- [ ] Demo video link
- [ ] “Run locally in 5 minutes” guide (docker-compose + npm)
- [ ] Public GitHub repo

---
