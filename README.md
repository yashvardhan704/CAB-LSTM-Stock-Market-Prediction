# CAB-LSTM: Context-Aware Attention-Based LSTM for Stock Market Prediction

## Overview

CAB-LSTM is a hybrid deep learning framework designed for stock market direction prediction using:

- Technical Indicators
- Financial News Sentiment
- Source-Weighted Attention Mechanism
- Sequential Deep Learning (LSTM)

The model combines quantitative financial indicators with qualitative investor sentiment extracted from financial news headlines.

---

## Key Features

- Attention-based LSTM architecture
- Source credibility weighted sentiment analysis
- - Multi-modal feature engineering
- Technical indicators:
  - RSI
  - MACD
  - Bollinger Bands
  - ATR
  - OBV
- Comparative benchmarking:
  - Logistic Regression
  - XGBoost
  - Standard LSTM
  - Proposed CAB-LSTM

---

## Research Objective

Traditional stock prediction models rely mainly on historical prices and ignore investor sentiment.

This project introduces a Context-Aware Attention-Based LSTM (CAB-LSTM) that integrates:

1. Technical market indicators
2. Financial news sentiment
3. Source credibility weighting
4.  Temporal attention mechanism

to improve directional stock market forecasting.

---

## Model Architecture

Input Features
    ↓
Technical Indicators + Weighted Sentiment
    ↓
Sequence Generation
    ↓
Stacked LSTM Layers
    ↓
Attention Mechanism
    ↓
Dense Layer
    ↓
Binary Prediction (Up/Down)

---

## Dataset

### Primary Dataset
S&P 500 with Financial News Headlines (2008–2024)
### Additional Publisher Dataset
- Reuters
- CNBC
- The Guardian

---

## Technical Indicators Used

| Indicator | Purpose |
|---|---|
| RSI | Momentum detection |
| MACD | Trend analysis |
| Bollinger Bands | Volatility estimation |
| ATR | Market volatility |
| OBV | Volume-price relationship |

---

## Sentiment Pipeline

1. News headline preprocessing
2. VADER sentiment analysis
3. Source authority weighting
4. Daily sentiment aggregation

   ### Source Weight Dictionary

| Source | Weight |
|---|---|
| Reuters | 1.5 |
| CNBC | 1.2 |
| Guardian | 1.1 |
| Other | 1.0 |

---

## Experimental Results

| Model | Accuracy |
|---|---|
| Logistic Regression | 48.52% |
| XGBoost | 60.46% |
| Standard LSTM | 78.57% |
| CAB-LSTM | 86.03% |

---

## Installation

```bash
git clone https://github.com/yourusername/CAB-LSTM-Stock-Market-Prediction.git
cd CAB-LSTM-Stock-Market-Prediction
pip install -r requirements.txt

