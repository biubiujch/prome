# Quickstart

## 1. Check Your Local Setup

```bash
prome doctor
```

## 2. List Available Datasets

```bash
prome datasets list
```

## 3. Run An Example Strategy

```bash
prome strategies examples
prome strategies run examples/crypto_trend_4h.json
```

## 4. Review Experiments

```bash
prome experiments list
prome experiments show <experiment_id>
```

## 5. Export Latest Signals

```bash
prome signals latest --experiment <experiment_id> --format json
prome export --experiment <experiment_id> --target ./signals
```

The exported signal files can be consumed by your own trading, alerting, or analytics system.
