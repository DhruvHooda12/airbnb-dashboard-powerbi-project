# Airbnb Global Operations Dashboard

A Power BI dashboard analyzing **279,712 Airbnb listings across 10 global cities**, covering platform growth from 2008–2020, market share by city, pricing by room type, and host/guest satisfaction ratings.

---

## 🏗️ Repo structure

```
├── data/
│   ├── Listings.csv                     # 279,712 listings — host, pricing, ratings, location
│   ├── Listings_data_dictionary.csv     # Field definitions for Listings.csv
│   ├── Reviews.csv                      # 5,373,144 reviews — listing_id, review_id, date, reviewer_id
│   └── Reviews_data_dictionary.csv      # Field definitions for Reviews.csv
├── powerbi/
│   ├── airbnb_powerbi.pbix              # Power BI report (3 pages)
│   └── airbnb_dashboard_pdf.pdf         # Static export of all pages
└── README.md
```

## ⚙️ Tech Stack

Power BI (data modeling, DAX measures, visuals)

---

## 📊 Dataset

| File | Rows | Description |
|---|---|---|
| `Listings.csv` | 279,712 | Listing name, host details, location, property/room type, price, minimum/maximum nights, and 7 review-score sub-metrics |
| `Reviews.csv` | 5,373,144 | Every review tied to a listing, with date and reviewer ID — used to build the platform growth timeline |

**Cities covered:** Paris, New York, Sydney, Rio de Janeiro, Istanbul, Rome, Bangkok, Cape Town, Mexico City, Hong Kong.

**Scope at a glance:** 279,712 listings · 182,024 hosts · 144 property types · 5.37M reviews.

---

## 📈 Dashboard Pages

### 1. Global Operations Overview
KPI cards (listings, cities, hosts, property types, reviews) plus a listings-over-time chart by room type (Private room / Shared Room / Entire place / Hotel Room), annotated against Airbnb's business lifecycle stages — Introduction → Growth → Maturity → Decline → Reinvention → COVID-19.

**Key insight:** 2015 was the peak year for new listings. Growth cooled in 2016–17 due to tightening local regulations, even as Airbnb turned profitable in H2 2016. A second growth phase from 2018 was cut short by COVID-19 in 2020.

### 2. Market Share by City
Listings by city, split by Superhost vs. non-Superhost, next to average price by room type.

**Key insight:** Paris, NYC, and Sydney together account for ~48% of total listings and reviews. Paris leads on both — plausibly because Paris hotel rooms average ~2x the price of an equivalent Airbnb ($800 vs. $462–$673 depending on room type).

### 3. Ratings Breakdown
Average overall rating by city, drillable into the 6 sub-metrics (accuracy, cleanliness, communication, location, value, and check-in — via the toggle between Overall Rating and Detailed Rating).

**Key insight:** Mexico City and Rio de Janeiro rate highest overall; Hong Kong and Istanbul rate lowest. Across every city, **cleanliness** and **value for money** are the two weakest-scoring sub-metrics.

---

## 🚀 Key Takeaways

The interesting part of this project isn't the KPI cards — it's the layered story a single dataset can tell once you connect listings to reviews to macro context: pricing pressure, regulation, and satisfaction all move together in ways that pure listing counts hide. That's the difference between a "here are some numbers" dashboard and a "here's what's actually happening" one.

---

## 👤 Author

**Chirag Gulati** — Founder, [Demox Media](https://demoxmedia.com)
