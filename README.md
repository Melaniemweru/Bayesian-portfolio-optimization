# Bayesian Portfolio Optimization
**Author:** Melanie  
**Date:** April 12, 2025  

> “Investing under uncertainty? Bayesian inference has your back.”

---

## 🚀 What’s This Project About?

This project explores how **Bayesian methods** can be used to **optimize a 3-asset portfolio** (Stock, Bond, Gold) under uncertainty. We estimate the unknown mean returns (\( \mu \)) and covariance matrix (\( \Sigma \)) of asset returns using **Gibbs Sampling** and **Metropolis-Hastings (MH)** — two powerful MCMC techniques.

We go beyond theory by simulating how this portfolio performs in **bull** and **crisis** markets, and visualizing the **efficient frontier** using posterior distributions.

---

## 💡 Why Bayesian?

Unlike classical models that give you fixed estimates, Bayesian Portfolio Optimization gives you **distributions**. This means:

- You model **uncertainty** directly.
- You can simulate portfolios under **various market scenarios**.
- You make more **robust investment decisions**.

---

## 🧠 How It Works

1. **Data:** Historical returns for Stock, Bond, and Gold.
2. **Prior Beliefs:** 
   - \( \mu \sim \text{Multivariate Normal} \)  
   - \( \Sigma \sim \text{Inverse-Wishart} \)
3. **Gibbs Sampling:** Efficient estimation of \( \mu \) and \( \Sigma \).
4. **MH Sampling:** Cross-check and validate Gibbs outputs.
5. **Diagnostics:** Trace plots and density plots for convergence.
6. **Simulation:** Analyze portfolio behavior in:
   - 📈 Bull Market
   - 📉 Crisis Market
7. **Efficient Frontier:** Visualize optimal portfolios using **Sharpe Ratio**.

---

## 📌 Key Insights

- 📈 **Stock**: Highest expected return, moderate volatility — best for growth.
- 💵 **Bond**: Stable, low return — best for risk-averse allocation.
- 🪙 **Gold**: Diversifier with modest returns and hedging potential.
- ❌ **MH vs Gibbs**: Gibbs showed better convergence. MH chains failed to mix.

---


## 🔭 Future Work

- Time-varying models (Dynamic Linear Models)
- Real-world constraints (e.g., transaction costs)
- Alternative priors like LKJ for flexible correlations

---

## 📘 Want to Explore?

Run the `report.Rmd` in RStudio to:

- Reproduce posterior estimates  
- Simulate portfolio returns  
- Visualize risk-return tradeoffs  

---



---

> “In uncertain markets, probability is your edge.”

