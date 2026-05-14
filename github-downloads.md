# GitHub Downloads

Prome release downloads are distributed through GitHub Releases.

## Download Page

```text
https://github.com/biubiujch/prome/releases/latest
```

The public GitHub repository contains user documentation and release assets only.

## Source Code

The product source code and internal development documentation are not published in the public documentation repository.

GitHub automatically provides source archives for every public repository release. For Prome, those archives contain only the public documentation repository contents.

## Release Assets

Use the attached release assets for installation:

```text
prome-{version}-macos-arm64.tar.gz
prome-{version}-macos-x64.tar.gz
prome-{version}-linux-x64.tar.gz
prome-{version}-windows-x64.zip
checksums.txt
```

Each platform bundle contains:

- install scripts for the local CLI, API, and Web entrypoints
- Python workspace wheels plus a pinned `requirements.txt`
- a Next.js standalone Web bundle
- public installation and quickstart docs
