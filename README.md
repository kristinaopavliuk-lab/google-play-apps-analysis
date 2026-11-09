# What Makes a Mobile App Successful?

Analysis of 10,000+ Google Play apps and 37,000+ user reviews to help a product team choose a category and a monetization model for a new Android app.

## Business question
A team with a limited budget wants to know which category and model (free or paid) give a new app better chances of getting installs and good ratings.

## Key findings
- **ENTERTAINMENT has high demand and low competition.** 84% of its apps reach 1M+ installs, compared with 35% across all apps, while it ranks only 24th of 33 categories by number of apps.
- **Users rate ENTERTAINMENT apps lower.** Only 17% of its apps are rated 4.5+, compared with 29% overall. High demand with lower ratings suggests that a high-quality app could stand out.
- **Free apps get more installs, paid apps get better ratings.** Median installs: 100,000 for free apps vs 1,000 for paid apps. 47% of paid apps are rated 4.5+, compared with 28% of free apps (chi-square test, p < 0.001).
- **GAME has the most negative reviews:** 37%, compared with 22% across all reviews.

## Recommendation
Consider ENTERTAINMENT for a pilot app with a free model, and focus on quality to stand out from competitors.

## Data
[Google Play Store Apps](https://www.kaggle.com/datasets/lava18/google-play-store-apps) on Kaggle (2018): app details and user reviews with sentiment.

## Approach
- Cleaned the data: converted text columns to numbers and dates, removed a broken row and duplicates
- Measured demand with median installs and the share of apps with 1M+ installs
- Measured quality with the share of apps rated 4.5+, only for apps with 100+ reviews
- Tested the free vs paid difference with a chi-square test

## Limitations
- The data is from 2018 and is a sample, not the whole store
- Installs is a lower bound of a range
- There is no data on revenue or user retention
- The analysis shows associations, not causes

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, SciPy

## Files
- `google_play_analysis_EN.ipynb`: full analysis with code and charts
