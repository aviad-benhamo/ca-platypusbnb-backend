# ADR 0001: Committed Frontend Assets

## Context

PlatypusBNB is a Coding Academy project representing a full-stack booking platform application. The backend serves both API endpoints and the static frontend client assets.

By default, the frontend build artifacts (compiled JavaScript and CSS bundles, assets, etc.) are located in the `public/assets/` directory.

The GitHub Repository Standard (GRS) recommends keeping the repository clean of generated artifacts and binaries by adding them to `.gitignore`. However, this project is classified as Coding Academy / Experimental, and requires a simple, single-service deployment and demo strategy.

## Decision

We have decided to keep the pre-compiled frontend build artifacts committed directly to Git inside the `public/` directory (specifically `public/assets/`).

This decision corresponds to **Option A** in our repository configuration and allows:
1. **Deployment Simplicity:** The backend can serve the complete application immediately after cloning, without requiring a separate build stage in target environments (e.g., Render, Heroku).
2. **Zero-Setup Demos:** Users or instructors checking the repository can run `npm start` or `npm run dev` and get the full working frontend without setting up a separate dev server, repository branch, or builder.

## Consequences

- **Git Repository Size:** The repository will track pre-built frontend JavaScript and CSS bundles, which increases Git repository size.
- **Frontend Update Workflow:** Any modifications to the frontend code must be built locally, and the updated files inside `public/assets/` must be committed to Git.
- **No Build Pipelines:** There is no requirement for CI/CD frontend build steps.
