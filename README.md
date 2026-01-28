# Supply Imbalance & Supply Decay Analyzer

**A DataForSEO-Based Decision Support Tool**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ekawahara01/Supply-Imbalance-Analyzer/blob/main/Supply_Imbalance_Analyzer.ipynb)

## 📊 Overview

The **Supply Imbalance & Supply Decay Analyzer** is a specialized market diagnostic tool designed to answer one core question:

> **"Do existing solutions exist — and if so, are they structurally failing to serve the market?"**

Unlike traditional SEO tools that focus on *demand* (keyword volume, difficulty), this tool focuses entirely on **supply quality**. It detects markets where supply exists but is outdated, fragile, or structurally inefficient—signaling a prime opportunity for disruption.

## 🎯 Key Differentiators

| Traditional SEO Tools | Supply Imbalance Analyzer |
|-----------------------|---------------------------|
| Focus on **Keyword Difficulty** | Focus on **Supply Fragility** |
| Measures **Domain Authority** | Measures **Supply Decay** |
| Identifies **Competitors** | Identifies **"Zombie Supply"** |
| "Can I rank?" | "Is the current market failing?" |

## 🧠 Core Metrics

### 1. Supply Health Score
A composite score (0-100) evaluating the structural integrity of the top search results.
*   **Dimensions**: Domain diversity, content freshness, maintenance signals.
*   **Verdict**:
    *   🔴 **Underserved** (<40): Supply is failing. Green light for entry.
    *   🟡 **Balanced**: Healthy market.
    *   🟢 **Saturated** (>80): Over-served. Avoid.

### 2. Supply Effort–Value Gap Index (SEVGI)
A proprietary metric to identify "Zombie Supply"—incumbents that rank due to legacy authority but deliver low value relative to their maintenance effort.

$$ \text{SEVGI} = \frac{\text{Content Complexity} \times \text{Maintenance Cost}}{\text{Search Visibility Outcome}} $$

*   **High SEVGI**: Identifies weak incumbents vulnerable to modern, efficient replacement.

## 🚀 How to Use

This tool is designed as a **zero-setup** Jupyter Notebook.

### Option 1: Run in Google Colab (Recommended)
1.  Click the "Open in Colab" badge above.
2.  Enter your **DataForSEO API Key** in the configuration cell.
3.  Select `Runtime > Run all`.

### Option 2: Run Locally
1.  Clone this repository.
2.  Install dependencies: `pip install pandas requests matplotlib seaborn`
3.  Open `Supply_Imbalance_Analyzer.ipynb` in Jupyter Lab or VS Code.

## 🛠️ Tech Stack & Architecture

*   **Core Engine**: Python (Pandas, NumPy)
*   **Data Source**: [DataForSEO API](https://dataforseo.com/) (Live SERP Data)
*   **Visualization**: Matplotlib / Seaborn
*   **Architecture**: Two-Layer Model (Rule-based Core + Optional AI Interpretation)

## 💰 Cost Efficiency
The tool includes a built-in **Efficiency Engine** that tracks API usage costs versus traditional enterprise SEO tools, typically demonstrating a **>90% cost reduction** for ad-hoc market analysis.

## ⚠️ Disclaimer
*This tool evaluates supply-side structure and sustainability. It does not measure total addressable market (TAM), revenue potential, or guarantee search rankings. It is a decision-support instrument, not a financial predictor.*
