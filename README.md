# tsblock Binaries

> _прищемили хвост_

## Original Project Attribution

This project includes components from:

- **tsblock**
  - [`tsblock`](https://github.com/ciffelia/tsblock) is a project by [ciffelia](https://github.com/ciffelia) and [Contributors](https://github.com/ciffelia/tsblock/graphs/contributors)
  - Available on [GitHub](https://github.com/ciffelia/tsblock.git)
  - Licensed under the [GNU General Public License v3.0](https://github.com/ciffelia/tsblock/blob/main/LICENSE)

## Changes Made

- Bump the Go toolchain and module dependencies (Go 1.21 → 1.27.1, `cilium/ebpf` 0.11 → 0.22, transitive deps)
- Regenerate the eBPF bindings and objects (`bpf2go`) against the updated `cilium/ebpf`
- Block interfaces matching `^cmld` in addition
- Log netlink subscription errors instead of panicking on them
