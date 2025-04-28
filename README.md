# Dynamic Airline Ticket Pricing Model

## Project Overview
This project builds a **dynamic pricing model** for airline tickets. The goal is to predict optimal ticket prices based on **real-time demand drivers** like load factor, days to departure, and competitor prices.

## Problem Statement
Airlines must adjust prices dynamically to optimize revenue while staying competitive. This project demonstrates how **machine learning** can support this process.

## Data
- **Synthetic dataset** generated with features:
  - Days to Departure
  - Load Factor (% of seats sold)
  - Competitor Prices
  - Day of the Week
  - Event/Holiday flag
- Dataset simulates **5,000 rows** of booking scenarios.

## Methodology
1. **Feature Engineering**:
   - Created interaction terms (e.g., Days to Departure × Load Factor).
   - Applied log and polynomial transformations.
   
2. **Modeling Techniques**:
   - Linear Regression
   - Random Forest Regressor
   - XGBoost Regressor

3. **Evaluation Metrics**:
   - RMSE (Root Mean Squared Error)
   - R-squared (explained variance)

## Deployment
- **FastAPI app** serves the trained model for real-time predictions.
- Example API endpoint: `/predict`

## Dashboard (Optional)
- Power BI/Tableau dashboard showcasing:
  - Booking trends
  - Predicted vs. actual prices
  - Model insights

## Business Impact
Dynamic pricing based on demand and competitor fares can:
- Increase revenue per available seat mile (RASM).
- Optimize load factor by adjusting fares in real-time.

## Future Work
- Integrate **real competitor data** (via scraping or APIs).
- Expand to include **route-specific patterns**.
- Explore **reinforcement learning** for continuous price optimization.

## How to Run
1. Clone this repo.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
