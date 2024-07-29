# Plato Pizza Report

## Project Overview

This is a Power BI project on sales analysis of an imaginary store PLATO’S PIZZA STORES. Things are going well at Plato's, but there's room for improvement. They have been collecting transactional data for the year 2015, but really haven't been able to put it to good use. They look forward to an analysis of the data and a report to help them find opportunities to drive more sales and work more efficiently.

## Data Sources

The dataset used for this project can be found [here](https://drive.google.com/drive/folders/1sT5AReif21UXjW1kICtZPrBb8yshNSOs). This dataset contains 4 tables in CSV format.

- The Orders table contains the date & time that all table orders were placed.
- The Order Details table contains the different pizzas served with each order in the Orders table, and their quantities.
- The Pizzas table contains the size and price for each distinct pizza in the Order Details table, as well as its broader pizza type.
- The Pizza Types table contains details on the pizza types in the Pizzas table, including their name as it appears on the menu, the category it falls under, and its list of ingredients.

## Data Cleaning/Preparation

Data was efficiently cleaned and transformed with the Power Query Editor of Power BI. The following data transformation steps were taken:

- Datatype for IDs changed from “WHOLE NUMBER” to “TEXT”.
- I used the first row as header in the PIZZA TYPES table.
- Converted price column from decimal to dollar.
- As I kept digging for more insights, I continued to iterate to suit my needs.

## Exploratory Data Analysis

The company has the following questions and problem to solve with the data:

- What days and times do we tend to be busiest?
- What are our best and worst selling pizzas?
- What's our average order value?
- How much money did we make this year? Can we identify any seasonality in the sales?

## Data Analysis

### Data Modelling

Table relationships were manually detected and below is the schema of the data model:

![image](https://github.com/user-attachments/assets/fd190534-43c3-45ae-9d50-512c6167d683)

### DAX Measures

The DAX measures created for this project are as follows:

Hour Column
Hour
- Revenue Column - `Revenue`
- AVG Order Value - `AVG Order Value`
- AVG Quantity per Order - `AVG Quantity per Order`

## Results and Findings

#### Busiest Days of the week and Busiest Times of the day

![image](https://github.com/user-attachments/assets/026c3a9c-9489-4085-a256-6dd0b7b992ef)

##### Busiest Days of the Week
My analysis reveals a clear pattern in customer orders throughout the week. Fridays are the busiest day, with 3.5K orders. This peak is likely driven by end-of-week celebrations and social gatherings, making it a crucial day for the business. Following closely is Saturday, with 3.3K orders, indicating that weekends, in general, see a surge in demand as customers indulge in leisure activities and dining out.

Midweek, from Tuesday to Thursday, maintains a steady flow of orders, ranging from 3.0K to 3.2K. This stability suggests that these days are consistently good for business, providing a reliable customer base. In contrast, Sundays see the lowest order volume at 2.6K, potentially due to customers preparing for the upcoming week and spending time at home. Mondays, slightly busier than Sundays with 2.8K orders, also reflect a slower start to the week.

##### Busiest Times of the Day
The time of day analysis provides further insight into customer order patterns. I observe a significant spike in orders at 11:00 AM, reaching 2.3K, which aligns with lunchtime when many customers seek convenient meal options. However, the most substantial order volumes occur in the evening, particularly between 5:00 PM and 7:00 PM, peaking at 7:00 PM with 2.4K orders. This period corresponds with dinner time, a critical window for the business.

Order volumes remain high from 5:00 PM through 9:00 PM, indicating sustained customer demand during the evening. Post 9:00 PM, there is a noticeable decline, with orders dropping to 1.5K by 11:00 PM, suggesting that late-night hours are quieter.

#### Best and Worst Selling Pizzas

![image](https://github.com/user-attachments/assets/2877eb2f-205e-4b8e-99d4-a01debc86b06)


##### Revenue by Category:

The Supreme category dominates the revenue landscape, contributing 30.37% of the total revenue with $220,065. Following closely, the Chicken category generates $204,226, accounting for 28.19% of the revenue. The Classic category, although slightly behind, still commands a significant 26.43% of total revenue with $191,689. Meanwhile, the Veggie category, despite being the least popular, contributes $111,099, making up 15.01% of the revenue. This distribution indicates a strong customer preference for the more robust and varied offerings in the Supreme and Chicken categories.

##### Top 5 Selling Pizzas by Revenue:
"The Classic Deluxe Pizza" stands out with 2,416 units sold, generating $41K in revenue. This indicates a high volume of sales, perhaps driven by a balance of taste and affordability. Close behind, "The Barbecue Chicken Pizza" and "The Thai Chicken Pizza" both generate $43K in revenue, with quantities sold at 2,372 and 2,315 units, respectively. These figures highlight the popularity and profitability of chicken-based pizzas. "The Spicy Italian Pizza," although generating slightly lower revenue at $35K, maintains a strong sales volume with 1,887 units sold. Finally, "The California Chicken Pizza" matches "The Classic Deluxe Pizza" in revenue with $41K from 2,302 units sold, reinforcing the appeal of chicken varieties.

##### Bottom 5 Selling Pizzas by Revenue:
On the opposite end of the spectrum, the bottom-selling pizzas present a stark contrast. "The Spinach Pesto Pizza" tops this list with $15.6K in revenue from 957 units sold, followed closely by "The Mediterranean Pizza" at $15.4K from 923 units. "The Spinach Supreme Pizza" and "The Green Garden Pizza" generate $15.3K and $14K in revenue, with 940 and 931 units sold, respectively. The least performing pizza, "The Brie Carre Pizza," only generates $11.6K from 480 units sold. This data clearly indicates these pizzas have not resonated well with customers, perhaps due to flavor profiles or pricing issues.

##### Analysis:
The best-selling pizzas are primarily from the Chicken and Classic categories, suggesting a strong customer inclination towards these flavors. The popularity of "The Classic Deluxe Pizza" in terms of quantity sold hints at a well-received product, likely due to its familiar taste and value proposition. On the other hand, the bottom-selling pizzas are predominantly from the Veggie and Spinach categories. The particularly low performance of "The Brie Carre Pizza" signals a need for a strategic review.

#### Further Insights

![image](https://github.com/user-attachments/assets/77d1aa06-a90e-450c-8bbe-fce1d6354b26)

##### Key Metrics Overview:
- Average Order Value: $38.31
- Total Revenue: $817.86K
- Total Orders: 21.35K
- Total Pizzas Sold: 50K

##### Monthly Revenue Trends:
At the start of the year in January, Plato's Pizza recorded a solid revenue of $68.8K. This suggests a steady customer base post-holiday season, indicating that many patrons maintained their pizza-ordering habits even after the festive period.

In February, revenue experienced a slight increase, reaching $70.4K. This uptick could be attributed to Valentine’s Day promotions or an overall increase in social gatherings during the month, contributing to higher pizza sales.

March, however, saw a decrease in revenue to $64.2K. This dip might reflect the end of winter and fewer holidays or events encouraging people to dine out, leading to a slight reduction in pizza orders.

April brought a notable rise in revenue to $73.4K. This boost was likely driven by Easter celebrations and the arrival of spring, prompting more outdoor gatherings and, consequently, more pizza orders.

May's revenue remained high at $71.4K, maintaining the momentum from April. This consistency could be due to continued pleasant weather and events such as Mother's Day, which might encourage family gatherings and increased pizza consumption.

June, in contrast, saw a significant decline in revenue to $56.4K. This drop might be related to the beginning of summer vacations, during which customers possibly opted for lighter meals or were traveling, leading to reduced local pizza orders.

July marked the peak of the year with the highest revenue of $72.6K. This peak could be linked to Independence Day celebrations and an overall increase in social activities during the summer, driving up pizza sales.

August's revenue dipped to $63.9K, following the July peak. This decline might be due to the end of the vacation season and the start of back-to-school preparations, which typically shift consumer focus away from dining out.

September witnessed a significant revenue drop to $38.3K, the lowest for the year. This substantial decline could be attributed to the transition into the fall season and a focus on school routines over dining out.

In October, revenue rebounded to $56.6K. This increase might be driven by Halloween festivities and more social events as people adjusted to the fall season, encouraging higher pizza sales.

November saw another rise in revenue to $70.4K. This increase could be linked to Thanksgiving celebrations and the onset of the holiday season, prompting more gatherings and pizza orders.

December, surprisingly, experienced a decline in revenue to $46.2K. Despite the holiday season, this drop might be due to customers opting for home-cooked meals during Christmas or experiencing post-holiday spending fatigue.

##### Annual Trends and Insights:
- The highest revenue month was July at $72.6K, while September was the lowest at $38.3K.
- Peaks in revenue generally occurred around major holidays and festive seasons (April, May, July, October, November).
- Significant dips were noted during transitional periods such as the end of summer (June) and the start of the school year (September).

#### Recommendations

Based on the detailed analysis of the sales data for Plato's Pizza Stores, several strategic recommendations can be made to help the business drive more sales and operate more efficiently.

1. Enhance Marketing and Promotions During Peak Times
Busiest Days:

- Fridays and Saturdays: Since these days have the highest number of orders, Plato's Pizza should capitalize on this trend by offering special deals and promotions targeted at weekend gatherings and celebrations. Examples include "Weekend Feast Deals" or "Party Packs" that cater to larger groups.
- Midweek Stability: Maintaining consistent midweek promotions can help sustain the steady flow of orders observed from Tuesday to Thursday. Introducing loyalty programs or midweek discounts could incentivize regular customers to order more frequently.

- Busiest Times:

- Lunchtime (11:00 AM): Implement lunch specials or combos aimed at the working population and students. Quick service and value-for-money meals can attract more lunchtime orders.
- Dinner Time (5:00 PM - 9:00 PM): Focus on family meal deals, dinner combos, and timely delivery service to cater to the high demand during this period. Advertising these deals during late afternoon hours can capture the attention of customers planning their dinner.

2. Revamp Low-Performing Menu Items

- Best-Selling Pizzas:

- Top Sellers: Highlight and promote the best-selling pizzas such as "The Classic Deluxe Pizza" and "The Barbecue Chicken Pizza" in marketing campaigns. Featuring customer favorites in promotions can drive sales and enhance customer satisfaction.

- Worst-Selling Pizzas:

- Underperformers: Conduct a thorough review of the least popular pizzas like "The Brie Carre Pizza" and "The Green Garden Pizza." Consider either improving the recipes or replacing them with new, innovative options that align more closely with customer preferences.

- Menu Optimization:
Introduce new pizzas based on popular ingredients from best-selling categories (Supreme and Chicken). Limited-time offers and seasonal pizzas can also keep the menu fresh and exciting.

3. Implement Targeted Seasonal Campaigns

- Seasonal Sales Trends:

- Holiday Peaks: Develop strategic marketing campaigns around major holidays and festive seasons that historically see revenue peaks (April for Easter, July for Independence Day, October for Halloween, November for Thanksgiving).
- Low Seasons: Address revenue dips in months like June and September by introducing summer-themed promotions or back-to-school discounts. These can include family bundles or student meal deals to attract specific customer segments during slower periods.

4. Optimize Operational Efficiency

- Data-Driven Decisions:

- Utilize the insights from peak times and best-selling items to optimize inventory management and reduce waste. Ensure that high-demand ingredients are always in stock, especially during peak days and times.

- Analyze delivery times and staffing levels to ensure prompt service during busy periods. Adjust staff schedules to align with peak order times to enhance customer service and reduce wait times.

Technology Integration:
Implement an advanced ordering system that can handle high volumes efficiently and offer seamless online ordering options. Encourage customers to place orders through an app or website, offering exclusive online deals to drive digital engagement.

5. Enhance Customer Experience and Loyalty

- Customer Feedback:

- Actively seek customer feedback on menu items and service quality. Use this feedback to make informed adjustments to the menu and improve service delivery.
- Regularly update customers on new promotions, menu changes, and special events through social media, email newsletters, and in-store promotions.

- Loyalty Programs:
Introduce or enhance a customer loyalty program that rewards frequent buyers with discounts, free items, or exclusive offers. Personalized rewards can increase customer retention and repeat business.

#### Conclusion
By strategically enhancing marketing efforts, revamping low-performing menu items, implementing targeted seasonal campaigns, optimizing operational efficiency, and focusing on customer experience, Plato's Pizza can drive more sales and improve overall business efficiency. Leveraging data-driven insights will enable the store to make informed decisions and stay ahead of customer preferences, ensuring sustained growth and profitability.
