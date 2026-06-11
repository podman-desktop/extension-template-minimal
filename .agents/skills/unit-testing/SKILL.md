# Unit Testing

Use this guide when adding tests to the minimal template.

## Recommendation

- Use Vitest for unit tests.
- Mock `@podman-desktop/api` behavior at module boundaries.
- Focus tests on command handlers and side effects (notifications, config use).

## Suggested setup

If tests are introduced, add:

- `vitest` and `@types/node` dev dependencies as needed
- `npm test` script
- `*.spec.ts` files colocated with tested logic
