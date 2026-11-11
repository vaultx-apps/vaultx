# Contributing to VaultX

Thank you for your interest in VaultX.

## Development Workflow

1. Create a feature branch from main.
2. Make your changes.
3. Test your changes locally.
4. Commit with a descriptive message.
5. Open a pull request for review.

## Branch Structure

- main: Stable production code
- feature/*: New features
- fix/*: Bug fixes

## Commit Convention

- feat: New features
- fix: Bug fixes
- docs: Documentation changes
- style: UI and styling changes
- refactor: Code improvements
- chore: Maintenance tasks

## Notes for this repository

- The site is a single self-contained `index.html` — no build step, no package
  manager. Keep it that way: do not introduce a build system or split the page
  into framework files without discussion in an issue first.
- Test locally by opening `index.html` in a browser or serving it with
  `python3 -m http.server 8000`. Live data comes from Robinhood Chain RPC
  endpoints, so network access is required for prices and wallet features.
- Contract addresses in the README and the site must match the on-chain
  contracts. Verify any address on Blockscout before committing it.
- $VAULTX is not launched. Do not add a contract address, price, or purchase
  link for it until the launch is announced.
