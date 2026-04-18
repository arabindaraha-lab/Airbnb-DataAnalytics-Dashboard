# Airbnb Listings, Host & Business Analysis  

## Project Overview  
This project analyzes Airbnb business performance using interactive dashboards. The focus areas include:  
- Revenue trends  
- Pricing strategies  
- Host distribution  
- Demand patterns  

The goal is to identify growth drivers, uncover underperforming areas, and provide data-driven recommendations to optimize pricing and improve listing performance.

---

## 🖼️ Cover Image  
![Cover Image](CoverPhoto.png)

---

## 📂 File Details  
- **Filename:** AirbnbCleanData.csv  
- **Total Records:** 50,000  
- **Primary Keys:** `id`, `host_id`, `city`, `room_type`  
- **Source Data:** AirbnbRawData.csv  
- **Tools Used:** Excel, Looker Studio  

---

## 📊 Data Dictionary  

| Column Name | Description | Data Type |
|------------|------------|----------|
| id | Unique listing ID | Integer |
| name | Listing name | String |
| host_id | Unique host ID | Integer |
| host_name | Host name | String |
| neighbourhood_group | Area group | String |
| neighbourhood | Area name | String |
| latitude | Location latitude | Float |
| longitude | Location longitude | Float |
| room_type | Property type | String |
| price | Daily price | Integer |
| minimum_nights | Minimum stay | Integer |
| number_of_reviews | Total reviews | Integer |
| last_review | Last review date | Date |
| reviews_per_month | Avg monthly reviews | Float |
| calculated_host_listings_count | Listings per host | Integer |
| availability_365 | Availability days | Integer |
| number_of_reviews_ltm | Reviews in last 12 months | Integer |
| license | License number | String |
| city | Listing city | String |
| scrape_date | Data collection date | Date |

---

## 🧠 Business Dashboard  

![Business Dashboard](business_dashboard.png)

### 🔑 Key Insights  

1. **📈 Monthly Revenue Trend**  
   - Revenue peaks during Nov–Mar (~₹9.98B)  
   - Drops significantly in Apr–May (~₹1.1B)  
   - Strong seasonality driven by travel trends  

2. **👤 Revenue by Host Type**  
   - Individual hosts dominate (~₹13.32B)  
   - Commercial hosts (~₹2.74B)  
   - Semi-professional hosts contribute minimally  

3. **📍 Top Locations by Reviews**  
   - Centro Storico (Rome) leads  
   - Followed by Westminster (London), Buttes-Montmartre (Paris)  
   - Indicates high-demand tourist hotspots  

4. **💰 Pricing Insights**  
   - Entire homes are priced highest  
   - London & Amsterdam = premium pricing  
   - Bangkok = lowest pricing  
   - Pricing strongly linked to demand  

5. **🏡 Room Type Performance**  
   - Entire homes: 37K listings, ₹16B revenue  
   - Private rooms: moderate contribution  
   - Hotel/shared rooms: minimal impact  
   - Platform dominated by entire-home rentals  

---

### 🚀 Business Recommendations  

- **Reduce Seasonality Risk**  
  - Introduce off-season discounts  

- **Diversify Host Base**  
  - Incentivize commercial hosts  

- **Optimize Pricing**  
  - Implement AI-based dynamic pricing  

- **Focus on High-demand Locations**  
  - Expand supply in Rome, London, Paris  

---

## 📊 Analytical Dashboard  

![Analytical Dashboard](analytical_dashboard.png)

### 🔑 Key Insights  

1. **📊 Business Scale**  
   - 50,000 listings, 29,251 hosts  
   - ₹17.03B revenue, 1.6M reviews  
   - Avg stay: 21 nights  
   - Avg availability: 158 days (concern)  

2. **📉 Demand Distribution**  
   - Moderate: 27.6%  
   - Low demand: 36%  
   - Majority listings underperforming  

3. **🔄 Demand vs Reviews**  
   - Low-demand listings → high reviews  
   - High-demand listings → fewer reviews  
   - Indicates older vs newer listing behavior  

4. **🌍 Geographic Demand**  
   - Strong presence in Europe (UK, France, Italy)  
   - Limited presence in Asia & Australia  

5. **📉 Price vs Reviews**  
   - Strong inverse relationship  
   - High price → lower engagement  
   - Budget listings perform better  

6. **📈 Growth Trends**  
   - Major spike in 2025 (~25.7K listings)  
   - Indicates rapid expansion  

---

### 🚀 Analytical Recommendations  

- **Improve Low-demand Listings**  
  - Optimize pricing & quality  

- **Review Strategy**  
  - Encourage more user reviews  

- **Control Supply Growth**  
  - Avoid oversaturation in major cities  

- **Personalization**  
  - Recommend listings based on budget & purpose  

---

## 🎯 Conclusion  
Airbnb shows strong growth driven by entire-home listings and European markets. However, challenges like seasonality, price sensitivity, and underperforming listings remain. Strategic pricing, demand optimization, and balanced expansion are key to long-term success.

---

## 🧹 Data Cleaning Notes  

| Column | Action |
|-------|-------|
| neighbourhood_group | Removed (missing values) |
| license | Removed (missing values) |
| scrape_date | Removed (duplicate values) |
| price_aprox | Created (fill missing prices) |
| price_in_inr | Created (currency conversion) |
| minimum_revenue | Created (revenue calculation) |
| last_review | Filled missing + extracted year/month |
| month_range | Created (season segmentation) |
| reviews_per_month | Filled with average |
| host_type | Created (host segmentation) |
| listing_demand | Created (Low/Medium/High classification) |

---

## 🛠️ Tools & Technologies  
- Microsoft Excel  
- Google Sheets  
- Looker Studio  

---

## 📌 Focus Outcomes  
- Optimize pricing strategy  
- Reduce low-performing listings  
- Improve demand forecasting  
- Support strategic business decisions  
