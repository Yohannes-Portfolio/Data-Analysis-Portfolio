# Project

Maven Roasters, which started in 2018, is a specialty coffee outlet that caters to a large demographic of customers with its retail outlet serving coffee, tea, bakery, and specialty drinks.

The company has seen record growth in the first half of 2023, with revenue growing 94% and transaction volume growing 106% over the first six months. In this growth explosion, the company now has gigantic amounts of transaction data that have not been leveraged before. In this project, six months of granular transaction data are extensively analyzed in an attempt to find key insights which will further propel this growth trend and reveal opportunities to further automate Maven Roasters' commercial success.

## Insights and recommendations are presented in the following key areas:

- Temporal Revenue Analysis: Analysis of sales patterns day-by-day and hour-by-hour to determine peak performing times to staff and inventory control.
- Product-Level Performance: Analysis of product and category-level performance, top revenue drivers analysis, and portfolio optimization opportunity.
- Customer Transaction Patterns: Analysis of buying patterns, frequency, and spend behavior for application in informing marketing and operating decisions.
- Strategic Growth Opportunities: Fact-based suggestions on how to sustain top-line growth and optimize operating productivity.

## Data Structure & Initial Checks

Maven Roasters' transaction database as seen below consists of a single table with detailed point-of-sale records, containing a total of 149,116 transaction records across six months (January-June 2023).

<img width="291" height="389" alt="image" src="https://github.com/user-attachments/assets/d6dd1634-e069-45a1-9ffb-08e6c4ba88b5" />

Before analysis was begun data cleaning operations involved the elimination of duplicate transactions, the resolution of null fields in non-key fields, and date/range time validation to ensure consistency in the data.

## Deep Dive Insights

<img width="1539" height="225" alt="image" src="https://github.com/user-attachments/assets/ddad6b43-6b2f-4925-91c9-9de9251040a0" />

### Revenue Is Highly Concentrated in Morning Hours

- The morning window from 8-11am generates 49% of total daily revenue—nearly half the business occurs in just four hours. The peak hour alone (10am) contributes 12.7% of the entire day's revenue. This extreme concentration is consistent across the entire six-month period.
- This pattern is identical every single day of the week, with minimal variance between weekdays and weekends. Saturday generates $23.4K in daily revenue compared to Monday's $24.1K—just a 3% difference. The data shows that day of week has virtually no impact on revenue performance, while time of day is the dominant factor.
- Afternoon hours (12-5pm) contribute 34% of daily revenue but operate at significantly lower productivity, generating an average of 5.7% revenue per hour compared to the morning's 12.2% per hour. This represents a 41% productivity gap between morning and afternoon periods. Evening hours (6-8pm) contribute less than 10% of daily revenue combined.

### Extreme Product Concentration and Transaction Value Variation

<img width="1532" height="659" alt="image" src="https://github.com/user-attachments/assets/ceb2e2fd-f22f-4c8f-aca8-8830f4b7a2ed" />

- Three products—Barista Espresso ($94K, 13.1%), Brewed Chai Tea ($79K, 11.0%), and Hot Chocolate ($76K, 10.6%)—account for 35% of total revenue. The top 10 products generate 77% of revenue ($554K of $719K), while the remaining 40+ menu items contribute just 23%. This concentration remained stable throughout the six-month growth period.
- Average transaction value varies dramatically across products, with premium items generating significantly more revenue per customer. Hot Chocolate averages $8.62 per transaction while Gourmet Coffee averages $4.18 per transaction—more than a 2x difference. The overall average transaction value across all products is $4.90.
- Revenue growth of 94% was driven almost entirely by transaction volume growth of 106%, while average transaction value remained flat at $4.71-5.00 throughout the period. This indicates growth is coming from customer acquisition and retention rather than increased spending per customer.

### Coffee and Tea Dominate Category Mix

<img width="1025" height="739" alt="image" src="https://github.com/user-attachments/assets/5963626f-0ba6-4cf4-ba2b-4c3fe04bb914" />

- Coffee represents 38% of total revenue ($273K) and Tea represents 28% ($201K)—together these two categories account for 66% of the business. This concentration remained consistent throughout the growth period, with both categories maintaining their revenue share even as overall volume doubled.
- Bakery items contribute 15% of revenue ($110K), Drinking Chocolate contributes 11% ($76K), and other categories make up the remaining 8%. Category composition showed minimal variance across the six months, indicating stable customer preferences.
- The coffee-heavy product mix aligns with the morning revenue concentration pattern. Coffee consumption is culturally associated with morning hours, which corresponds with the observed afternoon productivity decline.

## Recommendations

- Despite strong growth (94% revenue increase), afternoon productivity is 41% lower per hour than morning. Launch an afternoon menu strategy featuring Tea, Iced beverages, and Drinking Chocolate with targeted promotions. Reposition afternoon offerings as "refresh" rather than coffee-focused. Train staff to suggest these alternatives during afternoon hours rather than defaulting to the coffee-heavy morning menu.
- With a 2x transaction value gap between premium ($8.62) and budget items ($4.18), implement systematic upselling training. Staff should suggest upgrades ("Upgrade to Barista Espresso for $1.50 more?") and size increases ("Make it a large for 50¢?"). Visual menu boards should highlight premium options and make upselling natural for both staff and customers.
- Simplify the product portfolio by discontinuing bottom-performing SKUs. With top 10 products generating 77% of revenue, the remaining 40+ items create disproportionate complexity in inventory management, staff training, and menu design. Eliminate items contributing less than 1% of revenue individually to focus resources on proven winners.
- Adjust operating hours based on revenue patterns. Evening hours (6-8pm) contribute less than 10% of daily revenue while maintaining full staffing costs. Consider reduced hours, limited evening menu with skeleton staff, or targeted promotions to boost this daypart. A cost-benefit analysis is recommended.
- Protect the "Big 3" products (Barista Espresso, Chai Tea, Hot Chocolate = 35% of revenue) through redundant supply chains and quality controls. Any disruption to these mission-critical products directly impacts one-third of business performance. Ensure these items never experience stockouts and maintain consistent quality standards.

## Caveats & Assumptions

The analysis and recommendations are based on the following assumptions and limitations:

- Six-month timeframe: Data covers January-June 2023 only. Seasonal patterns outside this period (summer, holidays) are not captured and may differ from observed trends.
- Revenue focus only: Cost data (COGS, labor, overhead) was not available. Financial modeling incorporating margin analysis is recommended before implementation.
- Stable external conditions: Analysis assumes relatively consistent external factors (weather, competition, local events). Significant environmental changes may alter customer behavior patterns.
- Implementation capacity: Recommendations assume operational capability to execute changes (staffing, space, technology). Feasibility assessment required.
