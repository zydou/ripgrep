# ripgrep

This repository uses GitHub Actions to build the `rg` (ripgrep) tool. The [official repository](https://github.com/BurntSushi/ripgrep) includes binary releases for the following architectures:

- arm-unknown-linux-gnueabihf
- x86_64-unknown-linux-musl
- x86_64-apple-darwin
- x86_64-pc-windows-gnu
- x86_64-pc-windows-msvc
- i686-pc-windows-msvc

However, it lacks support for other architectures such as `aarch64-apple-darwin`. This repository aims to build these missing architectures. Specifically, it builds the following architectures:

- x86_64-unknown-linux-gnu
- aarch64-unknown-linux-gnu
- aarch64-apple-darwin

In addition, it also directly downloads the `dua` binary from the official source and uploads it to GitHub Release of the following architectures for convenience:

- x86_64-unknown-linux-musl
- x86_64-apple-darwin
- arm-unknown-linux-gnueabihf
