# Retail-Store-Inventory-and-Demand-Forecasting-Analytics
Retail Stores Inventory Management and Demand Forecasting. 
A Full Business Analytics Project Using SQL Server Connected With Power BI.

This Project Focused On The Relationship With: (Sales Performance, Expected Demand, Inventory Management, Restocking, And Inventory Risk) Into One Framework That Supports Decisions.

<img width="1920" height="1143" alt="Screenshot (220)" src="https://github.com/user-attachments/assets/6f1d89b3-4ae8-4721-b11e-86694dd6a2e7" />
<img width="1920" height="1143" alt="Screenshot (221)" src="https://github.com/user-attachments/assets/40e7a519-c0cb-4952-b3c1-ce830c913d80" />
<img width="1920" height="1146" alt="Screenshot (223)" src="https://github.com/user-attachments/assets/13e9cc94-ef9d-49eb-a723-68307de6ad56" />
<img width="1920" height="1140" alt="Screenshot (225)" src="https://github.com/user-attachments/assets/0355bb5c-88d1-40c9-a615-79f4d23e6ef3" />
<img width="1920" height="1143" alt="Screenshot (228)" src="https://github.com/user-attachments/assets/b809735d-c0c5-4e4c-835b-7e25035c3a07" />
<img width="1920" height="1140" alt="Screenshot (229)" src="https://github.com/user-attachments/assets/2375cc1d-b552-497b-962d-cf5303fcfcc7" />
<img width="1920" height="1136" alt="Screenshot (219)" src="https://github.com/user-attachments/assets/2cbe560b-3227-4ea3-a311-c93987eec19f" />




Executive Summary

Managing retail inventory means balancing two opposite risks: 
  Not having enough stock:-  which can limit what's available to sell
  having too much stock:-    which can tie up money and increase storage cost.

This project built a Power BI decision support solution for a retail network of (5 stores, 20 products, 5 categories)
Date records covering two years of daily data
The goal wasn't just to report past sales but to connect (sales performance, expected demand, inventory levels, restocking activity, and inventory risk) into one framework that supports decisions.


The Core Inventory Problem: The retailer faces two opposite situations.
 - Understock  If inventory drops below what's needed to cover expected demand the business becomes more exposed to availability problems.
 - Overstock   If inventory stays much higher than what's needed for expected demand money can stay tied up in products that aren't selling fast enough.

So the real challenge is: Is the inventory we have right for the demand we expect and where should restocking attention go first?
 - What are we selling and where is performance concentrated?
 - Where is inventory getting tight and where is there too much?
 - Which Store or Product combinations need attention first?


The project has there connected dashboards:
  Page One:- Sales analysis       - Covers performance by product, category, store, region, and time.
                                  - let the user zoom into any specific segment.
  Page Two: Demand analysis       - Compares recorded expected demand, storage and comparator price against actual number at the product
                                  - To Review our forecasting and market research pricing 
  Page There: Inventory analysis  - Brings current inventory, safety stock, reorder point, and coverage together into the operational Performance table.
                                  - This is the page meant for someone to open sort by risk and take action.

The analysis shows:-
 - 7M+ units sold,  $375M+ net revenue
 - 85% fill rate, 11K inventory turnover, 11.75% demand variability 
 - Summer was the strongest season at ~28% of total revenue
 - Store S003 and Product P0014 achieved the highest sales.
 - August and Wednesday was the best-performing month and day.
 - Several products were also identified as High Stock Risk


  
Next Steps

   1- identifying inventory risks to testing and improving replenishment decisions.
   2- High risk Store and Product combinations should be reviewed first especially when inventory is below the Reorder Point.
   3- Reorder Point and Safety Stock should become part of a repeatable replenishment policy based on demand, lead time, historical sales 



Business Problem

Retail inventory management sits between two costly mistakes.
  - Having (Understock) compared to expected demand risks missed sales and poor product availability.
  - Having (Overstock)  if inventory stays much higher than what's needed for expected demand.
       Money can stay tied up in products that aren't selling fast enough
Both problems come from the same root cause demand isn't constant and it doesn't behave the same way for every Store Product combination.

