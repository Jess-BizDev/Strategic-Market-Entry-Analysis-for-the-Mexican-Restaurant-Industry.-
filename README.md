# Strategic-Market-Entry-Analysis-for-the-Mexican-Restaurant-Industry.-
![Market Entry Roadmap](Github%20Cover%20photo%20for%20restaurant%20analysis.png)
In this analysis, I utilized Power BI to analyze 1,161 consumer ratings and identified high-ROI investment gaps in San Luis Potosí to support Market Entry Strategy and Investment Risk Mitigation.
[Download Power BI Source File(.pbix)](Restaurant_Rating_Data_Analysis.pbix)
## Project Objective: To determine the commercial viability and operational blueprint for a new culinary venture in Mexico.

### 1. Executive Summary
As a Business Development Manager, I know that entering a new market is one of the highest-risk moves a company can make. The difference between a failed venture and a market leader often comes down to Data-Driven Intelligence.
This report presents a comprehensive market entry strategy for the culinary sector in Mexico. While traditional investment models often rely on intuition, this study leverages 1,161 individual rating entries to identify a high-probability Product-Market Fit. By analyzing the intersection of consumer behavior (138 unique diners) and competitive supply (130 restaurants), we have identified a specific "Lean" investment model that minimizes operational overhead while maximizing customer satisfaction.

### 2. Data Cleaning & Integrity
To ensure the integrity of this investment strategy, I performed the following ETL (Extract, Transform, Load) steps in Power Query:

#### - Volume Verification
Utilized a COUNTROWS function to confirm a foundation of 1,161 individual reviews.
#### - Data Modeling
Established a Star Schema to link consumer demographics to performance ratings, ensuring all interactive visuals are mathematically synchronized.
#### - Handling Nulls
Cleaned "Unspecified" entries in budget and transport columns to prevent demographic skewing.

### 3. Research Questions & Intelligence Gathering
#### Question 1: What can you learn from the highest rated restaurants? Do consumer preferences have an effect on ratings?
Establishing a market baseline is the first step in performance benchmarking.
#### The Metric
- Using the DAX measure Average Overall Rating = AVERAGE(Ratings[Overall_Rating]), we identified a market-wide baseline of 1.20 out of 2.00.
- Our analysis confirms that satisfaction is highly dependent on cuisine alignment. Cuisines like Japanese and Coffee Shop consistently outperform the baseline, proving that investment must follow pre-existing consumer tastes to ensure high ratings.
- Ratings drop significantly when there is a mismatch between what consumers want and what the restaurant provides. Top-rated venues succeed because they align their service model (e.g., No Smoking Policy) with the specific lifestyle habits of the local demographic.

![Consumer Demographic & Market Performance Analysis](Restaurant%20Rating%20Analysis%20Page%201.png)

#### Question 2: What are the consumer demographics? Does this indicate a bias in the data sample?
Understanding the "Who" and "Where" is vital for site selection.
#### The Target
- 82% of the market are Students, primarily in their 20s, with 96% possessing Low to Medium spending power
#### The Bias
- There is a significant Geographic Bias, with 62% (86 consumers) concentrated in San Luis Potosí.
#### Business Conclusion
- Any successful market entry must be student-centric and geographically focused on San Luis Potosí to minimize customer acquisition costs.
#### Question 3: Are there any demand & supply gaps that you can exploit in the market?
We compared Cuisine Demand (total preferences) against Cuisine Supply (active competitors).
#### The Opportunity
- Mexican Cuisine represents the single largest "Blue Ocean" opportunity. It has a massive demand score of 97 but is served by only 28 restaurants.
#### The Gap
- This 69-point deficit represents an underserved market segment ready for a new entrant to capture volume.

![Investment Strategy: Mexican Cuisine Opportuinity](Investment%20Strategy%20Dashboard.png)

#### Question 4: If you were to invest in a restaurant, which characteristics would you be looking for?
A deep dive into the "Strategic Blueprint" of the Top 10 performers revealed a critical duality in the market:
#### The Lean Discovery
- While broad data suggests amenities are helpful, 6 out of the top 10 restaurants achieve 5-star ratings without alcohol service, without smoking sections, and without dedicated parking.
#### The Profile
 - These elite performers are  Medium-Priced and focus purely on culinary excellence rather than high-cost infrastructure.
### 4. Strategic Recommendations for Market Entry Roadmap
Based on the synthesis of 1,161 data points, I recommend the following Market Entry Roadmap:
#### 1.	Phase 1: The "Lean Entry" Model
- A.	Permitting: Launch without an alcohol license to save on high permitting costs and legal overhead, as 70% of top performers operate successfully without it.
- B.	Infrastructure: Focus on a "Medium" price point in a smoke-free environment. Do not prioritize expensive parking leases initially, as the top performers prove this is not a prerequisite for 5-star ratings.
#### 2.	Targeted Niche Selection:
- A.	Cuisine: Exclusively focus on Mexican Cuisine to capitalize on the 69-point supply-demand gap. The demand (97) and supply (28) represents a classic market void. This is our clearest path to capturing a huge market share with minimal initial competition.
- B.	Demographic: Brand the restaurant as "Student-Premium" that offers high-quality Mexican food at a price point accessible to the 82% student majority.
#### 3.	Geographic Site Optimization:
- A.	Location: Site the restaurant in central San Luis Potosí to leverage the 62% geographic concentration. With 62% of the consumer base concentrated here, it offers the highest density of target customers and the lowest cost of customer acquisition.
- B.	Accessibility: Choose a location within 500 meters of a public transit hub to accommodate the 60% of consumers who use public transport while also considering Public Parking to capture the 25% car-dependent market.

### 6. Conclusion
The data is conclusive. By adopting a Lean Operational Model in the high-demand Mexican Cuisine segment of San Luis Potosí, an investor can enter the market with lower CAPEX and a higher probability of achieving the elite status held by current top performers. This strategy transforms a high-risk venture into a calculated, data-backed market expansion.

#### Scroll Down for Technical Appendix
Connect with me on
[Linkedin](https://www.linkedin.com/in/rasheedat-jessica-alliagbor/)


---
## **Technical Appendix**

As a Business Development professional, data integrity is paramount. The following DAX measures were engineered to provide the mathematical foundation for the Market Entry Strategy.
```
### 1. Market Performance Baseline
Establishes the average performance across all 1,161 rating entries to identify market leaders.

```dax
Average Overall Rating = AVERAGE(Ratings[Overall_Rating])
