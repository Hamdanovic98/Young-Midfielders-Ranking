# Ranking Young Midfielders Based on Possession-Adjusted Statistics
## Project Overview
This project aims to identify and rank young midfielders who can excel in the Championship by analyzing possession-adjusted statistics. The analysis was conducted as part of a take-home project for a Recruitment Analyst position at SRC FTBL. The objective is to find versatile players with strong attributes both in and out of possession, who also have potential resale value.

## Dataset
The dataset includes player statistics for various positions. The data covers multiple seasons and includes metrics for both in-possession and out-of-possession actions.

## Methodology
### Data Filtering and Preparation
#### Filtering Criteria:

Players strictly under 25 years old were selected to focus on young talents.
Only midfield positions relevant to the project (single pivot, double pivot, and #8) were included.
Missing values were handled by excluding entries with incomplete critical information, such as birthdates.
#### Creating Aggregated Data:

Players' statistics were aggregated by position to handle cases where players played in multiple positions.
### Possession-Adjusted Statistics
#### In-Possession Statistics:

Normalized by dividing by the percentage of time the player's team had possession (player-match-possession).
#### Out-of-Possession Statistics:

Adjusted by multiplying by 30 and dividing by the opponent possession time, standardizing to a 50% possession scenario.
#### Normalization:

All statistics were normalized by dividing by a new column named 90s, which is calculated as minutes-played divided by 90 to get the stats per game.
### Ranking Players
#### Scoring System:

Players were ranked based on a composite score of their normalized in-possession and out-of-possession statistics.
Positive and negative weights were assigned to different metrics based on their impact on performance.
#### Final Ranking:

The top-ranked players were identified and analyzed for their potential to contribute to the team and their resale value.
### Results
The final results include a shortlist of the top young midfielders who meet the criteria and demonstrate strong performance based on possession-adjusted statistics.

### Files in the Repository
Data_Filtering_and_Preparation.ipynb: Jupyter Notebook for data filtering and preparation.

Ranking_Players.ipynb: Jupyter Notebook for possession adjustment and player ranking.

Top Targets Presentation.pptx: Presentation highlighting the potential targets.

The Approach of Identifying Top Young Versatile Midfielders.pdf: Detailed report describing the methodology and results.
## How to Use
### Clone the Repository:

git clone https://github.com/yourusername/young-midfielders-ranking.git
cd young-midfielders-ranking

### Install Dependencies:
Ensure you have Python and Jupyter Notebook installed.
Install the required Python packages using:

pip install -r requirements.txt

## Run Jupyter Notebooks:
Open and run the provided Jupyter Notebooks to understand the data preparation, possession adjustment, and ranking process.

## View the Presentation:
Open the Top Targets Presentation.pptx file to see the final presentation.

## Read the Report:
Open the The Approach of Identifying Top Young Versatile Midfielders.pdf file to read the detailed methodology and results.

## Conclusion
This project demonstrates a systematic approach to identifying and ranking young midfielders using possession-adjusted statistics. By focusing on key metrics and normalizing them based on possession, we can fairly compare players from different teams and make informed decisions for player recruitment.

## Acknowledgements
I would like to thank SRC FTBL for the opportunity to work on this project and for their inspiring work in football analytics.