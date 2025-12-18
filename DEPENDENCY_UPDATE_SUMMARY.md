# Dependency Update Summary

Date: 2025-12-18

Project layer: prplos-3449 (customization/meta layer)

Actions performed:
- Synchronized and updated all git submodules recursively:
  - git submodule sync
  - git submodule update --init --recursive

Rationale:
- Ensure external sources referenced by the meta-layer are aligned with their configured remotes before building against the core prplos tree.

Notes:
- If this repository pins specific submodule SHAs for reproducibility, verify the desired SHAs after the update.
- No build lockfiles are used in this layer; submodule SHAs act as the source of truth.

Related updates:
- Core prplos feeds were updated and installed in the adjacent prplos repository during this maintenance window.
