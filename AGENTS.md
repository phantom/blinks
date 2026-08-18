# Repository instructions

## Purpose
This TypeScript package provides Phantom Blink action APIs, React UI components, and a Chrome extension entrypoint for rendering actions on X.

## Layout
- `src/api/` defines action configuration, callbacks, registry behavior, and protocol types.
- `src/ui/` contains the React action components.
- `src/ext/twitter.tsx` is the X/Twitter extension entrypoint.
- `src/shared/` and `src/utils/` contain shared security and URL helpers.
- `test/` contains API and utility specifications.

## Commands
- Install dependencies: `yarn install`
- Build the package: `yarn build`
- Build before packaging: `yarn prepack`

## Constraints
The package publishes CommonJS, ESM, type declarations, and CSS from `dist/`; keep the exports in `package.json` aligned with the build output configured in `tsup.config.ts`.
