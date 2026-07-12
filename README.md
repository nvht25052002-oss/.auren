<div align="center">

<img src="https://img.shields.io/badge/AuRen%20OS-AI%20Agent%20Platform-00cfab?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBkPSJNMyAyMEwxMiAzTDIxIDIwSDE2TDEyIDEyLjVMOCAyMEgzWiIgZmlsbD0iIzAwY2ZhYiIvPjwvc3ZnPg==&logoColor=white&labelColor=0d0e14" alt="AuRen OS" />

```
 █████╗ ██╗   ██╗██████╗ ███████╗███╗   ██╗    ██████╗ ███████╗
██╔══██╗██║   ██║██╔══██╗██╔════╝████╗  ██║   ██╔═══██╗██╔════╝
███████║██║   ██║██████╔╝█████╗  ██╔██╗ ██║   ██║   ██║███████╗
██╔══██║██║   ██║██╔══██╗██╔══╝  ██║╚██╗██║   ██║   ██║╚════██║
██║  ██║╚██████╔╝██║  ██║███████╗██║ ╚████║██╗╚██████╔╝███████║
╚═╝  ╚═╝ ╚═════╝ ╚═╝  ╚═╝╚══════╝╚═╝  ╚═══╝╚═╝ ╚═════╝ ╚══════╝
```

### 🦞 AI Agent Platform — Built by the Community

