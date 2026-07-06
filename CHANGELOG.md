# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Added `.nvmrc` configuration file baseline to specify Node.js version `24.6.0` requirement.
- Added `engines` requirements to `package.json` to enforce compatibility with Node.js `>=24.6.0`.
- Documented project architecture decision regarding committed frontend build assets (Option A) in `docs/decisions/0001-committed-frontend-assets.md`.
- Created comprehensive GRS-compliant `README.md` containing Title, Project Status, Overview, Features, Quick Start, Environment Configuration parameters, Project Structure directory mapping, server architecture Mermaid diagram, and Development instructions.

### Changed
- Aligned project package version from stable `1.0.0` to experimental `0.1.0` in `package.json` and `package-lock.json` to correctly reflect repository lifecycle classification.
