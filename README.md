# Twitch User Growth Analysis

This project was completed as part of a data science challenge during the hiring process for Patreon. While the challenge permitted the use of any publicly available dataset, I chose to analyse Twitch data to simulate how behavioural insights could inform platform strategies. Given Patreon’s plan to implement live-streaming features, this analysis aimed to identify patterns of user engagement and streamer growth that support sustainable success on creator-driven platforms.

**View the full reports:**
- [R version (HTML report)](https://hanbingo.github.io/twitch-user-growth-analysis/)
- [Python version (HTML report)](https://hanbingo.github.io/twitch-user-growth-analysis/Twitch_Streaming_EDA_Hanbin_Go_Python.html)

---

## Overview

This analysis examined historical Twitch data from 2016 to 2024 to identify predictors of streamer success. It integrated exploratory visualizations, statistical modelling, and clustering to address four key questions:

1. How did global Twitch engagement evolve over time, especially during major events such as COVID-19?
2. What types of content drive viewer engagement and retention?
3. Which streamer behaviours predict follower growth?
4. Can we identify distinct behavioural profiles among top-performing streamers?

---

## Data Sources

- [Top Games on Twitch 2016–2024 (Kaggle)](https://www.kaggle.com/datasets/rankirsh/evolution-of-top-games-on-twitch)
- [Top 1000 Twitch Streamers (May 2024)](https://www.kaggle.com/datasets/hibrahimag1/top-1000-twitch-streamers-data-may-2024)

These datasets included platform-level trends, category insights, and individual streamer performance metrics.

---

## Methods

### R Version
- Data wrangling & visualization: `tidyverse`, `ggplot2`
- Modelling: `lme4` (linear mixed-effects models)
- Clustering: `kmeans`, `factoextra`

### Python Version
- Data wrangling: `pandas`, `numpy`
- Visualization: `matplotlib`, `seaborn`
- Modelling: `statsmodels`
- Clustering: `scikit-learn`

---

## Key Findings

### 1. Viewership Trends (2016–2024)
- Viewership rose steadily until March 2020, then spiked sharply due to lockdowns (+19% in March, +73% in April vs. predictions).
- Concurrent viewership remained high post-pandemic (~2.5 million average in 2023).

### 2. Content Engagement
- Twitch shifted from being game-driven (e.g., League of Legends) to personality-driven.
- **Just Chatting** became the most-watched category, highlighting the role of interactive content.

### 3. Predictors of Follower Growth
From the mixed-effects model:
- **Higher average viewers per stream** predicted greater follower gains.
- **Longer stream durations** were associated with diminishing returns.
- **Greater variety (more games per session)** predicted higher follower growth.

### 4. Behavioural Clusters (Top 1000 Streamers)
Four distinct streamer profiles emerged:
- **Very Active Streamers** – high frequency and duration (largest group)
- **Efficient Casual Streamers** – less active but highly efficient
- **Long-Hours Grinders** – very active but with lower efficiency
- **Top Streamer Stars** – moderate effort, highest growth (likely due to reach)

---

## Deliverables

### R Version
- [`hanbin_go_2025_04_29.Rmd`](./hanbin_go_2025_04_29.Rmd): Source code and analysis
- [`hanbin_go_2025_04_29.html`](./hanbin_go_2025_04_29.html): HTML report

### Python Version
- [`Twitch_Streaming_EDA_Hanbin_Go.ipynb`](./Twitch_Streaming_EDA_Hanbin_Go.ipynb): Python notebook
- [`Twitch_Streaming_EDA_Hanbin_Go_Python.html`](./Twitch_Streaming_EDA_Hanbin_Go_Python.html): HTML report (optional)

---

## Conclusion

Streamer growth was not solely a function of time invested or audience size. Instead, success was associated with:
- Regular engagement (not over-streaming),
- Content diversity,
- A focus on interactive, community-oriented formats.

These insights suggest that platforms like Patreon may benefit from tools that encourage personality-driven streaming and creator-audience interaction.

---

*This project is shared for educational and portfolio purposes only. All data were publicly available; no proprietary information from Patreon was used.*