# Quickstart

## 1. Install The Bundle

```bash
./install.sh
```

## 2. Check Your Local Setup

```bash
./bin/prome doctor
```

## 3. List Available Datasets

```bash
./bin/prome datasets list
```

## 4. Start The Local API And Web Workbench

```bash
./bin/prome-api
PROME_API_BASE_URL=http://127.0.0.1:8000 ./bin/prome-web
```

## 5. Run A Strategy From JSON

```bash
./bin/prome strategies run ./strategy.json --json
```

## 6. Review Experiments And Latest Signals

```bash
./bin/prome experiments list
./bin/prome signals latest --json
./bin/prome export experiment <experiment_id> --target ./signals
```

The exported signal files can be consumed by your own trading, alerting, or analytics system.
