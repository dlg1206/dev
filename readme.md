# Dev Docker Images

> Collection of docker images for quick dev environments. Each environment comes preconfigured with
> specialized [dotfiles](https://github.com/dlg1206/dotfiles).

Tag images for easy use:

```bash
docker pull ghcr.io/dlg1206/<image>
docker tag ghcr.io/dlg1206/<image> <image> 
docker run --rm -it <image>
```

## Alpine

### base

Minimal `alpine` image with common utils

**Base Image**: `alpine:3.22`

```bash
docker pull ghcr.io/dlg1206/alpine
```

#### Added Utils

- `curl`
- `git`
- `jq`
- `vim`

## Debian

### base

Minimal `debian 12` image with common utils

**Base Image**: `debian:bookworm-slim`

```bash
docker pull ghcr.io/dlg1206/debian
```

#### Added Utils

- `curl`
- `git`
- `jq`
- `ping`
- `vim` 