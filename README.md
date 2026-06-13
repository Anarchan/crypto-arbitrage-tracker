<p align="center">
  <img src="https://anarchain.co/_next/image?url=%2Fpic%2Fcat-logo.png&w=256&q=100" width="120" alt="Crypto Arbitrage Tracker Logo" />
</p>

<h1 align="center">Crypto Arbitrage Tracker</h1>

<p align="center">
  <strong>Crypto Arbitrage Tracking & Market Intelligence System</strong>
</p>

<p align="center">
  CAT is a market intelligence system designed by Anarchain to monitor crypto markets, compare prices across exchanges, calculate spreads, and analyze potential arbitrage opportunities with risk, liquidity, fees, and execution constraints.
</p>

<p align="center">
  <a href="https://anarchain.co/fa/projects/crypto-arbitrage-tracker">Project Page</a> ·
  <a href="https://cryptoarbitragetracker.com">CAT Website</a> ·
  <a href="https://anarchain.co">Anarchain</a> ·
  <a href="mailto:info@anarchain.co">Contact</a>
</p>

---

## Overview

**Crypto Arbitrage Tracker**, also known as **CAT**, is a crypto market analysis and arbitrage tracking system developed by **Anarchain**.

The system monitors cryptocurrency markets, compares prices between centralized and decentralized exchanges, detects price differences, and evaluates whether a raw spread can become a real, executable arbitrage opportunity.

CAT is designed to move beyond simple price difference detection. It considers trading fees, network costs, liquidity, slippage, transfer time, market limitations, and execution risk before presenting opportunities to users.

---

## The Problem

In crypto markets, the same asset may trade at different prices across exchanges and liquidity venues.

However, a raw price difference is not necessarily a real arbitrage opportunity.

A profitable-looking spread may disappear because of:

- Trading fees
- Withdrawal fees
- Network fees
- Low liquidity
- Slippage
- Transfer delay
- Deposit or withdrawal restrictions
- Fast market movement
- Incomplete order execution
- Differences between CEX and DEX settlement models

CAT was designed to help users evaluate opportunities more carefully instead of reacting only to raw spread numbers.

---

## CAT Solution

CAT creates an analytical layer over crypto market data.

The system collects data from multiple market sources, normalizes symbols and trading pairs, calculates price differences, estimates costs, evaluates risk, and ranks opportunities in a fast and filterable dashboard.

Core capabilities:

- Market price collection
- CEX and DEX monitoring
- Symbol and trading pair normalization
- Spread calculation
- Fee estimation
- Liquidity and slippage analysis
- Risk scoring
- Opportunity ranking
- Watchlist and alerts
- Historical snapshot storage
- Backtesting preparation

---

## Target Users

CAT is designed for:

- Crypto traders
- Market analysts
- Data teams
- Arbitrage researchers
- Crypto intelligence products
- FinTech and trading dashboards
- Advanced crypto users

---

## Data Sources

CAT can collect and process data from different market sources.

### Centralized Exchanges

- Binance
- OKX
- KuCoin
- Bybit
- Coinbase

### Decentralized Exchanges

- Uniswap
- PancakeSwap

### Market & Network Data APIs

- Market prices
- Trading volume
- Network fees
- Transfer cost context
- Liquidity and market context

---

## Data Flow Topology

```txt
CEX APIs / DEX APIs / Market APIs / Network Fees
        |
        v
Adapter Layer
Exchange adapters · API wrappers · Symbol mapping · Rate-limit handling
        |
        v
Ingestion & Scheduler
Scheduled fetch · Real-time stream · Ticker collection · Timestamp alignment
        |
        v
Normalization Layer
Normalize symbols · Align trading pairs · Quote currency unification · Clean outliers
        |
        v
Arbitrage Engine
Spread calculation · Fee estimation · Liquidity check · Slippage · Risk scoring
        |
        v
Opportunity Ranking
Priority scoring · Risk-adjusted opportunity list
        |
        v
Storage & Cache
PostgreSQL · MongoDB · Redis · S3 / MinIO
        |
        v
API Layer
Opportunity API · Filters · Watchlist · Alerts · Analytics
        |
        v
Dashboard
Opportunity table · Spread charts · Filters · Alerts · Watchlist
