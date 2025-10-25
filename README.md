Baseball Swing Analytics: Predicting Whiffs and Hard-Hit Balls
This project analyzes MLB pitch and swing data to predict swing outcomes like whiffs and hard-hit balls. 

Using player and pitch metrics, we generate actionable coaching insights, including optimal swing bands and pitch-specific strategies.

Dataset: Statcast pitch-level data for the 2024 season, provided by SFU DSSS and CSAS 2025
Key columns: release_speed, spin_rate, bat_speed, swing_length, pitch_type, description, launch_speed.

1. Open 'notebooks/Whiff and HardHit Percentage.ipynb' in Jupyter Notebook.
2. Run cells in order to:
    - Load data
    - Clean and filter swings
    - Generate visualizations
    - Train logistic regression models
3. Outputs: Whiff zone map, swing band heatmap, power trade-off curve, pitcher report.

Key Insights:
- Optimal swing band: 67–72 mph bat speed & 6–8 ft swing length
- High velocity up-and-in pitches increase whiffs unless batter's bat speed >72 mph
- Hard-hit probability plateaus beyond 72 mph

Project Structure:
├── data/                 # Raw CSV files
├── notebooks/            # Jupyter notebooks with analysis and visualizations
├── graphs/               # Graphs for visualization
├── requirements.txt      # Package dependencies
└── README.md             # Project overview