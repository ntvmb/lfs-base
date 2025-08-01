# lfs-base
Base files for an LFS system with sl-pkg. There's no source code here so don't expect much.

Current version: 12.3

# Errata for the current version
- In the base tarball, Python was not built with support for bzip2. Some packages will fail to build until Python is recompiled with bzip2 as a result of this.
  - To fix this issue, chroot to the target and issue this command:
```
# sl-pkg install --force-install bzip2 python
```
