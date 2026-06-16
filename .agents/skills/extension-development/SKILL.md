# Extension Development

Use this guide when adding or changing extension behavior.

## Core flow

1. Declare user-facing integration in `package.json` under `contributes`.
2. Implement behavior in `src/extension.ts`.
3. Keep commands small and delegate reusable logic to helper functions.

## Common tasks

- Add command: `contributes.commands` + API command registration.
- Add menu action: `contributes.menus` entry that invokes a command.
- Add settings: `contributes.configuration` and read with extension API.

## Validation

```sh
npm run build
npx tsc --noEmit src/extension.ts
```