The Inventory Risk
At any moment some products are getting close to running out while others are sitting with more stock than they're actually expected to sell.
Without a clear way to flag this both problems usually only get noticed after they've already cost the business money through a lost sale or a markdown.

The Demand Problem
The dataset has a recorded expected demand number for every (Store, Product, Date) 
Combination along with things that likely affect it: (seasonality, promotions, pricing, discounts, competitor prices, and weather)
Demand also varies in (how predictable it is?) not just how big it is 
Some products stay close to their expected demand consistently, while others swing a lot and that variability is itself a useful planning signal.

The Management Challenge
A monthly or weekly sales report tells a manager what already happened.
It doesn't tell them which of the twenty products across five stores needs a replenishment conversation this week.
That takes combining current inventory expected demand and variability into one prioritized view and being honest about which parts of that view are solid and which are estimated.


So the project was built around these goals:-

- This project focused on the relationship with: (Sales, Demand, Inventory, Restocking, Risk, Action)
- The real challenge isn't (How much inventory do we have?) But
  Is the inventory we have right for the demand we expect and where should restocking attention go first?
- Where is inventory risk concentrated why does it matter
- Which Store or Product combinations should be reviewed first?


Key Business Questions is:-

 - What are we selling and where is performance concentrated? Which products are performing best?
 - How does actual sales compare with recorded expected demand? 
 - Are we successfully converting forecasted demand into actual sales?
 - Where is inventory getting tight and where is there too much?
 - Which Store or Product combinations need attention first? 
 - Which stores generate the highest revenue?
 - How do promotions, weather, and seasonality affect sales?
 - Which of the underlying numbers are directly observed and which depend on an assumption?
 - Are current inventory levels enough to satisfy future demand?
 - How much inventory should be reordered?
 - Which products are at risk of stockout and how reduce it while keeping inventory efficient?



Methodology And Skills


Skills:- 
Power BI: Power Pivot, Data Transformation, Data Modeling, Data Clinging, Dax, Calculated Columns, Data Visualizations

Power BI:
  - ETL Processes, Data Clinging
  - Create "Calendar table" and DAX Measures
  - Data Modeling 
  - Designing Three connected dashboards (Overview, Stores, Performance)
  - Building KPI cards
  - Bar charts, Donut charts, Column chart, Line and Clustered column chart, and comparison tables
  - Filter panels for each dashboard (like Promotion, Weather, Store id, Product id, dates(Year, Month, Quarter, Day))
  - Keeping the same visual style and layout across all dashboards for a connected story


- Data Understanding And Grain
  - The source data works roughly at the level of: Store , Product , Date
  - With: 5 Stores, 20 Products, 5 Categories, 4 Regions ,about 73,000 records, two years of daily records
  - The analysis separates between:
      Current Inventory
      Historical Average Inventory
      Inventory at a specific point in time
  - This avoids one of the most common mistakes in inventory analysis: 
      treating daily inventory balances like they're transactions that can be added together.


- Data Preparation And Modeling everything was built entirely in Power BI using:-
  - (Power BI Desktop, Power Query, DAX)
  - I built a separate Calendar table and connected it to the main retail table through the Date field.
  - The Calendar table supports: (Year, Quarter, Month, Month Name, Day, Day Name, Week, Week Number)
  - This structure allowed for consistent time based analysis and filtering in the report.


- Data Transformation And KPI 
  Using DAX to create a lot of measures grouped by business purpose
  Each measure was built to answer a specific business question. like
   - Fill Rate:-        to quickly show whether sales are keeping up with expectations.
   - Safety Stock:-     to identify the critical point in inventory
   - Reorder Point:-    to turn that signal into a usable inventory threshold
   - Stock Risk flag:-  to turn all of this into something a manager can sort and act on without needing to understand the formulas behind it.



Analytical Methodology

The analysis followed a logical order:
   Business framing 
   Data preparation and modeling 
   Building KPIs 
   Descriptive and sales analysis 
   Demand analysis and Sales-vs-Demand comparison 
   Inventory coverage and replenishment analysis 
   Rule based risk labeling. 

