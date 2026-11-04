# tsblock Binaries

> _прищемили хвост_

## Original Project Attribution

This project includes components from:

- **tsblock**
  - [`tsblock`](https://github.com/ciffelia/tsblock) is a project by [ciffelia](https://github.com/ciffelia) and [Contributors](https://github.com/ciffelia/tsblock/graphs/contributors)
  - Available on [GitHub](https://github.com/ciffelia/tsblock.git)
  - Licensed under the [GNU General Public License v3.0](https://github.com/ciffelia/tsblock/blob/main/LICENSE)

## Changes Made

- Block interfaces matching `^cmld` in addition
- Exit non-zero when the netlink link subscription closes
- Attach only through cgroup `bpf_link` (Linux 5.7+)
- Replace `cockroachdb/errors` with the standard library
- Add `tsblock-btf` (matches `cilium_*`, `lxc*` and `cmld*` against `skb->dev->name` inside the BPF program, but needs Linux 6.2+ with BTF and the BPF JIT)
- Bump Go to 1.27.3 and every module dependency
- Regenerate the eBPF objects with `bpf2go`
