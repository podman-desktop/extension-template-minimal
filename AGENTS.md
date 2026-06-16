# AGENTS.md

## Project Overview

Minimal Podman Desktop extension template with a single TypeScript entrypoint.
It is intended as the smallest starting point for command/menu contributions and
simple extension lifecycle logic.

- **Tech stack**: TypeScript, Node.js, npm
- **Extension API**: `@podman-desktop/api`
- **Main entrypoint**: `src/extension.ts`

## Quick Start

```sh
npm install
npm run build
```

## Essential Commands

```sh
npm run build   # compile TypeScript into dist/
npm run watch   # incremental TypeScript rebuild
```

## Single-File Verification

```sh
npx eslint path/to/file.ts
npx tsc --noEmit path/to/file.ts
```

## Skills

Task-specific guidance lives in `.agents/skills/`:

- `extension-development` - adding commands, menus, and API usage
- `unit-testing` - lightweight Vitest testing patterns

## Architecture

- `src/extension.ts` registers extension logic and Podman Desktop API calls.
- `package.json` `contributes` section defines commands/menus/views.
- Built output is `dist/extension.js` loaded by Podman Desktop.

## Pattern References

- Add a command: `package.json` `contributes.commands` + handler in `src/extension.ts`
- Add menu item: `package.json` `contributes.menus` + command implementation
- Add config key: `package.json` `contributes.configuration`
