Baseball Swing Analytics: Predicting Whiffs and Hard-Hit Balls

This project analyzes MLB pitch and swing data to predict swing outcomes like whiffs and hard-hit balls. 

Using player and pitch metrics, we generate actionable coaching insights, including optimal swing bands and pitch-specific strategies.

We had 2 people work on jupyter notebooks for data analysis. Because we wanted to work in sync, we have 2 seperate jupyter notebooks. Each has different graphs that are going to be used in our presentation

Dataset: Statcast pitch-level data for the 2024 season, provided by SFU DSSS and CSAS 2025
Key columns: release_speed, spin_rate, bat_speed, swing_length, pitch_type, description, launch_speed.

How to run:
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
├── data/                 # Raw CSV files and links to source
├── notebooks/            # Jupyter notebooks with analysis and visualizations
    ├── Baseballtin.ipynb # Matthew's work, machine learning models and some heatmaps
    └── Whiff and HardH.. # Simon's work, graphs, visualization, cleaning
├── graphs/               # Graphs for visualization
├── requirements.txt      # Package dependencies
├── flowchart.md          # In depth description of our working process
└── README.md             # Project overview

Future Work:
- Extend to player-specific models
- Integrate pitch sequencing for dynamic strategy
- Deploy an interactive dashboard for coaches

