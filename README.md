Professional sports teams and analysts increasingly rely on advanced analytics to inform roster decisions, player development, and fan engagement strategies.
In this study, we apply the Knowledge Discovery in Databases (KDD) process to:

Select & pre-process NBA player performance data (1950–present).

Explore relationships between key metrics (points, assists, rebounds, FG%).

Build & evaluate a CNN‑based classifier to predict All‑Star selections.

Assess model performance (accuracy, AUC) and derive actionable insights for sports analytics.


Data & Features
Source: Kaggle NBA player statistics dataset (1950–present)

Key features:

Points per Game (PPG)

Assists per Game (APG)

Rebounds per Game (RPG)

Field Goal Percentage (FG%)

…and other per‑game and rate metrics

Target: Binary label indicating whether a player was selected as an NBA All‑Star in a given season.

🛠️ Methodology
KDD Process

Selection: Extract relevant seasons and players.

Preprocessing: Handle missing values, normalize metrics, balance classes.

Transformation: Create rolling‑window features and season‑level aggregates.

Summarization: Statistical summaries & correlation heatmaps.

Evaluation: Train/test split (80/20), cross‑validation on training set.

Model Architecture

Convolutional layers to capture local patterns across feature windows

Dense layers with dropout for regularization

Sigmoid output for binary classification

Training & Evaluation

Optimizer: Adam

Loss: Binary Cross‑Entropy

Metrics:

Accuracy: 90.06% on test set

AUC: 0.95

📈 Results & Insights
High predictive power (90.06% accuracy) indicates player stats are strong signals for All‑Star selection.

The CNN effectively captures feature interactions over seasonal windows.

Feature importance analysis highlights PPG and FG% as top predictors, but assists and rebounds also contribute meaningfully.

Demonstrates the value of deep learning in sports analytics for complex pattern recognition.
