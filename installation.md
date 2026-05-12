# Installation

Prome is designed to run locally.

## Download A Release

Go to the latest release page:

```text
https://github.com/biubiujch/prome/releases/latest
```

Download the archive for your operating system:

- macOS Apple Silicon: `prome-{version}-macos-arm64.tar.gz`
- macOS Intel: `prome-{version}-macos-x64.tar.gz`
- Linux x64: `prome-{version}-linux-x64.tar.gz`
- Windows x64: `prome-{version}-windows-x64.zip`

## Verify The Download

Download `checksums.txt` from the same release and verify the package checksum.

## First Run

```bash
prome doctor
```

The doctor command checks local paths, data availability, writable artifact directories, and runtime dependencies.

## Data

Prome can use local datasets. The MVP starts with crypto data and supports importing or registering compatible local data.
