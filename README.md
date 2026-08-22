# Stocket Remote Desktop (frozen post-v1 consumer)

> **Status:** frozen and unsupported for hosted inventory v1. The canonical hosted product is the private [`stocketfr/stocket`](https://github.com/stocketfr/stocket) monorepo. Desktop architecture and release work are explicitly post-v1 and remain tracked in this repository's open `post-v1` issues.

This repository preserves the last Tauri remote-desktop prototype as a standalone, reproducible workspace. It is not part of the hosted-v1 release, is not deployed, and must not be presented as a shipped capability.

## Verification

Use the pinned package manager from `package.json`:

```sh
corepack pnpm install --frozen-lockfile
corepack pnpm lint
corepack pnpm test
```

The workspace no longer checks out or links the legacy shared-packages repository. `pnpm-lock.yaml` is the immutable dependency record for this frozen revision.

## Releases

Automated desktop releases are disabled. The previous workflow assembled a desktop application from the legacy `stocketfr/frontend` polyrepo and could not represent the canonical hosted-v1 architecture. Do not tag or publish a desktop release until the post-v1 architecture, signing, update, and rollback contracts in issues #3–#5 are resolved through a new reviewed workflow.

## Licensing

This repository is proprietary and all rights reserved to Maximilian
(`maximilianpw`). Repository visibility does not grant permission to use,
modify, redistribute, or host its source or assets. See [LICENSE](LICENSE) and
[NOTICE](NOTICE). Unsolicited external code, documentation, design, and asset
contributions are not accepted without a written contribution agreement.
