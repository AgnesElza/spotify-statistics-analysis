
# 🎶 What Makes a Song a Hit?  
**A Multi-Perspective Statistical Analysis Using Spotify Data (2000–2020)**

This project explores the audio and metadata characteristics that influence whether a song becomes a **Spotify hit**, using a full-stack data science approach:

> **Statistical testing → Causal inference → Bayesian estimation**  
> to rigorously answer: _“Does increasing danceability make a song more popular?”_

---

## 🧠 Project Goals

- Identify which features correlate with hit potential
- Estimate the **causal effect** of danceability using Propensity Score Matching
- Quantify **uncertainty** using Bayesian A/B testing
- Develop a clean, dashboard-style visual summary of results

---

## 📁 Project Structure

```bash
.
├── data/
│   └── spotify_2000_2020.feather     # Cleaned dataset
├── notebooks/
│   ├── 01_eda_probability.ipynb      # Distribution, conditional probs, rare event framing
│   ├── 02_hypothesis_testing.ipynb   # Danceability vs hit significance test
│   ├── 03_bootstrapping_anova.ipynb  # Bootstrapped means & ANOVA on explicit
│   ├── 04_regression_models.ipynb    # Linear + logistic regression
│   ├── 05_causal_inference.ipynb     # DAGs, Propensity Score Matching
│   ├── 06_bayesian_inference.ipynb   # Bayesian A/B test with PyMC
│   └── 07_summary_visualizations.ipynb # Dashboard-ready visuals
```

---

## 📊 Key Results

| Method | Insight |
|--------|--------|
| 🎯 **Danceability** | Strongest positive predictor of popularity |
| 🧪 **Hypothesis Test** | High danceability triples hit probability |
| 📈 **Regression** | Danceability has the highest standardized effect |
| 🧠 **Causal Inference** | +1.28 point ATE (matched analysis) |
| 📈 **Bayesian Inference** | 95% credible interval for hit lift: **[1.2%, 1.8%]** |

---

## 📦 Tools & Libraries

- `pandas`, `numpy`, `seaborn`, `matplotlib`
- `statsmodels`, `scikit-learn`
- `pymc`, `arviz` for Bayesian inference
- `networkx` for DAG sketching

---

## 🧭 How to Reproduce

1. Clone this repo
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Run notebooks in order inside `notebooks/`

---

## 📌 Use Cases

- Product and feature analysis in media platforms
- A/B testing and experimentation design
- Causal storytelling 
- Bayesian thinking applied to real-world classification

---

## ✨ Inspiration

This project simulates how a **Product Data Scientist** at Spotify might:
- Evaluate what truly causes a track to succeed
- Navigate ambiguity using statistical reasoning
- Communicate results with visual clarity and rigor

---

## 🔗 License

MIT License.