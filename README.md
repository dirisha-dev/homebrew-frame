# homebrew-frame

Public Homebrew tap for **[frame](https://github.com/dirisha-dev/frame)** — a locally-bound
REST API for launching, snapshotting, and archiving AI agent sandboxes.

The frame source repo is private; this tap hosts the **prebuilt binaries** and the
Homebrew **cask**. Both are published automatically by
[GoReleaser](https://goreleaser.com) on each tagged frame release.

## Install

```sh
brew install dirisha-dev/frame/frame   # installs frame + Lima
frame bootstrap                        # create the Linux VM (containerd + gVisor) and start the API
frame doctor                           # verify readiness
```

`frame` runs agent sandboxes inside a Linux VM and forwards its REST API to
`http://127.0.0.1:7070` on the host.
