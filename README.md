# Helios Project

## Overview
The Helios Project is focused on analyzing solar flare data from the Reuven Ramaty High-Energy Solar Spectroscopic Imager (RHESSI) satellite, specifically covering datasets from 2004-2005 and 2015-2016. The aim of this project is to estimate solar flare intensity, discover solar hotspots, and understand solar activity cycles. By leveraging various machine learning techniques, the Helios Project contributes to a better understanding of solar phenomena and their potential impacts on Earth's communication systems, satellites, and power grids.

## Objectives
- Analyze RHESSI solar flare data to estimate flare intensity and track hotspots.
- Develop regression models to predict solar flare intensities based on different predictor values.
- Identify and track patterns in solar activity over time, particularly focusing on the 11-year solar cycle.
- Create visualizations for solar flare intensity and hotspots, helping in understanding the behavior and distribution of solar activity.

## Data
The dataset used in the Helios Project includes solar flare data obtained by the RHESSI satellite, containing attributes such as:
- **Date**: Timestamp of when the flare occurred.
- **Position (x.pos.asec, y.pos.asec)**: Coordinates of the flare on the Sun.
- **Energy (energy.kev.i, energy.kev.f)**: Energy range of the flare, measured in kilo-electron volts (keV).
- **Duration (duration.s)**: Duration of the flare in seconds.
- **Total Count (total.counts)**: Total number of corrected counts for a specific energy range.

## Methodologies
- **Machine Learning Models**: Linear Regression, Support Vector Machines, Decision Trees, Gradient Boosting (XGBoost), and Random Forest were used to estimate solar flare intensity.
- **Hyperparameter Tuning**: RandomizedSearchCV was used to optimize the model's performance by finding the best hyperparameter values.
- **Scaling and Cross-Validation**: Preprocessing methods such as RobustScaler and StandardScaler were tested. Cross-validation was done using RepeatedKFold to ensure robust evaluation.
- **Hotspot Discovery**: Kernel Density Estimation (KDE) was used to identify solar hotspots based on the estimated flare intensities.

## Key Findings
- **Hotspot Patterns**: Hotspots were mostly concentrated along the center of the solar axis. Two types of hotspots were identified—small, highly intense spots (D1) and larger regional hotspots (D2).
- **Solar Cycle Insights**: Analysis of solar flare data indicated a repeating solar cycle, approximately every 11 years, with similar sunspot activity in 2004-2005 and 2015-2016.
- **Intensity Maps**: Visualizations were generated to show the spatial distribution of solar flare intensity. Comparisons showed that solar activity varied significantly across the different time periods analyzed.

## File Structure
- **notebooks/**: Contains Jupyter notebooks used for data exploration, modeling, and visualizations.
- **data/**: Includes the datasets used for training and analysis.
- **models/**: Saved machine learning models.
- **visualizations/**: Images and videos of solar flare intensity maps and hotspot distributions.

## Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/helios-project.git
   ```
2. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebooks in the `notebooks/` directory to explore the data and build models.

## Dependencies
- Python 3.8+
- NumPy
- Pandas
- Scikit-learn
- XGBoost
- Matplotlib
- SciPy
