# rpm-repo

Self-hosted, GPG-signed DNF/RPM repository for [Glyph](https://github.com/hamidfzm/glyph), served via GitHub Pages at <https://glyph-md.github.io/rpm-repo>.

```bash
sudo tee /etc/yum.repos.d/glyph.repo < <(curl -fsSL https://glyph-md.github.io/rpm-repo/glyph.repo)
sudo dnf install glyph
```

RPMs, `repodata/`, `gpg.key`, and `glyph.repo` are pushed here automatically by the `publish-dnf` job in the Glyph release workflow. Do not edit by hand.
