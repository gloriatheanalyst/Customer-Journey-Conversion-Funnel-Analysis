
# Customer-Journey-Conversion-Funnel-Analysis
 A Data Analytics Project Using Python & Power BI

## 1. Project Overview

This project analyzes an e-commerce customer journey dataset to understand user behavior, identify drop-off points, and uncover factors affecting conversion rates. A full funnel analysis was conducted, alongside exploratory data analysis (EDA), demographic behavior analysis, and time-on-page insights.

The project includes:

- Python notebook with cleaning + EDA + funnel modeling

- Power BI dashboard visualizing user flow and conversion drivers

- Recommendations to improve conversion and reduce cart abandonment

## 2. Problem Statement

E-commerce websites experience significant drop-offs throughout the customer journey. The goal of this project is to:

- Understand how users move through the product funnel (Home → Product Page → Cart → Checkout → Confirmation → Purchase).
- Identify where and why the largest drop-offs occur.
- Analyze which user attributes (Device Type, Country, Referral Source) influence purchase likelihood.
- Quantify conversion rates at each stage.
- Provide actionable recommendations to improve the conversion funnel.

## 3. Project Objectives

1. Clean and prepare the dataset for analysis.
2. Perform exploratory data analysis to understand user behavior.
3. Build a full conversion funnel and measure drop-offs.
4. Analyze conversion rates by device, referral, and country.
5. Identify user behavior patterns such as time spent and cart usage.
6. Develop meaningful insights and recommendations.
7. Build a Power BI dashboard for visualization.

## 4. Dataset Description
Source: https://www.kaggle.com/datasets/sufya6/e-commerce-customer-journey-click-to-conversion/data

The dataset consists of user browsing sessions on an e-commerce platform.

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
#### Python (Jupyter Notebook)
Used for:
- Data cleaning
- Preprocessing
- EDA
- Funnel analysis
- Visualizations
#### Libraries
- pandas
- numpy
- matplotlib
- seaborn
#### Power BI
- Used to create:
- Funnel visualization
- Conversion dashboards
- Country and device insights
- KPI cards

### 6. Data Cleaning Summary
The following steps were applied:
- Converted Timestamp column to datetime
- Removed duplicate rows
- Removed negative values in time and items
- Sorted by SessionID + Timestamp
-  Checked missing values (none found)
-  Standardized categories
- Exported cleaned dataset

A fully cleaned dataset was saved as: **[customer_journey_cleaned_dataset.csv](https://github.com/gloriatheanalyst/Customer-Journey-Conversion-Funnel-Analysis/blob/main/customer_journey_cleaned_dataset.csv)**

### 7. Exploratory Data Analysis (EDA)
Key EDA Steps
- Distribution of time spent on pages
- Items in cart distribution
- Boxplots comparing features vs purchase outcomes
- Unique user and session counts
- Category distributions for Device, Country, Referral, PageType
- Analysis of browsing patterns

#### Core Findings

1. Time on page does not strongly correlate with purchase.

2. Desktop users had slightly higher conversion rates than mobile/tablet.

3. Google search drove the highest volume of sessions but not the highest conversions.

4. Some countries had significantly better cart-to-purchase performance.

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

### 12. Next Steps

- Build a predictive model for purchase likelihood
- Use clustering to identify user personas
- Add A/B testing insights
- Integrate more behavioral features (scroll depth, clicks, bounce rate)
- Build real-time funnel dashboards

### 13. Conclusion

This project successfully analyzed user behavior across an e-commerce customer journey. By combining Python-based EDA with Power BI funnel visualization, we identified key drop-off points, behavioral insights, and actionable recommendations.
These insights can greatly support strategic decisions in UX improvement, marketing targeting, and funnel optimization.
