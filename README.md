# Eliza Workspace Turborepo

This is a monorepo for the Eliza project. It is built with Turborepo and pnpm.

## Packages

- `eliza-core/`: The current Eliza monorepo.
- `eliza-stable/`: The stable version of Eliza.
- `eliza-custom/`: A custom version of Eliza meant for development purposes. (change the name of this to eliza-dev)
- `examples/`: A collection of example SDK implementations to integrate with Eliza.

## TODO

- [ ] Ensure we properly handle the imported packages (eliza-core and eliza-stable) for pulling current versions while keeping any necessary dependencies for building our turborepo. (we added type-doc and tsup to the `packages/eliza-stable/` root `package.json` file, and added a `tsup.config.ts` file to the `package.json` file in `packages/eliza-stable/core/`)
- [ ] Clean up/fix the `docs/src/dev/lifi/` docs.
- [ ] Update our `.cursorrules` file to make it specific for this Turborepo.
- [ ] Resolve the pnpm.overrides warning and other packages/eliza-core warnings.
- [ ] Configure turborepo remote caching.
- [ ] Script for running only a custom eliza project.
