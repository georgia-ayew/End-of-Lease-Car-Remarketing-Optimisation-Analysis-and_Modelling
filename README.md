# End-of-Lease-EV-Remarketing-Optimisation-using-Machine-Learning
=========================

Built a predictive model to estimate UK vehicle resale value and optimise end-of-lease disposal decisions using vehicle age, mileage, and specification data.

# Executive Summary

## Model Performance

**Model Used:** 

- Random Forest Regression (trained on historical UK Vehicle Sale Data 2023-2017)

**Target:**

- Vehicle Price (log transformed for modelling)

**Accuracy Metrics** 

- **R²**: 0.9 (90% of price variability explained)
- **RMSE**: £1,427 avergae deviation from predicted price 
- **MAE**: £846 average error per vehicle

## Key Insights from Residuals

**Residuals** = Actual Price – Predicted Price

**Undervalued Vehicles (sell for more than predicted):**

- Example: Low mileage, family-friendly, or premium models

- Average positive residual: up to £13,000

- Action: Highlight these vehicles in listings, consider pricing slightly higher to maximize revenue.

**Overvalued Vehicles (sell for less than predicted):**

- Example: Older, high-mileage, or less popular models

- Average negative residual: up to £4,500

- Action: Avoid overpricing these vehicles; consider promotions or faster turnover.

## Segment-Level Learnings

- Vehicles grouped by Emission Class, Age Band, and Engine size reveal patterns:

- Euro 6, low mileage, family cars → consistently undervalued → pricing opportunity

- Older, smaller engines → often overvalued → adjust acquisition/pricing strategy

- Using binned engine categories improves clarity of segment-level insights.

## Recommendations

**Pricing Strategy:**

- Increase prices on undervalued segments by £500–£1,500 depending on residual magnitude.

- Reduce prices on overvalued segments to accelerate sales and reduce holding costs.

**Inventory Planning:**

- Prioritize acquisition of vehicles that historically outperform predictions (low mileage, family-friendly, Euro 6).

- Avoid over-investing in segments that tend to underperform.

**Marketing:**

- Promote undervalued vehicles prominently to maximize ROI.

- Highlight key features undervalued by the model (engine size, Euro class, mileage).

**Model Monitoring & Refinement:**

- Re-train periodically with new sales data.

- Consider segment-specific models for rare/premium vehicles to reduce extreme residuals.