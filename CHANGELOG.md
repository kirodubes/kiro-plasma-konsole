# Changelog

## 2026.06.20 (payload)

### What Changed
- Captured the real Konsole config from a configured Plasma box into the repo:
  - `Kiro.profile` — default profile (ArcDark colours, Hack Nerd Font 12, 140×40,
    margin 5, unlimited scrollback, scrollbar right).
  - `ArcDark.colorscheme` — the matching colour scheme.
  - `konsolerc` — menubar disabled, `DefaultProfile=Kiro.profile`.
- All three ship via `/etc/skel` so a new user gets the Kiro profile as the default.

### Files Modified
- etc/skel/.local/share/konsole/Kiro.profile (new)
- etc/skel/.local/share/konsole/ArcDark.colorscheme (new)
- etc/skel/.config/konsolerc (new)
- etc/skel/.local/share/konsole/.gitkeep (removed — real payload now present)

## 2026.06.20

### What Changed
- Initial repo created in the Kiro ecosystem: default Konsole configuration for the
  Plasma edition.
- Standard markdown scaffold added (`README.md`, `CHANGELOG.md`, `CLAUDE.md`) per the
  ecosystem MD-scaffold rule.
- Canonical bash scaffold copied in (`up.sh`, `setup.sh`) plus `LICENSE`, `kiro.jpg`,
  `.gitignore`.
- Empty payload directory `etc/skel/.local/share/konsole/` created as a placeholder
  for the Konsole `*.profile` / `*.colorscheme` files still to be added.
- Git initialised with the kirodubes SSH remote; repo created on GitHub.

### Technical Details
- Modelled on the sibling `kiro-plasma-system-settings` / `kiro-plasma-keybindings`
  repos. `setup.sh` auto-detects the `~/KIRO/` path and sets the Kiro Dubes identity
  and the kirodubes remote.

### Files Modified
- README.md, CHANGELOG.md, CLAUDE.md (created)
- up.sh, setup.sh, LICENSE, kiro.jpg, .gitignore (copied)
- etc/skel/.local/share/konsole/.gitkeep (created)
