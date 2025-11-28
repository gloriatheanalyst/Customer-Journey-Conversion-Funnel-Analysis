📦 customer-journey-analysis/
│
├── 📁 data/
│   ├── raw_dataset.csv
│   └── customer_journey_cleaned_dataset.csv
│
├── 📁 notebook/
│   └── analysis.ipynb
│
├── 📁 powerbi/
│   └── dashboard.pbix
│
├── README.md
└── requirements.txt


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

The dataset consists of user browsing sessions on an e-commerce platform.

**Key columns include:**
SessionID — Unique session identifier

UserID — Unique user identifier

Timestamp — Event time

PageType — Page visited (home, product_page, cart, checkout, confirmation)

DeviceType — Mobile, Desktop, Tablet

Country — User's country

ReferralSource — Traffic origin (Google, Social, Email, etc.)

TimeOnPage_seconds — Time spent on each page

ItemsInCart — Number of items added

Purchased — 1 if purchase occurred, else 0

## 5. Tools & Technologies
#### Python (Jupyter Notebook)
Used for:
Data cleaning
Preprocessing
EDA
Funnel analysis
Visualizations

#### Libraries
pandas
numpy
matplotlib
seaborn

#### Power BI
Used to create:
Funnel visualization
Conversion dashboards
Country and device insights
KPI cards
