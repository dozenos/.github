# DozenOS

**DozenOS is an open-source, Debian-based network operating system for
routing and firewalling.**

It is an automated downstream rebuild of the [VyOS](https://vyos.io) rolling
release: every repository in this organization is a mechanical, regularly
re-synced mirror of its upstream counterpart, with branding and
build/distribution infrastructure as the only changes — no features are added
or removed. All source code remains under the **GNU GPL** (see each
repository's `LICENSE`/`debian/copyright`), and we are grateful to the
upstream maintainers and community for the software this project is built on.

## Downloads

Nightly ISO and virtual machine images can be downloaded from the
**[DozenOS nightly builds page](https://dozenos.github.io/dozenos-nightly-build/)**
(the same artifacts are attached to the
[GitHub Releases](https://github.com/dozenos/dozenos-nightly-build/releases) of
`dozenos-nightly-build`). Every artifact is minisign-signed; verification
instructions are on the page.

The default login is **`dozenos` / `dozenos`**. Change the password after
first boot.

## Building

Build tooling lives in [`dozenos-build`](https://github.com/dozenos/dozenos-build).
The nightly images are built and published (minisign-signed) from
[`dozenos-nightly-build`](https://github.com/dozenos/dozenos-nightly-build).
See each repository's own README for details.

---

*DozenOS is an independent project and is not affiliated with or endorsed by
the upstream project or its owners. "VyOS" is a trademark of its respective
owner; it is used here only to describe the upstream origin of this software.*
