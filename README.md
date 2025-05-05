# Twitch User Growth Analysis

This project was completed as part of a data science challenge during the hiring process for Patreon. While the challenge permitted the use of any publicly available dataset, I chose to analyse Twitch data to simulate how behavioural insights could inform platform strategies. Motivated by Patreon’s plan to implement live-streaming features on their platform, this analysis focused on identifying patterns of user engagement and streamer growth that contribute to sustainable success on creator-driven platforms.

## Overview

The analysis focused on identifying predictors of streamer success by examining historical Twitch data from 2016 to 2024. It combined exploratory data visualization with statistical modeling and clustering to answer the following key questions:

1. How did global Twitch engagement change over time, particularly during major events such as the COVID-19 pandemic?
2. What content types drive viewer engagement and retention?
3. Which streamer behaviours are most predictive of follower growth?
4. Can we identify distinct behavioural profiles among top-performing streamers?

## Data Sources

* [Top Games on Twitch 2016–2024 (Kaggle)](https://www.kaggle.com/datasets/rankirsh/evolution-of-top-games-on-twitch)
* [Top 1000 Twitch Streamers Data (May 2024)](https://www.kaggle.com/datasets/hibrahimag1/top-1000-twitch-streamers-data-may-2024)

Data included platform-wide metrics, game/category-level trends, and individual streamer performance.

## Methods

* Data wrangling and visualization: `tidyverse`, `ggplot2`
* Modelling: `lme4` for linear mixed-effects modelling
* Clustering: `kmeans`, `factoextra`

## Key Results

### Viewership Trends (2016–2024)

* Viewership steadily increased until March 2020, when global lockdowns caused a sharp spike (+19% in March and +73% in April compared to predictions).
* Average concurrent viewers remained elevated even after the pandemic surge, with \~2.5 million in 2023.

### Content Engagement

* Historically game-driven (e.g., League of Legends), Twitch shifted toward personality-driven content.
* **Just Chatting** became the most-watched category, highlighting a preference for interactive, conversational streams.

### Follower Growth Predictors

Using a linear mixed-effects model:

* **More average viewers per stream** predicted higher follower gains.
* **Longer stream durations** predicted fewer followers per stream, suggesting diminishing returns with excessive stream length.
* **Streaming more games per session** predicted more followers, potentially due to content variety.

### Behavioural Clusters

Clustering top 1000 streamers revealed four distinct groups:

* **Very Active Streamers** – frequent and long-duration streamers (largest group)
* **Efficient Casual Streamers** – less active but high follower efficiency
* **Long-Hours Grinders** – very active but less efficient in follower gain
* **Top Streamer Stars** – moderate effort with the highest follower growth (likely aided by brand reach)

## Deliverables

* [`hanbin_go_2025_04_29.Rmd`](./hanbin_go_2025_04_29.Rmd): Source code and analysis
* [`hanbin_go_2025_04_29.html`](./hanbin_go_2025_04_29.html): Final report with figures and insights

## Conclusion

Streamer success is not solely determined by total stream hours or raw audience size. Instead, consistent weekly engagement, moderate session lengths, and diverse content strategies were associated with efficient growth. These findings support the idea that platforms like Patreon may benefit from tools that promote conversational, community-driven content alongside traditional formats.

---

*This project is shared for educational and portfolio purposes only. All data used were publicly available and no proprietary information from Patreon was involved.*
