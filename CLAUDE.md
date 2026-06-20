# CLAUDE.md — kiro-plasma-konsole

## Project overview

See [README.md](./README.md). Ships the default **Konsole** profile, colour
scheme, and `konsolerc` for Kiro's Plasma edition.

## Current state

Created 2026-06-20. Standard Kiro bash scaffold (`up.sh`, `setup.sh`) plus the
three required markdown files. Payload dir `etc/skel/.local/share/konsole/` is an
empty placeholder — the actual `*.profile` / `*.colorscheme` files are still to be
captured from a configured box (see [[plasma-test-box]] / the snapshot workflow).

## Patterns & decisions

- Bash scripts follow the canonical Kiro template — see
  [up.sh](/home/erik/Insync/Kiro/Kiro-HQ/up.sh) / [setup.sh](/home/erik/Insync/Kiro/Kiro-HQ/setup.sh).
- `setup.sh` is path-aware: under `~/KIRO/` it sets the Kiro Dubes identity and the
  kirodubes remote automatically.
- Konsole profiles/colorschemes are **per-user** data (`~/.local/share/konsole/`),
  so they ship via `/etc/skel/` (new accounts). `konsolerc` (the app-level default
  profile pointer) can ship via `/etc/xdg/` if an all-users default is wanted —
  decide when the payload lands.

## Next steps

- Capture the real Konsole `*.profile` + `*.colorscheme` from a configured box and
  drop them into `etc/skel/.local/share/konsole/`.
- Add the build recipe under `~/KIRO-PKG-BUILD-APPS/` once the payload exists.

Open work for the ecosystem lives in
[HQ/MASTER_TODO.md](/home/erik/Insync/Kiro/Kiro-HQ/MASTER_TODO.md) — no per-repo TODO.md.
