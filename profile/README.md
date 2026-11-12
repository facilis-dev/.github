<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/facilis-dev/facilis/main/brand/facilis-logo-inverse.svg">
    <img src="https://raw.githubusercontent.com/facilis-dev/facilis/main/brand/facilis-logo.svg" alt="facilis.dev" width="440">
  </picture>
</p>

<h3 align="center">The right way is the easy way.</h3>

<p align="center">
  <a href="https://ide.facilis.dev"><b>Open the IDE</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/facilis-dev/facilis">Framework</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/facilis-dev/facilis/blob/main/docs/SPEC.md">Spec</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/facilis-dev/facilis/blob/main/docs/STATUS.md">Status</a>
</p>

---

**facilis.dev** builds **Facilis** (lat. *easy*) — a framework for building web applications in the browser, where the generated project is ordinary, MIT-licensed TypeScript and the rules that keep it safe are enforced by the framework, not by code review.

A static IDE runs the project inside a WebContainer. `vite dev` is the single dev server, Nitro v3 runs as a Vite plugin, the database is PGlite. You chat with an AI to scaffold routes, schemas and pages, and every patch is checked against 19 rules before it touches disk.

## What we believe

| Principle | Meaning |
| --- | --- |
| **Security is the fast path** | A route cannot exist without an auth check and a declared table dependency; a table cannot exist without an RLS policy. Insecure code does not compile, and a bug in one layer is caught by the next. |
| **Code is the source of truth** | The UI visualises and proposes. It never becomes a second source of truth: no hidden schemas, no config panels, no round-tripping from visual to code. |
| **You can always escape** | Generated code is just code — edit it, delete it, replace it. No lock-in and no runtime you cannot see. |
| **Day one is a link** | One process, one port, one HMR loop. Clone to running, authenticated app in minutes, with no local setup. |

## Repositories

| Repository | What it is |
| --- | --- |
| [`facilis`](https://github.com/facilis-dev/facilis) | The monorepo: framework packages (`@facilis.dev/*`), the IDE, examples and the spec. MIT. |

The framework packages ship to npm under the `@facilis.dev` scope.

## The stack

TypeScript (strict, ESM) · Node ≥ 22.15 · pnpm + turbo · Vite · Nitro v3 · Drizzle + PGlite · Zod · React 19 · Tailwind CSS v4 + shadcn/ui (Base UI) · Vitest.

## Start here

- **Use it** — <https://ide.facilis.dev>: create a project, or clone your own repository.
- **The contract** — [`docs/SPEC.md`](https://github.com/facilis-dev/facilis/blob/main/docs/SPEC.md): architecture, endpoints, invariants. If it disagrees with anything else, it wins.
- **The state** — [`docs/STATUS.md`](https://github.com/facilis-dev/facilis/blob/main/docs/STATUS.md): implemented, open, retired, and the commands that prove it.
- **The why** — [`docs/DECISIONS.md`](https://github.com/facilis-dev/facilis/blob/main/docs/DECISIONS.md): the decision log.
- **Build on it** — [`docs/DEV.md`](https://github.com/facilis-dev/facilis/blob/main/docs/DEV.md) and [`AGENTS.md`](https://github.com/facilis-dev/facilis/blob/main/AGENTS.md).

## Status

Pre-MVP and developed in the open. The framework and the IDE work end to end, but the API is not frozen: expect breaking changes before 1.0. The spec, the decision log and the status page are part of the product — anything unfinished says so.

## License

MIT, © facilis-dev. Brand assets live in [`brand/`](https://github.com/facilis-dev/facilis/tree/main/brand).

<p align="center"><sub>Security reports: please contact a maintainer privately instead of opening a public issue.</sub></p>