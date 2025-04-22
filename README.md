# IPL Data Analysis

This project performs an in-depth analysis of the Indian Premier League (IPL) cricket dataset using Apache Spark. The analysis focuses on various metrics, such as top scoring batsmen, economical bowlers, and the impact of winning the toss on match outcomes. The dataset contains match, player, ball-by-ball data, and more, enabling insights into IPL match statistics.

## Project Overview

The goal of this project is to use Apache Spark with PySpark for processing and analyzing IPL data. The following aspects are covered in the analysis:
- **Top Scoring Batsmen per Season**: Identifying the highest run-scorer for each season.
- **Economical Bowlers in Powerplay**: Finding bowlers with the best economy rate during the powerplay overs.
- **Impact of Winning Toss**: Analyzing whether winning the toss has any significant impact on the match outcome.
- **Runs Scored in Wins**: Analyzing the runs scored by players in matches that their team won.
- **Scores by Venue**: Determining the average score and highest score by venue.
- **Team Performance after Winning Toss**: Analyzing teams’ performance after winning the toss.

## Dataset

The project uses multiple CSV files that contain data related to IPL matches, players, ball-by-ball events, and teams. The dataset includes the following files:
- `Ball_By_Ball.csv`: Contains detailed ball-by-ball information such as runs scored, wickets, extras, and match details.
- `Match.csv`: Contains details about each match, such as teams playing, match winner, and toss information.
- `Player.csv`: Contains player-related data, including player names, batting hand, bowling skill, and country.
- `Player_match.csv`: Contains information on players' performance in each match.
- `Team.csv`: Contains data about teams participating in the IPL.

## Technologies Used

- **Python**: The project uses Python for data processing and analysis.
- **Apache Spark**: PySpark is used for distributed data processing, enabling efficient analysis of large datasets.
- **Matplotlib & Seaborn**: Used for data visualization and presenting insights in the form of charts and graphs.
- **Google Colab**: The project is developed and executed in Google Colab for easy sharing and execution in an online environment.

## Project Structure


- **`Ball_By_Ball.csv`**: Ball-by-ball data for matches.
- **`Match.csv`**: Information about each match played in the IPL.
- **`Player.csv`**: Information about players.
- **`Player_match.csv`**: Player performance data for each match.
- **`Team.csv`**: Data about the teams participating in IPL.
- **`IPL_Data_Analysis.ipynb`**: Jupyter notebook with the analysis code.
- **`README.md`**: Documentation for the project.

## How to Run

To run this project, you need to execute the Jupyter notebook `IPL_Data_Analysis.ipynb` in a Python environment with the necessary libraries installed. You can use Google Colab to execute the notebook without any setup.

1. Open the `IPL_Data_Analysis.ipynb` file in Google Colab.
2. Make sure the required libraries are installed by running the first few cells. These libraries include:
   - `pyspark`
   - `matplotlib`
   - `seaborn`
3. Upload the datasets to the appropriate location in Google Drive or provide the correct file paths to the dataset.
4. Run the notebook to perform the analysis.

## Steps Performed in the Analysis

1. **Data Loading & Preprocessing**:
   - Loaded CSV files using PySpark and defined custom schemas to ensure proper data types.
   - Cleaned and transformed data, including handling missing values and correcting date formats.

2. **Top Scoring Batsmen per Season**:
   - Calculated the total runs scored by each batsman in each season.
   - Identified the batsman with the highest total runs for each season.

3. **Economical Bowlers in Powerplay**:
   - Analyzed the performance of bowlers in the first 6 overs of each match.
   - Calculated the economy rate for bowlers and ranked them based on their economy rate and wickets taken.

4. **Impact of Winning Toss**:
   - Analyzed the impact of winning the toss on the match outcome.
   - Compared toss winner and match winner data to identify patterns.

5. **Runs Scored in Wins**:
   - Analyzed runs scored by players in matches that their team won.
   - Ranked players based on runs scored in winning matches.

6. **Scores by Venue**:
   - Analyzed match scores by venue, calculating average and highest scores per venue.

7. **Team Performance After Winning Toss**:
   - Examined team performance after winning the toss.
   - Analyzed how many matches were won by teams after they won the toss.

## Visualizations

Several visualizations have been created to highlight insights from the analysis:

- **Economical Bowlers in Powerplay**: A bar chart showing the top 10 bowlers with the best economy rate in powerplay overs.
- **Impact of Winning Toss**: A count plot showing the number of matches won after winning the toss.
- **Runs Scored in Wins**: A bar chart of the top batsmen who scored the most runs in winning matches.
- **Scores by Venue**: A bar chart showing the average score at each venue.
- **Team Performance after Winning Toss**: A bar chart showing the number of wins after winning the toss for each team.

## How to Contribute

Feel free to fork the repository and submit pull requests for any improvements, bug fixes, or additional features. Contributions are always welcome!

## License

This project is open-source and available under the [MIT License](LICENSE).


