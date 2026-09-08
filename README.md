# Quantitative Trading Engine & Institutional Skills Architecture

This repository hosts the production quantitative trading engine, walk-forward testing harnesses, and institutional skills catalog across 18 Binance USDT-M perpetual contracts.

## Repository Layout
- `Engine/`: Core strategy modules, real-time liquidation cascades, market-making pipelines, execution ratchets, and out-of-sample walk-forward evaluation harnesses.
- `skills/`: Comprehensive, unpacked institutional quant and engineering skills catalog containing 1303 specialized `.md` reference guides.

## Core Engine Modules (`Engine/`)
- `Engine/strategy/`:
  - `rp2_round7_residual_dislocation.py`: Round 7 Cross-Sectional Residual Dislocation Engine (v7.0) with causal daily Wilder ATR and multi-tier ratchet.
  - `funding_basis_carry_engine.py`: Spot-perp basis and 8h funding rate carry engine.
  - `s1_liquidation_cascade.py` & `s1_liquidation_cascade_v2.py`: Real-time liquidation cascade engine.
  - `institutional_alpha_master.py` & `s2_institutional_ml.py`: Institutional ML overlay classification suite.
  - `smc_*.py`: Smart Money Concepts reference playbooks (Mayne, Marco, Kane, Edgeful, Usman Noah, Marci).
- `Engine/core/`: Machine learning models, feature engineering pipelines, and execution invariants.
- `Engine/pipeline/`: Ingestion, normalization, and feature generation pipelines for Binance perpetuals.
- `Engine/verification/`: Causal audit tools, 20 OOS window scorecards, and friction accounting checks.

## Institutional Skills (`skills/`)
The `skills/` directory contains 1303 standalone `.md` skill specifications covering:
- Quant Research & Mathematical Modeling (`quant-analyst.md`, `agent-data-ml-model.md`, `backtesting-trading-strategies.md`, etc.)
- Engineering & Clean Code (`karpathy-guidelines.md`, `clean-code.md`, `systematic-debugging.md`, etc.)
- Machine Learning & MLOps (`training-machine-learning-models.md`, `evaluating-machine-learning-models.md`, etc.)
- Architecture & Optimization (`codebase-design.md`, `performance-optimization.md`, etc.)
