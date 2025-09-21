
# Airbnb Listings EDA Project: New York 2024

## Project Overview

This project performs Exploratory Data Analysis (EDA) on New York Airbnb data (2024) to uncover trends and patterns in rental listings. We use libraries like **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn** for data cleaning, visualization, and analysis.

---

## Objective

- Analyze room types, prices, and availability across different neighborhoods.  
- Understand host behavior and listing patterns.  
- Detect potential outliers in prices.  
- Provide recommendations for both guests and hosts based on insights derived.

---

## Dataset

- Includes **20,765 entries** and **22 features**, such as:  
  - `id`: Unique identifier for each listing  
  - `name`: Title of the Airbnb listing  
  - `host_name`: Name of the host  
  - `neighborhood_group`: Borough or neighborhood group  
  - `latitude`, `longitude`: Geolocation of listings  
  - `price`: Nightly rental price  
  - `room_type`: Type of accommodation (e.g., entire home, private room)  
  - `reviews_per_month`: Average monthly reviews  
  - `availability_365`: Number of days of availability in a year  

---

## Steps & Workflow

1. **Data Cleaning**  
   - Handle missing data (e.g. in `price`, `neighborhood`, `beds`).  
   - Convert `last_review` to a datetime format.  
   - Remove or cap extreme price outliers (e.g. prices > \$1,000) to avoid skewing visualizations.

2. **Exploratory Data Analysis**  
   - **Room Type Distribution**: Bar plots to show counts of each room type; identify most common types.  
   - **Neighborhood Insights**: Analyze price variation by boroughs; compare averages.  
   - **Availability Trends**: Look at relationships among price, availability, number of reviews, and beds (via heatmaps, pair plots).  
   - **Price Distribution & Outliers**: Histograms, boxplots to explore distribution and highlight extreme values.  
   - **Host Behavior**: Study hosts with multiple listings.  
   - **Review Behavior**: Relationships among reviews, price, availability using pair plots.

3. **Data Visualization**  
   - Pairplots for correlation among numerical features.  
   - Heatmaps for feature correlation.  
   - Histograms & Boxplots for price distributions and outliers.  
   - Bar charts for categorical variables (room_type, neighborhood_group).

---

## Key Findings & Insights

- **Price Trends**:  
  Manhattan has the most expensive listings; Brooklyn follows. Entire homes/apartments are significantly more expensive than private/shared rooms.

- **Room Type Distribution**:  
  Most listings are for entire homes/apartments, but private rooms are more budget‑friendly.

- **Outliers**:  
  Some listings priced extremely high (e.g. \$10,000+)—these may distort analysis if not dealt with.

- **Availability Patterns**:  
  Listings with high availability often have more reviews and tend to have lower prices, possibly due

  ## Recommendations

### For Guests

- **Choose listings with high availability and strong reviews** — these tend to be more reliable and less prone to scheduling conflict.  
- **Opt for private rooms in boroughs like Brooklyn** if budget is a concern — they often provide a better deal vs entire apartments in Manhattan.  
- **Look for essential amenities**: Wi‑Fi, air conditioning, heating, a well‑equipped kitchen, washer/dryer etc. These tend to increase comfort, especially for longer stays. (Many NYC listings already have these; having them makes a big difference.) :contentReference[oaicite:0]{index=0}  
- **Check for self‑check‑in or smart locks** — flexibility in arrival times and contactless check‑ins are increasingly expected. :contentReference[oaicite:1]{index=1}  
- **Pay attention to listing descriptions & photos** — good visuals, clear descriptions, and correct amenities can help avoid surprises.  

---

### For Hosts

- **Ensure your listing is legally registered** (e.g. comply with NYC’s short‑term rental laws / registration requirements) to avoid penalties or delisting. :contentReference[oaicite:2]{index=2}  
- **Maintain high‑quality amenities** — amenities like strong Wi‑Fi, AC, a clean kitchen, washer/dryer, modern appliances matter a lot. Adding less common but desirable amenities (smart locks, eco‑friendly touches, special entertainment) can help your listing stand out. :contentReference[oaicite:3]{index=3}  
- **Improve guest experience with prompt responses, good communication, and maintaining cleanliness** — hosts with better response rates and positive reviews tend to book more often.  
- **Optimize pricing with market trends** — be aware of what other listings in your neighborhood are offering and at what prices; adjust during high & low demand seasons.  
- **Track performance using feedback and analytics tools** — use ratings, reviews, occupancy data, and other metrics to identify where improvements are needed.  

---

## Conclusion

This project provides valuable insights into the New York Airbnb market, offering clarity for both guests and hosts. Through Exploratory Data Analysis (EDA), we uncovered key trends such as:

- Pricing differences across boroughs, with Manhattan commanding the highest average rates.  
- Entire home/apartment listings being substantially more expensive than private or shared rooms.  
- The presence of extreme price outliers that can skew statistical summaries.  
- Correlations between availability, reviews, and pricing, suggesting reflections of guest experience and host responsiveness.

These findings allow guests to make more informed choices and hosts to adjust their strategies accordingly.  

---


