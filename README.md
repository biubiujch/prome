# Prome

Prome is a local-first quantitative strategy platform for composing, training, backtesting, and exporting strategy signals.

The application runs on your own machine. Your data, models, experiments, and signal artifacts stay local unless you explicitly move them elsewhere.

## What You Can Do

- Register or import market data.
- Compose strategies manually.
- Train and backtest models locally.
- Export standardized signals for your own systems.
- Use Web UI, CLI, and local API workflows.

## MVP Scope

The first release focuses on local research and signal export:

- Crypto data first.
- Manual strategy composition.
- LightGBM + Qlib research pipeline.
- Local experiment tracking.
- Standard strategy artifact bundle.
- CLI and local API access to latest signals.

Live trading is not included. Prome exports signals so you can connect them to your own execution stack.

## Download

Download the latest release from the GitHub Releases page:

```text
https://github.com/biubiujch/prome/releases/latest
```

Choose the package for your operating system, then follow the Quickstart.

## Quickstart

```bash
prome doctor
prome datasets list
prome strategies examples
prome strategies run examples/crypto_trend_4h.json
prome experiments list
prome signals latest --experiment <experiment_id> --format json
```

## Documentation

- [Installation](./installation.md)
- [Quickstart](./quickstart.md)
- [Signals And Artifacts](./signals-and-artifacts.md)
- [GitHub Downloads](./github-downloads.md)
