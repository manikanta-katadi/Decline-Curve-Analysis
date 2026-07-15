# Decline Curve Analysis (DCA) of an Oil Well

## Project Overview

This project demonstrates the application of **Arps Decline Curve Analysis (DCA)** to historical oil well production data for evaluating production performance, comparing decline models, forecasting future production, estimating productive well life, and calculating the **Estimated Ultimate Recovery (EUR)**. The complete workflow was implemented in **Python** using **Jupyter Notebook**.

> **Note:** The original production dataset is **not included** in this repository due to confidentiality requirements.

---

## Objectives

- Analyze historical oil well production data.
- Implement Arps Exponential, Hyperbolic, and Harmonic decline models.
- Estimate decline parameters using nonlinear regression.
- Compare decline models using statistical performance metrics.
- Forecast future oil production until the economic limit.
- Estimate Estimated Ultimate Recovery (EUR).
- Visualize historical, forecast, cumulative, and yearly production trends.

---

## Input Data

The analysis is based on historical monthly production data containing:

- Production Time
- Oil Production Rate
- Water Cut
- Gas-Oil Ratio (GOR)

> **Note:** The original production dataset is proprietary and has been excluded from this repository.

---

## Technologies Used

### Programming Language

- Python

### Development Environment

- Jupyter Notebook

### Python Libraries

- NumPy
- Pandas
- Matplotlib
- SciPy (`scipy.optimize.curve_fit`)

---

## Methodology

### 1. Historical Production Analysis

- Imported and organized production data using Pandas.
- Evaluated production trends through:
  - Oil Production Rate vs Time
  - Water Cut vs Time
  - Gas-Oil Ratio (GOR) vs Time

### 2. Decline Curve Modeling

Implemented the three classical Arps decline models:

- Exponential Decline
- Hyperbolic Decline
- Harmonic Decline

### 3. Parameter Estimation

Estimated decline parameters using nonlinear least-squares regression (`curve_fit`).

Estimated:

- Initial Production Rate (qi)
- Initial Nominal Decline Rate (Di)
- Hyperbolic Decline Exponent (b)

Applied parameter bounds to ensure physically realistic solutions.

### 4. Model Evaluation

Compared the decline models using:

- Coefficient of Determination (R²)
- Root Mean Square Error (RMSE)

Selected the best-fit model based on statistical performance.

### 5. Production Forecasting

Forecasted future oil production until the selected economic limit.

### 6. Reserve Estimation

Calculated:

- Historical Cumulative Production
- Forecast Cumulative Production
- Estimated Ultimate Recovery (EUR)

### 7. Yearly Production Analysis

Generated:

- Yearly Average Oil Production Rate
- Yearly Oil Production
- Yearly Cumulative Oil Production

---

## Engineering Analysis Performed

### Historical Production Analysis

- Oil Production Rate Analysis
- Water Cut Analysis
- Gas-Oil Ratio Analysis

### Decline Curve Analysis

- Exponential Decline Curve Fit
- Hyperbolic Decline Curve Fit
- Harmonic Decline Curve Fit

### Model Evaluation

Compared decline models using:

- Initial Production Rate (qi)
- Initial Decline Rate (Di)
- Hyperbolic Decline Exponent (b)
- Coefficient of Determination (R²)
- Root Mean Square Error (RMSE)

### Production Forecasting

Generated:

- Historical + Forecast Production Profile
- Production Forecast to Economic Limit

### Reserve Estimation

Calculated:

- Historical Cumulative Production
- Forecast Cumulative Production
- Estimated Ultimate Recovery (EUR)

### Yearly Production Analysis

Generated:

- Yearly Average Oil Production Rate
- Yearly Oil Production
- Yearly Cumulative Oil Production

---

## Technical Skills Demonstrated

- Decline Curve Analysis (DCA)
- Reservoir Performance Evaluation
- Production Forecasting
- Estimated Ultimate Recovery (EUR)
- Nonlinear Curve Fitting
- Statistical Model Evaluation
- Parameter Estimation
- Data Analysis using Pandas
- Scientific Computing using NumPy
- Numerical Optimization using SciPy
- Engineering Visualization using Matplotlib
- Technical Report Writing

---

## Repository Structure

```text
Decline-Curve-Analysis/
│
├── DCA.ipynb
└── README.md
```

---

## Confidentiality

This repository demonstrates the engineering methodology, Python implementation, and analytical workflow of a Decline Curve Analysis project.

To comply with confidentiality requirements:

- The original production dataset is **not included**.
- No proprietary reservoir data, field names, well identifiers, asset-specific information, or internal company documents are shared.
- Notebook outputs containing confidential production data have been removed before publication.

This repository is intended solely to demonstrate the implementation of Decline Curve Analysis using Python for educational and portfolio purposes.
