# 🎮 Steam Data Analysis & Game Recommendation System

## 📌 Motivation

In late 2023, Steam revised its regional pricing policy for Turkey, resulting in a dramatic price increase due to dollarization. As an active user since 2020, I wanted to reflect on my game library and create a personal analytical summary — part retrospective, part exploratory project — before my usage habits inevitably change. This project analyzes my Steam game data and uses machine learning to generate recommendations and insights.

---

## 📦 Data Collection

This project required combining data from multiple sources:

- **Steam Web APIs** to retrieve my personal game library and playtime statistics.
- **SteamDB** for pricing and release date information via web scraping.
- Data was cleaned and merged into a unified `.csv` file for analysis.

---

## 📊 Data Analysis

Initial steps involved exploring and visualizing the dataset:

- Calculated **correlations** between features.
- Created two custom metrics:
  - **Cost per Hour** = Price / Playtime
  - **Worthness** = A custom metric to evaluate the value of a game based on both cost and engagement.
- Generated visualizations to understand my spending and playing habits.

---

## 🤖 Machine Learning

### Supervised Learning

- Labeled the dataset as **played** vs **unplayed** games.
- Trained a regression model (e.g., Linear Regression) on played games to predict:
  - Expected **playtime** for unplayed games.
  - Expected **worthness**, based on predicted playtime.
- Output:
  - Top 20 unplayed games by predicted playtime.
  - Top 20 unplayed games by predicted worthness.

### Unsupervised Learning

- Applied clustering techniques (e.g., KMeans) to identify patterns in:
  - **Playtime vs. Price**
  - **Playtime vs. Release Date**
  - **Price vs. Release Date**

---

## 📌 Key Findings

- I tend to prefer **cheaper and older games**.
- I generally get **good value** from the games I buy.
- The model predicts I would enjoy the **Steins;Gate** series, based on my previous play history.
- My current worthness metric may need refinement, as several low-ranked games are still ones I consider worthwhile.
- Game data clusters around lower price and lower playtime, suggesting a preference for shorter, budget-friendly titles.

---

## 🚀 Future Improvements

- Add **genre classification** to better understand genre-specific preferences.
- Use **genre-based supervised models** to improve game suggestions.
- Enable users to input a **Steam ID** to generate personalized recommendations.
- Train a **neural network** using data from multiple users to cluster player types and improve prediction quality.
- Add a module for predicting whether a given game aligns with my preferences based on past behavior.

---

## 🧰 Tech Stack

- **Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Requests, BeautifulSoup
- **Data Sources**: Steam Web API, SteamDB

---

## 📁 Project Structure

