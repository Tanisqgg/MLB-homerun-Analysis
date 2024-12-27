# The Evolution of Average Home Runs in Major League Baseball

## Overview
This project analyzes the evolution of average home runs in Major League Baseball (MLB) by comparing two distinct decades: 1901-1910 and 2001-2010. It provides a detailed examination of changes in home run rates over time, utilizing data visualization, statistical tests, and hypothesis testing.

## Dataset
The dataset used for this project is the **`mlb_teams`** dataset, sourced from:
- [OpenIntro](https://www.openintro.org/data/index.php?data=mlb_teams)
- [Lahman’s Baseball Database](https://github.com/cdalzell/Lahman)

### Dataset Description
- **Rows**: 2784
- **Columns**: 41
- **Variables Used**: `year`, `decade`, `homeruns`, `games_played`, `n`, `mean`, `sd`
- **Time Range**: 1901-1910 and 2001-2010
- **Focus**: Comparing average home runs per game across decades.

## Key Features
1. **Data Preprocessing**:
   - Filtered the dataset for the specified decades.
   - Calculated `home runs per game` as the key metric.

2. **Statistical Analysis**:
   - Confidence intervals for average home runs.
   - Hypothesis testing to assess significant differences between decades.

3. **Visualization**:
   - Line graphs showing trends in home runs per game.
   - Residual plots to evaluate model fit.
   - Density plots and bar graphs for decade-specific comparisons.

4. **Significant Historical Context**:
   - Early 1900s: Focus on contact hitting.
   - Early 2000s: Rise in power hitting, with influences from steroids and longer seasons.

## Findings
- Average home runs per game have significantly increased over time:
  - **1901-1910**: 0.22 - 0.32 (95% confidence interval)
  - **2001-2010**: 2.02 - 2.18 (95% confidence interval)
- A **p-value of 6.10e-17** strongly supports that home run rates differ significantly between the two decades.
- Influences on trends include changes in season length, team numbers, player focus, and steroid usage.

## Tools and Libraries
- **Language**: R
- **Libraries**:
  - `ggplot2`: Data visualization
  - `dplyr`: Data manipulation
  - `stats`: Statistical analysis
