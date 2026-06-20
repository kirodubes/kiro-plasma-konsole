# Changelog

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
