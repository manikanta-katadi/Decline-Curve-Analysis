# Decline Curve Analysis (DCA) of an Oil Well

## Project Overview

This project involved performing Decline Curve Analysis (DCA) on historical oil well production data to evaluate production performance, compare Arps decline models, forecast future oil production, estimate the productive life of the well, and calculate the Estimated Ultimate Recovery (EUR). The complete workflow was implemented in Python using Jupyter Notebook during my Summer Internship at ONGC – Institute of Reservoir Studies (IRS), Ahmedabad.

------------------------------------------------------------

## Project Objective

- Analyze historical oil well production data.
- Apply Arps Decline Curve Analysis (DCA).
- Compare Exponential, Hyperbolic, and Harmonic decline models.
- Select the best-fit decline model using statistical evaluation.
- Forecast future production until the economic limit.
- Estimate Estimated Ultimate Recovery (EUR).
- Perform cumulative and yearly production analysis.

------------------------------------------------------------

## Input Data

Historical production dataset containing:

- Monthly Oil Production Rate
- Production Time
- Water Cut
- Gas-Oil Ratio (GOR)

------------------------------------------------------------

## Software & Libraries

Software
- Python
- Jupyter Notebook

Libraries
- NumPy
- Pandas
- Matplotlib
- SciPy (curve_fit)

------------------------------------------------------------

## Complete Workflow

### 1. Data Preparation

- Imported and organized historical production data using Pandas.
- Verified and prepared the dataset for decline curve analysis.

------------------------------------------------------------

### 2. Historical Production Analysis

Performed production trend analysis by generating:

- Oil Production Rate vs Time
- Water Cut vs Time
- Gas-Oil Ratio (GOR) vs Time

Key Observations

- Oil production continuously declined throughout the production period.
- Water cut gradually increased, indicating increasing water production.
- GOR initially increased and later declined, indicating changing production behavior during reservoir depletion.

------------------------------------------------------------

### 3. Arps Decline Curve Modeling

Implemented all three classical Arps decline models:

- Exponential Decline
- Hyperbolic Decline
- Harmonic Decline

Implemented mathematical rate-time equations for each model in Python.

------------------------------------------------------------

### 4. Decline Parameter Estimation

Estimated model parameters using SciPy's nonlinear least-squares optimization (curve_fit).

Estimated parameters:

- Initial Production Rate (qi)
- Initial Nominal Decline Rate (Di)
- Hyperbolic Decline Exponent (b)

Applied parameter bounds during optimization to obtain physically realistic solutions.

------------------------------------------------------------

### 5. Model Performance Evaluation

Evaluated all decline models using:

- Coefficient of Determination (R²)
- Root Mean Square Error (RMSE)

Results

Exponential Decline
- qi = 1413.69 BOPD
- Di = 0.058460 month⁻¹
- R² = 0.9789
- RMSE = 44.46 BOPD

Hyperbolic Decline
- qi = 1514.08 BOPD
- Di = 0.082168 month⁻¹
- b = 0.4800
- R² = 0.9869
- RMSE = 35.03 BOPD

Harmonic Decline
- qi = 1629.94 BOPD
- Di = 0.122717 month⁻¹
- R² = 0.9785
- RMSE = 44.87 BOPD

------------------------------------------------------------

### 6. Model Selection

Compared all decline models using R² and RMSE.

Outcome

- Hyperbolic Decline Model achieved the highest R² (0.9869).
- Hyperbolic Decline Model achieved the lowest RMSE (35.03 BOPD).
- Selected the Hyperbolic Decline Model for production forecasting.

------------------------------------------------------------

### 7. Production Forecasting

Forecasted future oil production using the Hyperbolic Decline Model until the economic limit of 40 BOPD.

Forecast Results

- Estimated productive life ≈ 119 months.
- Generated historical and forecast production profile.

------------------------------------------------------------

### 8. Estimated Ultimate Recovery (EUR)

Calculated cumulative oil production by combining historical production and forecast production.

Result

- Estimated Ultimate Recovery (EUR) ≈ 892,716 STB.

------------------------------------------------------------

### 9. Engineering Analysis Performed

Historical Production Analysis

- Oil Production Rate Analysis
- Water Cut Analysis
- Gas-Oil Ratio Analysis

Decline Curve Analysis

- Exponential Decline Curve Fitting
- Hyperbolic Decline Curve Fitting
- Harmonic Decline Curve Fitting

Model Evaluation

- Statistical comparison of decline models
- Comparison using qi, Di, b, R² and RMSE

Production Forecasting

- Historical + Forecast Production Profile
- Forecast until Economic Limit

Cumulative Production Analysis

- Historical Cumulative Production
- Forecast Cumulative Production
- Estimated Ultimate Recovery (EUR)

Yearly Production Analysis

- Yearly Average Oil Production Rate
- Yearly Oil Production
- Yearly Cumulative Oil Production

------------------------------------------------------------

## Engineering Concepts Applied

- Decline Curve Analysis (DCA)
- Arps Decline Models
- Production Forecasting
- Reservoir Performance Evaluation
- Nonlinear Curve Fitting
- Parameter Estimation
- Statistical Model Validation
- Model Selection using R² and RMSE
- Estimated Ultimate Recovery (EUR)
- Economic Limit Analysis
- Water Cut Analysis
- Gas-Oil Ratio Analysis
- Cumulative Production Analysis
- Yearly Production Analysis

------------------------------------------------------------

## Technical Skills Demonstrated

- Production Data Analysis
- Reservoir Engineering Calculations
- Production Forecasting
- Statistical Model Evaluation
- Scientific Computing using Python
- Data Processing using Pandas
- Numerical Optimization using SciPy
- Engineering Visualization using Matplotlib
- Technical Report Writing

------------------------------------------------------------

## Key Outcomes

- Successfully implemented Arps Decline Curve Analysis using Python.
- Estimated decline parameters (qi, Di and b) through nonlinear regression.
- Compared Exponential, Hyperbolic and Harmonic decline models using statistical performance metrics.
- Identified the Hyperbolic Decline Model as the optimum forecasting model (R² = 0.9869, RMSE = 35.03 BOPD).
- Forecasted oil production until the economic limit of 40 BOPD.
- Estimated an Estimated Ultimate Recovery (EUR) of approximately 892,716 STB.
- Generated professional engineering plots for production history, decline model fitting, production forecasting, cumulative production, water cut, GOR, and yearly production analysis.
- Prepared a complete technical report including Problem Statement, Theory, Methodology, Results & Discussion, Conclusion, and References.

------------------------------------------------------------

## Confidentiality Note

This project summary is intended only for resume preparation, interview discussion, and documentation of technical work performed during the internship.

The project description focuses on the engineering methodology, Python implementation, analytical workflow, and technical skills acquired during the internship. It does not contain any confidential ONGC information or proprietary reservoir data.

No raw production data, reservoir models, well identifiers, field names, asset-specific information, internal reports, or proprietary software outputs are included.

Any public sharing of this project should continue to exclude the original datasets and confidential information provided during the internship, in accordance with ONGC confidentiality requirements.
