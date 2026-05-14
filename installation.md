# Installation

Prome is designed to run locally.

## Runtime Prerequisites

- Python 3.12 or newer
- Node.js 24 or newer

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

## Extract And Install

```bash
tar -xzf prome-{version}-linux-x64.tar.gz
cd prome-{version}
./install.sh
```

On Windows, extract `prome-{version}-windows-x64.zip` and run `install.bat`.

## Startup Paths

CLI:

```bash
./bin/prome doctor
```

API:

```bash
./bin/prome-api
```

Web:

```bash
PROME_API_BASE_URL=http://127.0.0.1:8000 ./bin/prome-web
```

The doctor command checks local paths, data availability, writable artifact directories, and runtime dependencies. The Web bundle expects the local API to be reachable through `PROME_API_BASE_URL`.

## Data

Prome can use local datasets. The MVP starts with crypto data and supports importing or registering compatible local data.
