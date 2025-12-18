# U.S. Breweries Analysis

## 📌 Project Overview
This project analyzes the distribution of breweries across the United States to uncover geographic patterns, brewery types, and population-normalized brewery density. 

The dataset was programmatically extracted using the *OpenBreweryDatabase API*, reflecting a real-world data acquisition workflow.

---

## 🎯 Objectives
* *Analyze* the geographic distribution of breweries across U.S. states and cities.
* *Identify* dominant brewery types.
* *Compare* states using both absolute counts and brewery density per 100,000 people.
* *Highlight* brewery hotspot regions.

---

## 🧾 Data Source

### Primary Dataset
* *Source:* OpenBreweryDatabase API
* *Coverage:* All breweries in the United States
* *Records:* 7807 breweries (7256- Post Processing)
* *Key Fields:* brewery_type, city, state, country

### Supporting Dataset
* *U.S. State Population Data:* Used to calculate brewery density per 100,000 people.

---

## 🛠 Tools Used
* *OpenBreweryDatabase API:* Data extraction.
* *Microsoft Excel:* Data cleaning, Pivot tables, XLOOKUP, and KPI cards.

---

## 🧹 Data Cleaning & Preparation
The following steps were performed before analysis:
1. *Consolidation:* Merged API responses into a single dataset.
2. *Cleaning:* Removed unused columns and standardized state names.
3. *Integration:* Joined brewery data with population data using XLOOKUP.
4. *Metrics:* Created calculated fields for *Brewery Counts* and *Density*.

---

## 📈 KPIs Included
The following metrics provide a high-level snapshot of the industry:
* *Total Breweries*
* *Total States Covered*
* *Most Common Brewery Type*
* *State with Highest Brewery Count*
* *State with Highest Brewery Density*

---

## 🔍 Analysis & Key Findings

### 1️⃣ Brewery Type Distribution

<img width="600" height="371" alt="Brewery type distribution" src="https://github.com/user-attachments/assets/7b6e9310-8f66-4c10-833f-5a89f55edca8" />

*Insight:* Microbreweries dominate the U.S. brewery ecosystem with arounf 57% indicating a strong market for small, independent craft producers.

### 2️⃣ Breweries by State (Total Count)

<img width="600" height="371" alt="States with most brewries" src="https://github.com/user-attachments/assets/6cd43727-0b88-404c-aee4-bd6961a362b3" />
*Insight:* California leads in total brewery count, driven by its large population and urban concentration.

### 3️⃣ Brewery Hotspot Cities

<img width="600" height="371" alt="Cities with most brewries" src="https://github.com/user-attachments/assets/9fe8c86b-48ea-4ca9-bf44-66495efda8bb" />

*Insight:* Specific cities like *Portland* and *San Diego* emerge as dominant hubs with high concentrations of establishments.

### 4️⃣ Brewery Density Analysis (Key Metric)

The density was calculated using the formula:
$$Brewery\ Density = \frac{Number\ of\ Breweries}{Population} \times 100,000$$

<img width="600" height="371" alt="Top 10 states with brewries per 100k people" src="https://github.com/user-attachments/assets/b0ddf0b3-5ceb-4f44-b90a-28404f230482" />

<img width="3399" height="2295" alt="geo hotspot" src="https://github.com/user-attachments/assets/4572c725-9899-4524-89bc-9fd615b27a1e" />

*Insight:* Raw counts can be misleading. States like *Maine* and *Utah* rank significantly higher in density despite having fewer total breweries than California.

---

## 💡 Business Interpretation
---

## 1️⃣ Microbreweries Dominate the U.S. Brewing Industry
Microbreweries form the overwhelming majority of establishments in the U.S. dataset.
* *Key Takeaway:* The industry is primarily driven by small, independent, craft-focused businesses rather than large regional or national players. This suggests a consumer preference for local branding and specialized flavors.

---

## 2️⃣ Geographic Distribution is Highly Uneven
Brewery presence is not spread equally across the country.
* *The Leaders:* A small number of states account for a disproportionately high share of total breweries.
* *California:* Holds the highest total count, largely driven by its massive population and urban density.
* *Regional Imbalance:* Many states remain significantly underserved, highlighting a clear regional imbalance in the craft beer market.

---

## 3️⃣ High Brewery Count ≠ High Brewery Density
The data proves that raw numbers can be misleading. A state can have hundreds of breweries but still have a low "per capita" availability.
* *The Comparison:* When adjusted for population, smaller states frequently outperform larger ones.
* *Example:* While California has a massive count, its density is only *≈ 2.26 breweries per 100,000 people*, which is moderate compared to smaller craft-heavy states.

---

## 4️⃣ Smaller States Lead in Brewery Density
Population-normalized metrics provide a much more accurate "Fair Comparison" between states.
* *Top Performers:* States like *Maine and Utah* rank among the highest in brewery density.
* *Insight:* These states have a high concentration of breweries relative to their residents, indicating a deeply rooted local beer culture.

---

## 5️⃣ Brewery Activity is Clustered in Specific Cities
Growth is not just state-wide; it is highly localized.
* *Hotspots:* Cities like *Portland* and *Denver* emerge as clear brewery hubs.
* *Ecosystems:* This clustering suggests that these cities have strong local craft culture, high tourism demand, and supportive business regulations.

---

## 6️⃣ Strategic & Business-Level Takeaways
* *Tourism:* High-density states are the strongest candidates for brewery-related tourism and hospitality investments.
* *Market Entry:* Low-density states may represent *untapped or emerging markets* where competition is lower.
* *Competition:* Brewery-heavy cities may face higher barriers to entry, requiring new businesses to have a very strong unique selling proposition (USP).

---

## ⚠ Limitations
* No sales or revenue data was included in the API.
* Density is based on population, not consumption rates.
* City-level population data may have minor alignment variances.

---

## 🏁 Conclusion
This project demonstrates a complete analytical workflow—from API-based data extraction to data cleaning and insight generation. By utilizing *normalized metrics* (Density), the analysis provides a much deeper understanding of market saturation than raw totals alone.
