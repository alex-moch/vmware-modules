# vmware-modules

Kernel module source for VMware Workstation's `vmmon` and `vmnet`.

## Source

Extracted from `VMware-Workstation-Full-25H2u1-25219725.x86_64.bundle`.

```
sha256: 721aa93c4ebcaa51ac6db75ed97c7a4db10aa88110446890db1e40bfafc7566a
```

## Tested

Built with Clang 22.1.2 and tested against:

- Linux 6.19.10
- Linux 7.0.0-rc5

## Building

```sh
cd vmmon-only && make CC=clang LD=ld.lld && cd ..
cd vmnet-only && make CC=clang LD=ld.lld && cd ..
```

When built via Gentoo's `linux-mod-r1` eclass, the correct compiler is picked up automatically from the kernel configuration.

## Mirrors

This repository is mirrored on Codeberg, GitLab, GitHub and SourceHut:

- https://codeberg.org/alexm/vmware-modules
- https://gitlab.com/alex-moch/vmware-modules
- https://github.com/alex-moch/vmware-modules
- https://git.sr.ht/~alexm/vmware-modules

## License

GPL-2.0
