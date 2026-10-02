# Code Snippet Manager

A lightweight, dependency-free TypeScript code snippet manager — save, search, organize, and export reusable code snippets from the terminal or any TypeScript/JavaScript project.

## Features

- **Snippet storage** — `StorageManager.ts.txt` handles saving, loading, and persisting snippets locally
- **Fast search** — `SearchManager.ts.txt` provides full-text search across snippet titles, tags, and code
- **Export** — `ExportManager.ts.txt` exports snippets to files for sharing or backup
- **Simple UI layer** — `UIManager.ts.txt` renders a minimal console/browser interface for browsing snippets
- **Shared types** — `Types and Main Entry 1/2.txt` define the core `Snippet` types and the main entry point
- **Build script** — `Compile TypeScript.sh` compiles the `.ts.txt` sources; `bash 1.sh` / `bash 2.sh` are quick utility scripts
- **User Guide** — plain-language walkthrough of everyday usage

## Tech Stack

- TypeScript (sources kept as `.ts.txt` for portability)
- Bash shell scripts
- `tsconfig.json` included for compilation
- MIT licensed

## Quick Start

1. Rename the snippet sources from `*.ts.txt` to `*.ts`, or reference them directly as text.
2. Compile with the included script:
   ```bash
   bash "Compile TypeScript.sh"
   ```
   (or `npx tsc` with the bundled `tsconfig.json`)
3. Import `StorageManager`, `SearchManager`, `ExportManager`, and `UIManager` from the main entry point and start adding snippets.

## Project Structure

```
.
├── Types and Main Entry 1.txt   # core types + entry point
├── Types and Main Entry 2.txt   # extended types
├── StorageManager.ts.txt        # persistence layer
├── SearchManager.ts.txt         # search layer
├── ExportManager.ts.txt         # export layer
├── UIManager.ts.txt             # UI layer
├── Compile TypeScript.sh        # build helper
├── bash 1.sh / bash 2.sh        # utility scripts
├── Project Structure.txt        # original structure notes
├── User Guide                   # usage walkthrough
├── tsconfig.json
└── LICENSE (MIT)
```

## Deploy Notes

Not a web app — no deployment target. Use it as a library of snippet-management building blocks in your own projects.

---

Built by Girish Lade — https://ladestack.in
