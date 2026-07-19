# cc-common

Source of truth for shared agent-team skill docs used by the `cc-cmds` and `wishket-cmds` Claude Code plugins.

## Files

- `agent-team-protocol.md`
- `askuserquestion.md`
- `team-cleanup.md`

## How this repo is used

- Edit the shared docs **here only** — this repo is the single upstream source of truth.
- Changes propagate **one-way and automatically**: a sync step copies byte-identical vendored copies into each consumer.
- Consumers:
  - https://github.com/Nharu/cc-cmds
  - https://github.com/Nharu/wishket-cmds
- The vendored copies inside the consumer repos are **not** edit points — any edit there is overwritten on the next sync. Change the upstream doc in this repo instead.

## License

MIT — see `LICENSE`.
