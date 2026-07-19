# cc-common

Source of truth for shared agent-team skill docs, synced one-way into downstream Claude Code plugin repos.

## Files

- `agent-team-protocol.md`
- `askuserquestion.md`
- `team-cleanup.md`

## How this repo is used

- Edit the shared docs **here only** — this repo is the single upstream source of truth.
- Changes propagate **one-way and automatically**: a sync step copies byte-identical vendored copies into each downstream repo.
- Those vendored copies are **not** edit points — any edit there is overwritten on the next sync. Change the upstream doc in this repo instead.

## License

MIT — see `LICENSE`.
