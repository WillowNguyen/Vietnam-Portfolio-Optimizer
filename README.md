# 📊 Vietnam Stock Portfolio Optimizer  
*A Business Intelligence project turning market data into investable insights*

This repository showcases my **individual project** building a **portfolio optimization and risk analytics** workflow for Vietnam’s stock market using **Python**.  
It applies **Modern Portfolio Theory** (Efficient Frontier, Max Sharpe, Min Vol), **Monte Carlo simulation**, and **risk metrics** (VaR/CVaR) — then visualizes results so **investors and BI teams** can make better decisions with confidence.

---

## 🎯 Business Problem
How can a portfolio be constructed to **maximize risk-adjusted return** while being **transparent and explainable** for stakeholders?  
This project answers it by delivering a BI-friendly analysis: **clear inputs → robust analytics → decision-ready visuals**.

**Key business goals**
- Identify optimal portfolios (Max Sharpe, Min Vol) from VN stocks
- Benchmark against **VNINDEX** / **VN30**
- Quantify risk with **VaR/CVaR** and visualize drawdowns
- Provide **repeatable**, auditable analytics for reporting

---

## 📊 Data
- **Universe**: Vietnamese listed stocks (blue chips across HOSE/HNX/UPCOM)  
- **Source**: VNStock API (prices), Pandas for processing  
- **Frequency**: Daily close (multi-year history)  
- **Benchmarks**: VNINDEX, VN30  

> Data is fetched/processed in the notebook; no proprietary data is stored in the repo.

---

## ⚙️ Methodology (BI-ready)
1) **Data prep & sanity checks**
   - Cleaning, alignment of trading calendars, log-returns, covariance estimation

2) **Monte Carlo Simulation (10k+ portfolios)**
   - Random weight generation with constraints (long-only, sum to 1)
   - Compute **expected return**, **volatility**, **Sharpe ratio**

3) **Efficient Frontier & Optimal Points**
   - Plot frontier; locate **Max Sharpe** and **Min Volatility** portfolios
   - Extract **optimal weights**, risk/return, and KPIs

4) **Risk Intelligence**
   - **Parametric/ Historical VaR** and **CVaR**
   - **Drawdown** analysis for stress view

5) **Benchmarking & Attribution**
   - Compare cumulative performance vs **VNINDEX** / **VN30**
   - Discuss risk-adjusted improvements and sensitivity

---

## 🚀 Results & Business Impact
- Optimized portfolios deliver **superior risk-adjusted performance** vs market benchmarks  
- Clear visualization helps **non-technical stakeholders** understand trade-offs  
- Risk metrics (VaR/CVaR, drawdown) support **scenario planning** and **policy limits**

### Figures
**Efficient Frontier (with optimal points)**  
![Efficient Frontier](Results/efficient_frontier.png)

**Monte Carlo cloud of portfolios**  
![Monte Carlo](Results/monte_carlo_scatter.png)

**Portfolio vs Benchmarks (cumulative return)**  
![Performance vs Benchmarks](Results/performance_vs_benchmarks.png)

**Optimal Weights**  
![Weights Pie](Results/weights_pie.png)

**Correlation Structure**  
![Correlation Heatmap](Results/correlation_heatmap.png)

**Risk Metrics Summary**  
![Risk Table](Results/risk_metrics_table.png)

> All figures are reproducible from the notebook in `/Notebooks`.

---

## 💡 Insights for BA/BI Stakeholders
- **Explainability**: Frontier + weights make portfolio choices defensible in committees.
- **Risk Governance**: VaR/CVaR and drawdown provide policy-grade risk controls.
- **Scenario-friendly**: Easy to rerun with different universes or constraints.
- **Reusable patterns**: The same pipeline fits product P&L, fund reporting, or CIO dashboards.

---

## 📂 Repository Structure
