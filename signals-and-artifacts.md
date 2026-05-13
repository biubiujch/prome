# Signals And Artifacts

Prome experiments produce a strategy artifact bundle. This bundle lets you reproduce the experiment and consume the generated signals outside Prome.

## Artifact Bundle

```text
artifacts/experiments/{experiment_id}/
  strategy.json
  dataset.json
  model.pkl
  model_meta.json
  predictions.parquet
  signals.parquet
  latest_signal.json
  backtest.json
  report.html
  run.log
```

## Latest Signal Format

```json
{
  "schema_version": 1,
  "strategy_name": "crypto_trend_4h",
  "dataset_id": "crypto_4h",
  "market": "crypto",
  "generated_at": "2026-05-12T10:00:00Z",
  "signal_time": "2026-05-12 08:00:00",
  "horizon": 1,
  "artifact_uri": "artifacts/experiments/task_001",
  "signals": [
    {
      "instrument": "BTCUSDT",
      "action": "buy",
      "score": 0.73,
      "weight": 0.25,
      "rank": 1,
      "metadata": {}
    }
  ]
}
```

Prome does not place live trades. Use the exported signals with your own execution stack.
