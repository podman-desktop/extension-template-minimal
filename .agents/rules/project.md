## Scope

Applies to all files in this repository.

## Rules

- Keep extension entrypoint logic in `src/extension.ts`.
- Register commands/menus/configuration in `package.json` `contributes`.
- Use `@podman-desktop/api` for Podman Desktop integration points.
- Keep startup logic fast and avoid blocking activation.
