# English Premier League 2019-2020 Data Analysis

## Project Overview
This project performs a comprehensive end-to-end analysis of the English Premier League (EPL) 2019-2020 season using Python, Pandas, Altair, and machine learning. The analysis includes data cleaning, exploratory data analysis (EDA), interactive visualizations with linked brushing, referee analysis, and predictive modeling to forecast match outcomes.

## Files Description
- **`EPL_Analysis.ipynb`**: The main Jupyter Notebook containing 12 sections of analysis:
  1. Setup and imports (pandas, altair, scikit-learn)
  2. Data loading and inspection
  3. Data cleaning with quality checks
  4. Feature engineering (9 new features created)
  5. Exploratory data analysis
  6. Team-level performance analysis with linked interactive visualizations
  7. Home advantage analysis
  8. Correlation analysis
  9. Discipline and aggression patterns
  10. Referee strictness analysis
  11. **Predictive modeling** (Logistic Regression & Random Forest)
  12. Comprehensive conclusion
  
- **`cleaned_dataset.csv`**: The processed dataset with handled missing values and engineered features
- **`england-premier-league-2019-to-2020.csv`**: The raw dataset
- **`video_script.md`**: Complete script for the 3-4 minute video presentation
- **`README.md`**: This file

## Data Source
The dataset was obtained from [Sports-Statistics.com](https://sports-statistics.com/sports-data/soccer-datasets/) (English Premier League 2019-2020).

**Dataset Contains:**
- 380 matches from the 2019-20 season
- Match statistics: goals, shots, shots on target, corners, fouls, yellow/red cards
- Team names, referees, and match results

## Prerequisites

Before running this project, ensure you have the following installed on your computer:

1. **Python 3.8 or higher**
   - Download from [python.org](https://www.python.org/downloads/)
   - Verify installation: `python --version`

2. **Jupyter Notebook**
   - Will be installed with the dependencies in Step 1 below
   - Alternatively, install separately: `pip install notebook`

## How to Run

### Step-by-Step Instructions:

**Step 1: Install Required Libraries**
Before opening the notebook, install all required dependencies:
```bash
pip install pandas altair notebook scikit-learn numpy
```

**Step 2: Navigate to Project Folder**
Open your terminal/command prompt and navigate to the project directory:
```bash
cd path/to/project/folder
```

**Step 3: Launch Jupyter Notebook**
```bash
jupyter notebook
```
This will open Jupyter in your default web browser.

**Step 4: Open the Notebook**
- In the Jupyter file browser, click on `EPL_Analysis.ipynb`
- The notebook will open in a new tab

**Step 5: Execute All Cells**
To see all visualizations and outputs properly:
- Go to the menu bar: **Kernel → Restart & Run All**
- Wait 1-2 minutes for all cells to execute
- All interactive charts and results will appear

### What You'll See:
- Interactive Altair charts (with linked brushing - click and drag to select teams)
- Statistical analysis and correlations
- Machine learning model predictions
- Confusion matrices and feature importance
- All 12 sections with comprehensive analysis

## Key Features & Insights

### Interactive Visualizations
- **Linked Brushing**: The Team Archetypes scatter plot features cross-filtering. Select teams by clicking and dragging, and the linked chart below updates automatically.
- **All charts are interactive**: Hover for tooltips, zoom, and pan

### Predictive Modeling (NEW)
- **Models**: Logistic Regression and Random Forest classifiers
- **Target**: Predict match outcome (Home Win / Draw / Away Win)
- **Features**: HST, AST, HC, AC, HF, AF, HY, AY (as per project proposal)
- **Performance**: Achieved 50-60% accuracy with confusion matrix visualization
- **Feature Importance**: Shots on target identified as most predictive factor

### Referee Analysis (NEW)
- Analysis of referee strictness based on average cards per match
- Interactive ranking of all EPL referees
- Insights on officiating styles and tactical implications

### Statistical Findings
1. **Home Advantage**: Home teams win 47% vs 30% for away teams (+17% advantage)
2. **Defense Wins Championships**: Liverpool's defense (14 goals conceded) beat Man City's offense (56 goals scored)
3. **Shot Accuracy is King**: Strongest predictor of success (validated by ML models)
4. **Discipline Doesn't Win Games**: Weak correlation between fouls and points
5. **Referee Variation**: 2-3 card difference between strictest and most lenient officials

## Project Structure
```
project/
│
├── EPL_Analysis.ipynb          # Main analysis notebook (REQUIRED)
├── cleaned_dataset.csv          # Processed data (REQUIRED)
├── england-premier-league-2019-to-2020.csv  # Raw data (REQUIRED)
├── README.md                    # This file (REQUIRED)
├── video_script.md              # Video presentation script
└── project_submission.zip       # Submission package
```

## Technologies Used
- **Python 3.8+**
- **Pandas & NumPy**: Data manipulation and analysis
- **Altair**: Interactive visualizations with linked brushing
- **scikit-learn**: Machine learning (Logistic Regression, Random Forest)
- **Jupyter Notebook**: Interactive development environment

## Academic Integrity Statement
This project represents original analysis and code. All external code has been properly cited. The dataset source is credited above. The predictive modeling and interactive visualizations fulfill the requirements stated in the project proposal.

## Contact
For questions about this analysis, please refer to the detailed explanations and interpretations provided throughout the Jupyter Notebook.