[![License](https://img.shields.io/badge/License-MIT-00cfab?style=flat-square&labelColor=0d0e14)](LICENSE)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-3178c6?style=flat-square&labelColor=0d0e14&logo=typescript)](https://www.typescriptlang.org)
[![Node.js](https://img.shields.io/badge/Node.js-24-339933?style=flat-square&labelColor=0d0e14&logo=nodedotjs)](https://nodejs.org)
[![pnpm](https://img.shields.io/badge/pnpm-workspace-f69220?style=flat-square&labelColor=0d0e14&logo=pnpm)](https://pnpm.io)
[![React](https://img.shields.io/badge/React-19-61dafb?style=flat-square&labelColor=0d0e14&logo=react)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-6-646cff?style=flat-square&labelColor=0d0e14&logo=vite)](https://vitejs.dev)

</div>

---

## 🌐 Live Applications

| App | Path | Description |
|-----|------|-------------|
| 🚀 **AuRen Workspace** | `/workspace/` | AI agent development IDE with chat, tools, extensions |
| 🧩 **AuRenHub** | `/aurenhub/` | Community marketplace for skills & plugins |
| 📊 **AI Platform Dashboard** | `/` | Analytics dashboard for AI dev platforms 2024–2026 |
| 🎨 **AI Platforms Slides** | `/ai-platforms-slides/` | Professional slide deck on AI landscape |
| 🔧 **Debug Loop Simulator** | `/simulator/` | Self-healing debug loop visualizer |
| ⚡ **API Server** | `/api/` | Express 5 REST API with OpenAPI contract |
| 🌐 **Portal** | `/aurenhub/portal` | Unified portal linking all apps |

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🤖 AuRen Workspace
- **AI Agent Chat** — Real-time conversation with self-improving AI
- **Debug Loop** — Detect → Patch → Verify automation
- **Extensions** — VSCode-style marketplace with 30+ extensions
- **Tools Library** — 50+ tools across 6 categories
- **Projects** — Full project management with ZIP export
- **Authentication** — Mandatory login with GitHub/Google/Email

</td>
<td width="50%">

### 🧩 AuRenHub
- **Skills Marketplace** — 16 community-built skills
- **Plugin Ecosystem** — 12 one-click installable plugins
- **GitHub OAuth** — Full GitHub authentication flow
- **Publisher Profiles** — 8 verified publishers
- **Search & Filter** — Real-time filtering by tags & categories
- **Portal Hub** — Unified app launcher for all AuRen tools

</td>
</tr>
</table>

---

## 🏗️ Architecture

```
auren-os/                           # pnpm monorepo
├── artifacts/
│   ├── auren-workspace/            # 🚀 Main AI workspace (React + Vite)
│   │   ├── src/pages/              # landing, workspace, tools, library, etc.
│   │   ├── src/components/         # Sidebar, MobileNav, AuRenMascot
│   │   └── src/hooks/useAuth.ts    # localStorage auth system
│   │
│   ├── aurenhub/                   # 🧩 Skills & plugins marketplace (React + Vite)
│   │   ├── src/pages/              # home, skills, plugins, publishers, portal
│   │   ├── src/components/         # Navbar, Drawer
│   │   ├── src/data/catalog.ts     # Skills & plugins data
│   │   └── src/hooks/useAuth.ts    # GitHub OAuth auth system
│   │
│   ├── ai-platform-dashboard/      # 📊 Analytics dashboard (React + Vite + Recharts)
│   ├── ai-platforms-slides/        # 🎨 Slide deck artifact
│   ├── debug-simulator/            # 🔧 Self-healing loop visualizer
│   ├── api-server/                 # ⚡ Express 5 REST API
│   └── mockup-sandbox/             # 🎭 Component preview server (dev-only)
│
├── lib/
│   ├── api-spec/                   # OpenAPI 3.1 contract (SSOT)
│   ├── api-client-react/           # Generated React Query hooks
│   ├── api-zod/                    # Generated Zod schemas
│   └── db/                         # Drizzle ORM + PostgreSQL schema
│
├── scripts/                        # Utility scripts
├── tsconfig.base.json              # Shared TypeScript config
└── pnpm-workspace.yaml             # Workspace catalog & settings
```

---

## 🎨 Design System

```
Color Palette:
  Background:  #080809 / #0d0e14   Dark near-black
  Cards:       #0f0f12 / #16171e   Elevated surfaces
  Accent:      #00cfab             AuRen teal (primary)
  Text:        #e8eaf2             Primary text
  Muted:       #8892a4             Secondary text

Typography:    Inter (system-ui fallback)
Mascot:        Custom kawaii SVG crab — rounded, big eyes, rosy cheeks
```

---

## 🚀 Getting Started

### Prerequisites
- **Node.js** 24+
- **pnpm** 9+
- **PostgreSQL** (auto-provisioned on Replit)

> **Note for Replit users:** `.replit` is excluded from version control (it is Replit-specific platform config). When opening this repo on Replit, the platform recreates `.replit` automatically from `artifact.toml` service definitions — no manual setup needed.

### Installation

```bash
# Clone the repository
git clone https://github.com/dotcom-03/auren-os.git
cd auren-os

# Install dependencies
pnpm install

# Set up environment variables
cp .env.example .env
# Edit .env with your DATABASE_URL and SESSION_SECRET

# Push database schema
pnpm --filter @workspace/db run push

# Start all services
pnpm --filter @workspace/api-server run dev
pnpm --filter @workspace/auren-workspace run dev
pnpm --filter @workspace/aurenhub run dev
```

### Generate API types from spec

```bash
# After modifying lib/api-spec/openapi.yaml:
pnpm --filter @workspace/api-spec run codegen
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Runtime** | Node.js 24, TypeScript 5.9 |
| **Package Manager** | pnpm workspaces (monorepo) |
| **Frontend** | React 19, Vite 6, Wouter, Framer Motion |
| **Styling** | Tailwind CSS v4 + inline styles |
| **API** | Express 5, OpenAPI 3.1 (contract-first) |
| **Database** | PostgreSQL + Drizzle ORM |
| **Validation** | Zod v4 + drizzle-zod |
| **Code Generation** | Orval (React Query hooks + Zod schemas) |
| **Build** | esbuild (API), Vite (frontends) |
| **Logging** | Pino + pino-http |

---

## 📁 Key Commands

```bash
# Development
pnpm --filter @workspace/auren-workspace run dev      # Workspace (port 20860)
pnpm --filter @workspace/aurenhub run dev             # AuRenHub (port 19113)
pnpm --filter @workspace/api-server run dev           # API (port 5000)

# Quality
pnpm run typecheck                                    # Full typecheck
pnpm run build                                        # Build all packages

# Database
pnpm --filter @workspace/db run push                  # Push schema changes

# API
pnpm --filter @workspace/api-spec run codegen         # Regenerate API types
```

---

## 🤝 Contributing

We welcome contributions from the community! Here's how to get started:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feat/your-skill-name`
3. **Build** your skill or plugin following the AuRenHub spec
4. **Submit** a pull request with a clear description

### Building a Skill

Skills are self-contained modules that extend AuRen's capabilities:

```typescript
// Example skill structure
export const mySkill = {
  name: "My Awesome Skill",
  version: "1.0.0",
  description: "What this skill does",
  tags: ["automation", "productivity"],
  run: async (input: string) => {
    // Your skill logic here
    return { result: "Done!" };
  }
};
```

---

## 📊 Project Stats

```
Languages:     TypeScript 94% · CSS 4% · Other 2%
Artifacts:     7 (5 web apps + 1 API + 1 sandbox)
Total Pages:   25+
Components:    50+
API Endpoints: 15+
```

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**Built with 🦞 by the AuRen OS community**

[![Portal](https://img.shields.io/badge/Portal-All%20Apps-00cfab?style=for-the-badge&labelColor=0d0e14)](https://04e39574-267a-4b0c-ac60-41c28b84a950-00-3nkcqof30z1w2-squc36sb.sisko.replit.dev/aurenhub/portal)
[![Workspace](https://img.shields.io/badge/Workspace-Open-00cfab?style=flat-square&labelColor=0d0e14)](https://04e39574-267a-4b0c-ac60-41c28b84a950-00-3nkcqof30z1w2-squc36sb.sisko.replit.dev/workspace/)
[![Hub](https://img.shields.io/badge/AuRenHub-Explore-818cf8?style=flat-square&labelColor=0d0e14)](https://04e39574-267a-4b0c-ac60-41c28b84a950-00-3nkcqof30z1w2-squc36sb.sisko.replit.dev/aurenhub/)

*AuRen OS is not affiliated with Anthropic.*

</div>
