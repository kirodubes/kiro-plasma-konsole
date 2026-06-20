<p align="center">
  <img src="kiro.jpg" alt="Kiro" width="220" />
</p>

# kiro-plasma-konsole

Default **Konsole** configuration for Kiro — the terminal profile, colour scheme,
and behaviour applied out of the box on the Plasma edition (font, transparency,
scrollback, default profile). Sibling to
[kiro-plasma-system-settings](https://github.com/kirodubes/kiro-plasma-system-settings),
[kiro-plasma-keybindings](https://github.com/kirodubes/kiro-plasma-keybindings) and
[kiro-plasma-servicemenus](https://github.com/kirodubes/kiro-plasma-servicemenus).

## What's in this repo

- `etc/skel/.local/share/konsole/` — the Kiro Konsole `*.profile` and
  `*.colorscheme` files, seeded into a new user's home via `/etc/skel/`.
  Currently a scaffold — drop the shipped profile/colorscheme files in here.
- `setup.sh`, `up.sh` — standard Kiro bash scaffold (git identity + sync).

## Installation

### From `nemesis_repo` (recommended)

```ini
[nemesis_repo]
SigLevel = Never
Server = https://erikdubois.github.io/$repo/$arch
```

```bash
sudo pacman -Syu
sudo pacman -S kiro-plasma-konsole
```

### Manual

```bash
git clone https://github.com/kirodubes/kiro-plasma-konsole.git
cd kiro-plasma-konsole
sudo cp -rT etc/skel /etc/skel
```

Existing users can copy the profile straight into their own home:

```bash
cp -rT /etc/skel ~/
```

Then set the Kiro profile as default in **Konsole → Settings → Manage Profiles**
(or it applies automatically to new accounts).

## Websites

Information : https://kiroproject.be

## Social Media

Youtube : https://www.youtube.com/erikdubois

<!-- KIRO-FUNDING-FOOTER:START — managed by Kiro-HQ/cascade-readme-footer.sh -->
## Help fund Kiro

Everything I build here stays free and open — always. If Kiro or any of these
tools have ever saved you time or taught you something, a small monthly
contribution helps keep the work going. Donations target break-even, nothing
more — the core always stays free for everyone.

- GitHub Sponsors: https://github.com/sponsors/erikdubois
- Patreon: https://www.patreon.com/c/kiroproject
- YouTube memberships: https://www.youtube.com/@ErikDubois/join
- Ko-fi: https://ko-fi.com/erikdubois
- PayPal: https://www.paypal.me/erikdubois
<!-- KIRO-FUNDING-FOOTER:END -->

## License

See [LICENSE](./LICENSE).
