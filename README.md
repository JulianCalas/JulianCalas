# Julian Calas

**Sports data analyst** focused on baseball and player development, with projects across the NBA, NFL and MLB.

I coached as an assistant for Barry University varsity baseball, where I tracked game and practice stats live, built Excel reports for the staff, and wrote scouting reports on opposing pitchers. I hold a B.S. in Economics and International Affairs from Florida State University and a BrainStation Data Analyst Certification, and I work with loan data every day as a credit analyst at NewDay USA. I speak fluent Spanish.

## Portfolio projects

### ⚾ [MLB Statcast Stuff+ pitch quality model](https://github.com/JulianCalas/mlb-stuff-plus-pitch-analysis)
A Stuff+ style model that grades pitches only on physical traits (velocity, spin, movement, release, approach angles, fastball gaps), trained on 2.1 million Statcast pitches from 2024 to 2026.
- The grade stabilizes fast: split-half reliability is 0.75 at 100 pitches, while actual run value is still 0.32 at 1,000 pitches. Year over year Stuff+ correlates 0.78, against 0.21 for ERA.
- Approach angles and break drive the grade more than raw velocity (SHAP).
- Includes a player development memo on Marlins LHP John King and a one-page opposing-pitcher scouting card.
- *Python, LightGBM, Gaussian mixture clustering, SHAP, DuckDB/SQL, Streamlit*

### 🏈 [NFL 4th-down decision bot](https://github.com/JulianCalas/nfl-fourth-down-bot)
Custom win probability, conversion, field goal and punt models combined into a go/punt/kick recommendation for every 4th down, built on 580,005 nflverse plays from 2014 to 2025 and graded on seasons each model never saw.
- Coaches went for it only 27% of the time the model said to, which is where most lost win probability comes from.
- Aggressiveness on clear "go" calls rose from 31% in 2018 to 54% in 2025.
- Win probability log loss of 0.452, close to nflfastR's spread-adjusted model (0.444) and better than its plain model (0.481).
- *Python, gradient boosting, GLMs, calibration, decision analysis, DuckDB/SQL, Streamlit*

### 🏀 [NBA shot quality model](https://github.com/JulianCalas/nba-shot-quality-model)
Expected field goal % and points over expected for every shot, separating shot making from shot selection.
- On 219,100 held-out 2025-26 shots, LightGBM beats the zone-average baseline (log loss 0.639 vs 0.657) and is well calibrated.
- Shrinkage keeps small samples off the leaderboards. Kevin Durant, Nikola Jokić and Shai Gilgeous-Alexander lead shot making, and Rudy Gobert has the best shot selection.
- *Python, logistic regression, LightGBM, empirical Bayes shrinkage, DuckDB/SQL, matplotlib shot charts, Streamlit*

## Skills
**Languages and tools:** Python (pandas, NumPy, scikit-learn, LightGBM, matplotlib), SQL (DuckDB, SQLite), Excel, Tableau, Google Sheets, Git, Streamlit
**Methods:** regression and classification, gradient boosting, calibration, season-based validation, Bayesian shrinkage, clustering, SHAP, win probability and decision models
**Domains:** baseball pitch tracking (Statcast), NFL play-by-play, NBA shot data, player development and scouting reports
