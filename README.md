# filament

A monorepo project using Turborepo, pnpm, and Astro.

## Getting Started

### Using DevContainer

This project is configured with a DevContainer that includes all necessary tools:
- Node.js
- pnpm
- Turbo
- just
- jq
- checksy

Open this repository in VS Code and use "Reopen in Container" to get started.

### Manual Setup

If not using the devcontainer, ensure you have:
- Node.js (>= 18.0.0)
- pnpm (9.15.0)
- just (optional, for using justfile commands)

Install dependencies:
```bash
pnpm install
```

## Available Commands

### Using just (recommended)
```bash
just build   # Build all packages
just dev     # Run development mode
just static  # Build static assets
```

### Using pnpm directly
```bash
pnpm run build   # Build all packages
pnpm run dev     # Run development mode
pnpm run static  # Build static assets
```

## Project Structure

```
.
├── apps/
│   └── pages/          # Astro static site
├── packages/
│   └── schema/         # Shared schema package
├── filaments/          # Future filament packages
└── turbo.json          # Turborepo configuration
```

## Workspace Packages

- **@filament/pages**: Astro static site generator
- **@filament/schema**: Shared TypeScript schema package