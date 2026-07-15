# Decline Curve Analysis (DCA) of an Oil Well

## Project Overview

This project demonstrates the application of **Arps Decline Curve Analysis (DCA)** to historical oil well production data for evaluating production performance, comparing decline models, forecasting future production, estimating the productive life of the well, and calculating the **Estimated Ultimate Recovery (EUR)**. The complete workflow was implemented in **Python** using **Jupyter Notebook** as part of my Summer Internship at **ONGC – Institute of Reservoir Studies (IRS), Ahmedabad**.

> **Note:** The original production dataset is **not included** in this repository due to confidentiality requirements.

---

## Objectives

- Analyze historical oil well production data.
- Implement Arps Exponential, Hyperbolic, and Harmonic decline models.
- Estimate decline parameters using nonlinear regression.
- Compare model performance using statistical evaluation metrics.
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

> **Note:** The original dataset is proprietary and has been excluded from this repository.

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
- Analyzed production behavior through:
  - Oil Production Rate vs Time
  - Water Cut vs Time
  - Gas-Oil Ratio (GOR) vs Time

### 2. Decline Curve Modeling

Implemented the three classical Arps decline models:

- Exponential Decline
- Hyperbolic Decline
- Harmonic Decline

### 3. Parameter Estimation

Estimated decline parameters using SciPy's nonlinear least-squares optimization (`curve_fit`).

Estimated:

- Initial Production Rate (qi)
- Initial Nominal Decline Rate (Di)
- Hyperbolic Decline Exponent (b)

Applied parameter bounds to ensure physically realistic solutions.

### 4. Model Evaluation

Compared all decline models using:

- Coefficient of Determination (R²)
- Root Mean Square Error (RMSE)

### 5. Production Forecasting

Selected the best-fit model and forecasted oil production until the economic limit of **40 BOPD**.

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

## Results

| Model | qi (BOPD) | Di (/month) | b | R² | RMSE (BOPD) |
|------|----------:|------------:|---:|------:|------------:|
| Exponential | 1413.69 | 0.058460 | 0.0000 | 0.9789 | 44.46 |
| Hyperbolic | 1514.08 | 0.082168 | 0.4800 | **0.9869** | **35.03** |
| Harmonic | 1629.94 | 0.122717 | 1.0000 | 0.9785 | 44.87 |

### Key Findings

- The **Hyperbolic Decline Model** provided the best agreement with the historical production data.
- Forecasted production until an economic limit of **40 BOPD**.
- Estimated productive life of approximately **119 months**.
- Estimated Ultimate Recovery (EUR) of approximately **892,716 STB**.

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

### Model Comparison

Compared decline models using:

- Initial Production Rate (qi)
- Initial Decline Rate (Di)
- Hyperbolic Exponent (b)
- Coefficient of Determination (R²)
- Root Mean Square Error (RMSE)

### Production Forecasting

Generated:

- Historical + Forecast Oil Production
- Forecast until Economic Limit

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

This repository demonstrates the engineering methodology, Python implementation, and analytical workflow developed during an industrial internship.

To comply with confidentiality requirements:

- The original production dataset is **not included**.
- No proprietary reservoir data, field names, well identifiers, asset-specific information, or internal company documents are shared.
- Any notebook outputs containing confidential production data should be removed before publication.

This repository is intended solely to showcase the implementation of Decline Curve Analysis using Python for educational and portfolio purposes.
