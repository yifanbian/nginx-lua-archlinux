# nginx-lua-archlinux

This repository contains files required by `makepkg` to build a custom `openresty` package.

Although artifacts made by this repo is called `openresty`, this repo has no relation with the OpenResty official.

Nginx modules in this package: `array-var-nginx-module`, `echo-nginx-module`, `headers-more`, `lua-nginx-module`, `lua-upstream-nginx-module`, `memc-nginx-module`, `ngx_coolkit`, `ngx_devel_kit`, `redis2-nginx-module`, `set-misc-nginx-module`, `srcache-nginx-module`, `stream-lua-nginx-module`.

## Build

Build a package:

```bash
makepkg -s
```

Build a package and install it:

```bash
makepkg -si
```

Build a package and sign it:

```bash
makepkg -s --sign --key <GPG key id>
```

To compress package with `zst` instead of `xz`, edit `/etc/makepkg.conf`:

```
PKGEXT='.pkg.tar.zst'
```

Add this package to a repo:

```bash
repo-add /path/to/repo.db.tar.gz /path/to/*.pkg.tar.zst
```
