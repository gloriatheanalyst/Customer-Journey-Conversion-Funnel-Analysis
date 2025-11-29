
# Customer-Journey-Conversion-Funnel-Analysis
 A Data Analytics Project Using Python & Power BI

## 1. Project Overview

This project maps the full e-commerce customer journey — from homepage visits to purchases — to uncover drop-off points, device/channel differences, and behavioral patterns that impact conversion. By combining Python-based exploratory data analysis (EDA) with interactive Power BI dashboards, it delivers actionable insights to reduce cart abandonment and improve conversion.

Key Deliverables:

- Cleaned dataset **[customer_journey_cleaned_dataset.csv](https://github.com/gloriatheanalyst/Customer-Journey-Conversion-Funnel-Analysis/blob/main/customer_journey_cleaned_dataset.csv)**
- Python notebook (data cleaning, EDA, funnel modeling)
- Power BI dashboard (conversion funnel, device, country, referral insights)
- Recommendations report

## 2. Problem Statement

E-commerce websites experience significant drop-offs throughout the customer journey. Understanding these drop-offs is critical for improving user experience, reducing cart abandonment, and increasing revenue.

The project aims to:
- Map the funnel (Home → Product → Cart → Checkout → Confirmation → Purchase).
- Identify where the largest drop-offs occur.
- Analyze how device type, country, and referral source influence purchase likelihood.
- Quantify conversion rates at each stage.
- Provide actionable recommendations to optimize the funnel.

## 3. Objectives

1. Clean and prepare the dataset for analysis.
2. Perform exploratory data analysis to understand user behavior.
3. Build a full conversion funnel and measure drop-offs.
4. Analyze conversion rates by device, referral, and country.
5. Identify user behavior patterns such as time spent and cart usage.
6. Develop insights and recommendations.
7. Build an interactive Power BI dashboard for visualization.

## 4. Dataset Description
Source: https://www.kaggle.com/datasets/sufya6/e-commerce-customer-journey-click-to-conversion/data

**Key columns include:**
- SessionID — Unique session identifier
- UserID — Unique user identifier
- Timestamp — Event time
- PageType — Page visited (home, product_page, cart, checkout, confirmation)
- DeviceType — Mobile, Desktop, Tablet
- Country — User's country
- ReferralSource — Traffic origin (Google, Social, Email, etc.)
- TimeOnPage_seconds — Time spent on each page
- ItemsInCart — Number of items added
- Purchased — 1 if purchase occurred, else 0

## 5. Tools & Technologies
#### Python (Jupyter Notebook):Data cleaning, Preprocessing, EDA, Funnel analysis, Visualizations
- Libraries: pandas, numpy, matplotlib, seaborn

#### Power BI: Funnel visualization, conversion dashboards, KPI cards, country/device insights, slicers, drill-through

### 6. Data Cleaning Summary
The following steps were applied:
- Converted Timestamp column to datetime
- Checked for duplicate rows (none found)
- Checked and Removed negative values in time and items if any
- Sorted by SessionID + Timestamp
- Checked missing values (none found)
- Standardized categories
- Exported cleaned dataset

### 7. Exploratory Data Analysis (EDA)
Key EDA Steps
- Distribution of time spent on pages
- Items in cart distribution
- Boxplots comparing features vs purchase outcomes
- Unique user and session counts
- Category distributions (Device, Country, Referral, PageType)
- Analysis of browsing patterns

#### Core Findings

1. Time on page does not strongly correlate with purchase.

2. Desktop (20.35%) users had slightly higher conversion rates than mobile (*20.17%*) and tablet(*20.08%*)

3. Google search(*21.64%*) drove the highest volume of sessions but not the highest conversions.
   	ReferralSource	Sessions	Conversions	ConversionRate
0	Direct	1226	243	19.82%
1	Email	1251	251	20.06%
2	Google	1280	277	21.64%
3	Social Media	1243	239	19.23%

5. Some countries had significantly better cart-to-purchase performance.

### 8. Conversion Funnel Analysis

#### Stages analyzed:
- Home
- Product Page
- Cart
- Checkout
- Confirmation
- Purchase

#### Metrics computed:
- Sessions at each stage
- % of total traffic
- Conversion rate from previous step
- Drop-off numbers and drop-off rate
- Cart-to-purchase and checkout-to-purchase KPIs

#### Key Findings:
- Largest drop-off occurred between Product Page → Cart
- Checkout completion rate was relatively strong
- A small percentage of sessions reached the final confirmation stage
- Device and country impacted funnel progression

### 9. Insights & Interpretations
🔹 Insight 1 — Time Spent is Not Predictive

Purchasers and non-purchasers showed almost identical time-on-page averages.
Longer browsing is not a sign of higher likelihood to convert.

🔹 Insight 2 — Device Matters

Desktop users converted the most, suggesting mobile experience may need optimization.

🔹 Insight 3 — Referral Source Quality Varies

Google brings the most sessions, but Email and Direct traffic showed better conversion ratios.

🔹 Insight 4 — Major Drop-Off at Add-to-Cart Stage

This suggests product pages may need:

- clearer pricing
- more compelling CTAs
- faster loading

🔹 Insight 5 — Country Differences

Some countries have significantly higher funnel completion, indicating potential targeting opportunities.

### 10. Power BI Dashboard Overview

The Power BI report includes:

- Overview KPIs (Total Sessions, Purchases, Conversion Rate)
- Device conversion comparison
- Country performance charts
- Referral source conversion bar chart
- Full customer journey funnel visualization
- Time-on-page comparison insights

This dashboard allows stakeholders to monitor conversion performance at a glance.
![Customer Journey Conversion Analysis Dashboard](https://github.com/gloriatheanalyst/Customer-Journey-Conversion-Funnel-Analysis/blob/main/Customer%20Journey%20Conversion%20Analysis%20Power%20Bi.png)

### 11. Recommendations
✔ Optimize Mobile UI/UX

Improve button size, layout, loading speed.

✔ Improve Product Page Clarity

Reduce information overload, clearer pricing, stronger call-to-action.

✔ Strengthen Cart Experience

Show shipping cost estimates earlier, simplify cart layout.

✔ Enhance High-Intent Traffic Sources

Focus on Email, Direct, and Search retargeting.

✔ Reduce Friction in Checkout

Auto-fill fields, reduce form steps, enable guest checkout.

✔ Personalize User Experience

Recommend products based on browsing history.

### 12. Ethical Considerations

User Privacy:
Dataset contains anonymized user IDs; no personal information is included.

Bias & Fairness:
Differences across countries or devices must not be interpreted as user deficiencies; instead, system design may contribute.

### 13. Next Steps

- Build a predictive model for purchase likelihood
- Use clustering to identify user personas
- Add A/B testing insights
- Integrate more behavioral features (scroll depth, clicks, bounce rate)
- Build real-time funnel dashboards

### 14. Limitations

- Dataset is simulated (not real-world user data)
- No product-level details (price, category)
- No clickstream depth (scrolls, button clicks)
- No information on marketing campaigns
- Funnel stages are assumed based on PageType sequence

These limitations affect how broadly the findings can be generalized.

### 15. Conclusion

This project successfully analyzed user behavior across an e-commerce customer journey. By combining Python-based EDA with Power BI funnel visualization, we identified key drop-off points, behavioral insights, and actionable recommendations.
These insights can greatly support strategic decisions in UX improvement, marketing targeting, and funnel optimization.
