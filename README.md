# Hybrid-Real-time-trading-reporting-MQL5-FastAPI-SQLite-PowerBI-
Developed a full-stack, low-latency data pipeline to capture execution data from a MetaTrader 5 Expert Advisor (MQL5) and present real-time performance analytics in a customizable Power BI dashboard. The solution enforces data integrity by using an API (FastAPI) to validate, clean, and store trade data in a centralized database.

## 📖 Introduction
This project integrates **MetaTrader 5 (MQL5 Expert Advisor)** with a **FastAPI service** and a **SQLite3 database**, enabling real‑time trade logging and reporting. Data is visualized in **Power BI**, creating a hybrid workflow for trading telemetry and analytics.

**Key Components**
- API: FastAPI (Python 3.13)
- Database: SQLite3 (`trades` table)
- Writer: MT5 EA (MQL5)
- Include files: `common_utils.mqh`
- Reader: Power BI via ODBC (Christian Werner SQLite driver recommended)

---

## 🏗 Architecture
```text
MT5 EA (MQL5) → FastAPI (Python 3.13) → SQLite3 (trades table) → Power BI (ODBC)
