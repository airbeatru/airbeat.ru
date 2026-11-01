# AirBeat FM-1 Stage 11 experimental CI

This directory contains experimental AirBeat FM-1 DSP and Skiff patchers for build/review, NOT hardware installation.

- overlay.tar.xz.b64 is base64 of a checked XZ TAR with 31 source/patcher files from Stage 11.
- SHA256 of decoded archive: 1d3e81b3cdfe953dc5c3565421250eef4fabc05559bcc56bc60f56f9217b8395.
- SHA256 of firmware/eng_airbeat.c inside archive: 64c5ab43537e601642bab69c51896d99c83f6f51520ae1220fa4323bfd78238e.
- Pinned Skiff upstream commit: 8eb0e273b62d964dc7f53ca78257c19fdc38bd9e from https://github.com/illuminus5/skiff .
- GPL-3.0-only. Skiff original attribution remains in patched source.
- Main branch and website airbeat.ru remain untouched. No hardware flashing or automatic binary release.

Workflow airbeat-fm1-integrated.yml validates the archive, applies Stage 6, 7, 8 patches to exact Skiff sources, attempts a JieLi hardware build and host integrated tests. Even a successful build requires CPU/RAM and hardware recovery review before device installation.
