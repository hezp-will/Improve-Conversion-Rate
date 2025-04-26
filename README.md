# Conversion Rate Analysis and Improvement

## Project Overview
This project explores and predicts conversion rates on an e‑commerce site to guide marketing and product strategies. We profile users, quantify relationships between user characteristics and conversion, build predictive models, and derive actionable recommendations to boost conversions.

## Data Description
- **country**: User origin (based on IP)
- **age**: Self‑reported at sign‑up
- **new_user**: 1 if first visit, 0 for returning users
- **source**: Acquisition channel (`Ads`, `Seo`, `Direct`)
- **total_pages_visited**: Session engagement proxy
- **converted**: Label (1 = purchase, 0 = no purchase)

Data is split into training and test sets (80/20) for modeling.

## Key Questions
1. **User Profile**: Who visits and what are their attributes?
2. **Conversion Associations**: How do demographics, channel, and behavior relate to conversion?
3. **Indicators**: Which features signal high vs. low conversion rates?
4. **High‑Convert Segment**: What common traits define top converters?
5. **Target Audience**: Which group should marketing campaigns prioritize?
6. **Prediction**: How can we forecast conversion probability?
7. **Next Steps**: After predicting, how do we act to improve conversion?

## Exploratory Data Analysis
- Summarize distributions (counts, means) by segment
- Visualize:
  - Conversion rate by channel and user type
  - Age distribution vs. conversion
  - Engagement (pages visited) vs. conversion

## Modeling Approach
- **Train/test split** using `train_test_split`
- **Baseline**: Logistic Regression for interpretability
- **Advanced**: Random Forest to capture non‑linear effects

## Model Evaluation
- **Metrics**:
  - ROC AUC for ranking quality
  - Precision, recall, F1 for segment-level insights

## Recommendations and Next Steps
- **Young Users**: Amplify marketing on channels popular with younger demographics to leverage their strong conversion rates.
- **Germany Expansion**: Prioritize acquisition of German users—despite low traffic, their high conversion presents substantial growth potential.
- **Loyal Users**: Launch targeted email campaigns with special offers for returning customers to boost repeat conversions.
- **Older Demographics (≥30)**: Conduct a UI/UX audit and form a dedicated team to improve conversion rates for users aged 30 and above.
- **China Localization**: Urgently address Chinese-site issues (translation, cultural fit, payment flow) to capitalize on a large user base.
