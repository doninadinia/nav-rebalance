# nav-rebalance

> nav · rebalance · paper

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

Portfolio NAV rebalance — one symbol, equity print.

## Features

- Default venue binance / PORTFOLIO
- Built-in rebalance strategy plus paper mode
- Risk manager with daily-loss kill switch
- OHLCV store and SHA-256 stub candles
- Backtester with fill + fee model
- Click CLI: backtest, paper, status, orders

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd nav-rebalance
python -m pip install -e .
python -m navreb --help
```

## CLI Usage

```bash
navreb backtest --bars 200
# Replay stub candles

navreb paper
# Start a paper session

navreb status
# Print engine state

navreb orders
# List simulated fills
```

## Project Structure

```
navreb/
  core/        engine + risk
  strategy/    grid / dca / ema hooks
  exchange/    stub order client
  data/        candles + backtest
  cli.py
tests/
```

## Configuration

See `navreb/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `exchange` | `binance` | Venue id |
| `symbol` | `PORTFOLIO` | Default pair |
| `strategy` | `rebalance` | Active strategy |
| `mode` | `paper` | paper or backtest |

## Tests

```bash
python -m pytest -q
```

## Background

Desk scripts search nav-rebalance, not a branded tracker.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![nav](https://img.shields.io/badge/nav-111827?style=flat-square) ![rebalance](https://img.shields.io/badge/rebalance-111827?style=flat-square) ![nav-rebalance](https://img.shields.io/badge/nav%20rebalance-111827?style=flat-square) ![trading-bot](https://img.shields.io/badge/trading%20bot-111827?style=flat-square) ![crypto-trading](https://img.shields.io/badge/crypto%20trading-111827?style=flat-square) ![binance](https://img.shields.io/badge/binance-111827?style=flat-square) ![defi](https://img.shields.io/badge/defi-111827?style=flat-square) ![algorithmic-trading](https://img.shields.io/badge/algorithmic%20trading-111827?style=flat-square)

`nav` `rebalance` `nav-rebalance` `trading-bot` `crypto-trading` `binance` `defi` `algorithmic-trading` `quantitative-finance` `open-source` `python`

Search: nav-rebalance · nav · rebalance · paper · Portfolio NAV rebalance — one symbol, equity print.

---

<sub>Portfolio NAV rebalance — one symbol, equity print.</sub>
