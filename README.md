# SpendDNA — Your Wallet's Year-End Story

**"Spotify Wrapped for your money."**

A Python-based transaction analytics tool that decodes 6 months of synthetic Indian UPI/bank transaction data for a fictional Bengaluru software engineer, Rahul Sharma. SpendDNA parses messy, real-world-style bank export data, extracts canonical vendor names, categorizes spending across 12 categories, detects spending personality archetypes, flags anomalous transactions, and prints a clean, screenshot-worthy financial report — all using only core Python, NumPy, and Pandas.

##  What It Does

- **Transaction Parser** — cleans 4 mixed date formats and 3 mixed amount formats, standardizes debit/credit types, removes duplicates

- **Vendor Extractor** — maps ~35 messy merchant description variants to canonical vendor names (e.g. `POS SWIGGY BANGALORE`, `BUNDL Tech P L` → `Swiggy`)

- **Category Tagger** — classifies every transaction into 12 spending categories (Food Delivery, Quick Commerce, E-commerce, Investments, etc.)

- **Spending Overview** — total income, expenses, net savings, savings rate, top vendors and categories

- **Monthly Trend Analysis** — category-wise spending across 6 months, biggest month-on-month growth/decline

- **Time-of-Day Patterns** — peak spending hours per category, late-night food-delivery behavior

- **Anomaly Detection** — z-score based flagging of unusually large transactions per category

- **Spending Archetype Detection** — classifies Rahul into personality archetypes (Foodie, Investor, YOLO Spender, etc.) based on quantitative rules

---

##  Tech Stack & Constraints

Built entirely with:

- Python fundamentals (strings, dicts, functions, f-strings)

- NumPy

- Pandas (`groupby`, `pivot_table`, `.dt`, `.str`, `transform`)

- `datetime`



## ▶️ How to Run

1. Clone or download this repository

2. Ensure `rahul_transactions.csv` is in the same folder as the notebook

3. Open `SpendDNA_Samrudhi.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab

4. Run all cells top to bottom (`Kernel → Restart & Run All` / `Runtime → Restart and run all`)

5. The final cell prints the full formatted report to the console

**Requirements:** Python 3.x, pandas, numpy

```bash

pip install pandas numpy

```

---

## 📁 Repository Contents

| File | Description |

|---|---|

| `SpendDNA_Samrudhi.ipynb` | Main analysis notebook |

| `rahul_transactions.csv` | Synthetic 6-month UPI transaction dataset (1,328 rows) |

| `README.md` | This file |

---

## 👤 About

Built as part of **The Unlox Academy — Week 2 Minor Project (SpendDNA)**, Data Science Program.

**Author:** Samrudhi Shetty

**Batch:** Data Science August 2026

---

## ⚠️ Note

This project runs exclusively on the provided synthetic dataset (`rahul_transactions.csv`). No real personal financial data is included in this repository.
