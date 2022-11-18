# turborepo-tailwindcss

A sample setup of a Turborepo monorepository with shared Tailwind CSS configurations.

## Installation

1. Install all the dependency packages found in the `package.json` files across the monorepo apps by running `pnpm i` from the project root directory.
2. To start the development servers of all the applications in your monorepo in parrallel, simply run `pnpm dev`. To start an individual app the monorepo, run:
   `pnpm i --filter <name> dev` (_name_: is found/set in the package.json for each individual app folder)

## Apps & Packages

- `apps/docs`: a sample documentation [Next.js]() app
- `apps/web`: a sample web [Next.js]() app
- `packages/ui`: a stub React component library shared by both `web` and `docs` applications
- `packages/config`: shared `tailwindcss`, `eslint` configurations (includes `eslint-config-next`, `eslint-config-prettier`, `eslint-plugin-prettier` etc..)
- `packages/tsconfig`: `tsconfig.json`s which can be used by extending them throughout the monorepo
