Ready patches for openchamber/openchamber issues #7449 and #7450.

- `forgejo-pr-watch.patch` — PR watch for Gitea/Forgejo `/pulls/N` addresses (issue #7449).
- `ci-wait.patch` — built-in `ci` wait source for commit and branch checks without a PR (issue #7450).

Both were generated against `3a0dbea` (v2.8.0). Validation: `bun run type-check`, `bun run lint`, `bun run build` pass; the two affected server test files pass 65/65. Live run on web against a self-hosted Forgejo woke the session with real check results.
