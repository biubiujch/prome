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
  "strategy_id": "crypto_trend_4h",
  "experiment_id": "exp_001",
  "generated_at": "2026-05-12T10:00:00Z",
  "market": "crypto",
  "freq": "4h",
  "signals": [
    {
      "instrument": "BTCUSDT",
      "timestamp": "2026-05-12T08:00:00Z",
      "score": 0.73,
      "rank": 1,
      "side": "long",
      "confidence": 0.68,
      "target_weight": 0.25
    }
  ]
}
```

Prome does not place live trades. Use the exported signals with your own execution stack.
