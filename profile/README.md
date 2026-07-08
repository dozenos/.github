# DozenOS

**DozenOS is a downstream rebuild of [VyOS](https://vyos.io) — an open-source, Debian-based network operating system.**

Every repository in this organization is an **automated 1:1 mirror** of the
corresponding [`vyos/*`](https://github.com/vyos) repository, produced by a
mechanical rename/rebrand transform and re-synced from upstream on a schedule.
DozenOS builds the same router/firewall platform VyOS does — the difference is
branding and build/distribution infrastructure, not features.

## Relationship to VyOS

- **All source code originates from VyOS** and remains under the **GNU GPL**
  (see each repository's `LICENSE`/`debian/copyright`). DozenOS adds no
  proprietary code; it re-brands and re-builds existing free software.
- Repositories here map one-to-one onto their upstream counterparts, e.g.
  `dozenos/dozenos-build` ← `vyos/vyos-build`,
  `dozenos/dozenos-1x` ← `vyos/vyos-1x`,
  `dozenos/hvinfo` ← `vyos/hvinfo`, and so on.
- The transform renames the four case-forms of *VyOS* → *DozenOS* while
  deliberately **keeping** the historical `vyatta` names (they are part of
  the upstream package/command interface, not branding).

We are grateful to the VyOS maintainers and community for the software this
project is built on.

## A note on upstream references

A few `vyos`-owned URLs are **kept on purpose**, because DozenOS reuses that
upstream infrastructure rather than re-hosting it — for example the SBOM tool
download from `cdn.vyos.io` and kernel source tarballs from
`packages.vyos.net/source-mirror`. These are the only intentional `vyos`
references left in the trees, and they exist so the build keeps working.

## Building

Build tooling lives in [`dozenos-build`](https://github.com/dozenos/dozenos-build).
The nightly ISO is built and published (minisign-signed) from a dedicated
build-and-release repository. See each repository's own README for details.

---

*DozenOS is an independent project and is not affiliated with or endorsed by
VyOS or Sentrium S.L. "VyOS" is a trademark of its respective owner; it is used
here only to describe the upstream origin of this software.*