Every stage up to this point is built into the current project: the stages after this  using
   Demand variability to fine tune
   Safety stock
   Statistical forecasting and scenario analysis



The project designed around these pages
 Page One:- Sales analysis covers performance by product, category, store, region, and time.
    - Page opens with five KPI cards (Total Unit Sold, Net Revenue, Total Discount, Fill Rate, Yearly Turnover)
    - Seasonality revenue breakdown
    - Monthly revenue and units trend
    - Regional and category comparisons
    - ("best of the last two years") highlights for month, day, store, and product
        giving a reader the full picture of performance in seconds.
    - Filters for (Promotion, Category, Region, Seasonality, Year, Quarter, Month, and Day Name)
        let the user zoom into any specific segment.
       
 Page Two:- Demand analysis
    - Compares recorded expected demand against actual sales at the product.
    - Page supports deeper investigation: three toggle views (Price, Product, Inventory)
      Let a user switch the same page between 
         Inventory by Product comparison
         Sales vs Demand comparison 
         Price vs Competitor Price comparison
    - While store level storage and supply and Revenue correlation charts stay visible the whole time for context. 
    - Filters for (Promotion, Category, Region, Seasonality, Year, Quarter, Month, and Day Name) let the user zoom into any specific segment.
       
 Page There: Inventory analysis
    - Brings together current inventory, safety stock, reorder point, and coverage into the operational Performance table.
    - Page turns investigation into action:
    - KPI cards for (Fill Rate, Demand Variability, DIO, and average daily sales and demand) 
    - Sit above a sortable product table listing 
       (Inventory Now, Safety Stock, Reorder Point, DIO, Order to Storage, Recommended Order, EOQ, Turnover, and Stock Risk ) 
    - Filterable by Store and Region.
    - This is the page meant for someone to open sort by risk and take action.



Results
  
Overall Commercial Performance
Across the period studied the dashboard shows roughly:
6.50M Units Sold, 375M Net Revenue, 63M Total Discount, 11K Yearly Turnover
The Executive Overview also shows that revenue isn't spread evenly across regions and categories.

 
  1-The North region and the Groceries category have the strongest revenue.
      Region
      North:       about 168M  Net Revenue
      East:        about 139M  Net Revenue
      Category 
      Groceries:   about 134M  Net Revenue
      Furniture:   about 99M   Net Revenue
      That mean: Revenue performance isn't spread evenly across the retail network.
       Inventory, promotions, and management attention don't need to be spread the same way across every region and category.
      Decision:- Use regional and category performance as one input when deciding which inventory reviews and commercial checks come first.
                 
  2-There is a recurring gap between recorded expected demand and actual sales.
      The Product Comparison view shows expected demand generally staying equal to or above actual sales for a large part of the product range.
      That mean: The number gap is real but the dataset doesn't tell us why it's happening.
      Possible reasons include:
         inventory shortages, sales coming in lower than expected, an overly optimistic demand estimate, pricing effects, 
         competitor pressure, promotion effects
      The gap is a signal to look into not a direct measure of Lost Sales.
      Decision:- Focus on the biggest gaps to a manual review to figure out whether the cause is limited inventory
             instead of assuming right away that they're stockouts.
         
  3- A specific group of products is flagged High Risk on the operational table
     Two products in particular, P0008 and P0018, show negative Order to Storage numbers in the operational data shown.
     The operational Performance table shows roughly: 35K Current Inventory, 30K Safety Stock, 41K Reorder Point, 16K Order-to-Storage, 
        24K Recommended Order 
     Some Store and Product combinations are below their calculated Reorder Point while restocking hasn't kept up with sales.
     That mean:- These combinations are the clearest candidates for a near-term inventory review.
     Decision:- Focus on High Risk products first especially the ones showing negative restocking activity.
     
  4- Store performance isn't the same across the network. Store S003 stands out as the strongest store in the analysis
     With roughly: 82M Net Revenue, 1.325M Units Sold
     The store-level analysis also shows different inventory and restocking patterns between stores.
     That mean:- One single restocking policy might not work equally well for every store.
     Decision:- Check restocking and inventory settings at the Store and Product. instead of only relying on network-wide averages.
   
  5- Several products show net revenue lower than a competitor price scenario
     The Price Chart Comparison shows products like P0001–P0007 with Net Revenue sitting below Revenue by Competitor Price
     Some products bring in less revenue with their current pricing than the modeled competitor price scenario suggests.
     That mean:- This is a scenario based on the same actual sales volume  it's not real competitor revenue.
     This points to products that might be worth reviewing for pricing.
     Decision:- Send these products for a pricing check instead of treating this result as a direct pricing recommendation.
    
    

