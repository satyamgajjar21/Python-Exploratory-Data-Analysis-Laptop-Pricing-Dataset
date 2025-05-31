
# 💻 Hands-on Lab: *Exploratory Data Analysis – Laptop Pricing Dataset*

Estimated time needed: **45 minutes**

In this lab you will apply essential EDA techniques to discover how
different hardware and categorical features influence laptop prices.

---

## 🎯 Objectives
By the end of the notebook you will be able to

1. **Visualize** individual feature patterns (scatter plots, box plots).  
2. **Describe** data numerically with `DataFrame.describe()` and value-counts.  
3. **Group & pivot** data to explore categorical effects on price.  
4. **Quantify** relationships with the Pearson correlation coefficient & *p*-values.

---

## 🗂️ Table of Contents
| Section | Description |
|---------|-------------|
| [1. Setup](#1-setup) | Install & import required libraries |
| [2. Load Data](#2-load-data) | Download & read CSV into a DataFrame |
| [3. Visualize Individual Features](#3-visualize-individual-features) | Regressions & box plots |
| [4. Descriptive Statistics](#4-descriptive-statistics) | Numeric & object summaries |
| [5. GroupBy & Pivot](#5-groupby--pivot) | Mean price by GPU × CPU core |
| [6. Correlation & Causation](#6-correlation--causation) | Pearson *r* and *p*-values |
| [7. Conclusions](#7-conclusions) | Key take-aways & next steps |

*Click any section heading above to jump directly to that part of the notebook.*

---

## 1  Setup

This lab uses:

| Library | Purpose |
|---------|---------|
| `pandas` | data manipulation |
| `numpy` | math operations |
| `scipy` | statistical tests |
| `matplotlib`, `seaborn` | visualization |

Install **Seaborn** in JupyterLite:

```python
import piplite, asyncio, sys
await piplite.install('seaborn')
