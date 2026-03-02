# pdf-character-count

React + TypeScript + Vite project scaffolded with ESLint, Prettier, Husky, lint-staged, and Vitest.

## Prerequisites

- Node.js 18+ (Node 22.19.0 detected during setup)
- npm 10+ (npm 10.9.3 detected during setup)

## Install

```bash
npm install
```

## Scripts

- `npm run dev` – start Vite dev server
- `npm run build` – TypeScript build + Vite production build
- `npm run preview` – preview built app
- `npm run typecheck` – TypeScript type checking (no emit)
- `npm run lint` – run ESLint
- `npm run lint:fix` – run ESLint with auto-fix
- `npm run format` – format with Prettier
- `npm run format:check` – check formatting with Prettier
- `npm run test` – run Vitest in watch mode
- `npm run test:run` – run Vitest once (CI mode)

## Testing

Vitest is configured in `vite.config.ts` with a `jsdom` environment and `src/setupTests.ts` sets up `@testing-library/jest-dom`. A basic React Testing Library test lives in `src/App.test.tsx`.

## Linting & Formatting

- ESLint Flat Config is defined in `eslint.config.js` with React hooks, import ordering, accessibility, and unused-imports rules.
- Prettier is configured via `.prettierrc` and `.prettierignore`.

## Pre-commit hooks

Husky and lint-staged are configured (once the project is in a Git repo with `.git` present):

- `.husky/pre-commit` runs `npx lint-staged` and `npm run typecheck`.
- `lint-staged` formats and lints staged files.

## Project structure

- `src/` – React application source
- `src/App.tsx` – main app component
- `src/App.test.tsx` – example test
- `src/setupTests.ts` – test setup