Strategic Recommendations 
      
  1- Inventory Management: Focus on High Risk Inventory First
     Risk or Opportunity: A specific group of Product combinations is below the calculated Reorder Point 
       Showed in (Performance table Stock Risk) column
     Recommendation:      Review High Risk combinations first
                          Especially products like (P0008 and P0018) where restocking activity is also negative.
     Expected benefit:    If demand continues without proper restocking the business becomes more exposed to running out of stock.
     Priority:            High


  2- Demand Planning: Look Into the Biggest Demand Gaps 
     Risk or Opportunity: Demand Variability is different across products with an overall figure of roughly 11.75%.
       Showed in Demand Variability measure on the Performance page
     Recommendation:      Look into the biggest gaps by combining: Current Inventory, Coverage, Price, Competitor Price, Promotion
                          , Seasonality, Store before deciding on a specific cause.
     Expected benefit:    Products with more variability are harder to plan for reliably using just one fixed safety-stock rule.
     Priority:            High

  3- Store Management
     Risk or Opportunity: Stores show different patterns in revenue, volume, storage and supply.
       Showed in Storage and Supply by Store ID and Net Revenue vs Units Sold correlation charts      
     Recommendation:      Review replenishment settings store by store
                             starting with the stores that show the biggest inventory to order imbalance.
     Expected benefit:    One replenishment policy for all five stores risks over supplying some stores and under supplying others.
     Priority:            Medium

  4- Pricing Commercial: Treat the Competitor Price Analysis as a Commercial Check Not a Final Answer
     Risk or Opportunity: Several products show lower net revenue than the modeled competitor price scenario.
       Showed in The Price Comparison view flags products like (P0001 - P0007).
     Recommendation:      Run a proper commercial check before changing any prices.
     Expected benefit:    These products might be pricing opportunities but the scenario alone doesn't prove price sensitivity or extra profit.
     Priority:            Medium
      
  5-Forecasting
    Risk or Opportunity: The project currently uses the dataset's recorded expected demand field as its demand planning input
       no statistical forecasting model (moving average, exponential smoothing, ARIMA, or machine learning) has been built.
    Recommendation:      See "Next Analytical Layer" below this is the single most valuable improvement to the existing decision chain.
    Expected benefit:    Current demand numbers should be treated as a planning input not a tested forecast when shared internally.
    Priority:            High
 

Strategic Recommendations:- 

 - Prioritizing which Store or Product combinations need inventory review first using the Stock Risk flag.
 - Comparing sales against recorded expected demand to find combinations worth investigating.
 - Comparing pricing against a competitor price scenario at the product level.
 - Tracking revenue and volume trends across region, category, season, and store.
 - Highlighting replenishment activity that isn't keeping up with sales.


Next Steps

   1- identifying inventory risks to testing and improving replenishment decisions.
   
   2- High risk Store and Product combinations should be reviewed first especially when inventory is below the Reorder Point.
 
   3- Reorder Point and Safety Stock should become part of a repeatable replenishment policy based on demand, lead time, historical sales 

   4- Demand forecasting should be developed at the Store and Product starting with simple baselines such as Naive Forecast and Moving Average.

   5- Forecasting models must be tested using historical data and metrics.

   6- The replenishment policy should also be tested through historical simulation to evaluate stockouts, coverage, inventory.

   7- The final goal is a continuous process of Monitor, Investigate, Act, Measure, Improve, supported by better supply chain data and business KPIs.


