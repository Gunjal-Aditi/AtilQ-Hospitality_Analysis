# AtliQ-Hospitality_Analysis 🏨

## [Live Dashboard](https://bit.ly/3Ol8Oiy) 

## 1. Overview 🔍
AtliQ Grands is a renowned luxury hotel chain operating across India. However, it is facing a decline in market share and revenue due to ineffective management decisions. To tackle this, the revenue management team is utilizing Business Intelligence and Data Analysis to bridge gaps and enhance business performance.

The team aims to hire a skilled Data Analyst to provide actionable insights to counter the challenges.

## 2. Project Goals 🎯
1. Develop essential metrics based on predefined lists 📊
2. Construct a dashboard based on stakeholder requirements 🖥️
3. Generate insightful findings that go beyond predefined metrics and mock-up dashboards 💡

## 3. Import & Explore Data 📥🔎
### A. Importing Data into Power BI 💼
Import data from multiple tables into Power BI, including both fact and dimension tables.

### B. Using SQL to Explore Data 💻
Use SQL to understand available data before diving into analysis.

#### AtliQ Grands Overview 🏨
- 7 properties in 4 cities
- Rooms: Elite, Premium, Presidential, and Standard 🛏️
- 6 main booking platforms and some less effective alternatives 📅

#### Provided Dataset 📂
- **dim_date** – This table contains date-related information, including dates, week numbers, and day types (weekend and weekday). 🗓️
- **dim_hotels** – This table provides data on property identifiers, property names, categories, and city locations Hotel details 🏨
- **dim_rooms** – This table details room identifiers and room classifications.🛏️
- **fact_aggregated_bookings** – This fact table features property IDs, check-in dates, room categories, successful bookings, and capacity information. 📊
- **metrics list** – This dataset contains a collection of key performance measures, complete with the DAX formulas used to compute them. 🔑
- **fact_bookings** – Booking details, financial info, ratings 💰

## 4. Data Modeling 🛠️
Data modeling is essential for performance. After importing data into Power BI:
1. Clean, format, and transform using Power Query 🧹
2. Establish relationships using **Star Schema** or **Snowflake Schema** 🔗
3. Validate data against stakeholder benchmarks ✅

## 5. Dashboard Designing 🎨
The dashboard will be created based on mockups received from stakeholders. Users can navigate through different views:

### Home View
In the Home view, all the view buttons will be accessible. Users will land on specific view pages by clicking the button and you can navigate to the certain view.

The different views are:

| Views | Description | 
| ------ | ----------- | 
| Overall | It gives an overview of all the data which belongs to revenue, bookings, ratings, etc. | 
| Revenue | It enables users to analyze revenue of the AtliQ's hotels and enables them to understand the total bookings and expand other financial metrics|
| Booking   | It shows a detailed analysis of bookings efforts, which supports explaining different key metrics |

Here is the list of basics:

**Day Type** – Day is the category of days in a week. Weekday and Weekend. In the hospitality sector, the weekend is Friday and Saturday. Most of the customers checkout on Sunday.

**Booking Platforms** – Booking platforms are the modes that are used by customers to book rooms. These include AtliQ’s own booking platform and third-party platforms as well.

**Week Number**– Week number is the number of weeks in a year.

**Property Name** – Property name is the name of individual hotels.

**Property ID** – Property ID is the unique ID given to the properties.

**WoW** – Week on Week is the metric to compare the performance change over the week.

Here is the list of measures:

| Measures | Description |
| ------ | ---------- |
| Revenue | It is the most common metric used in every industry to get the total revenue_realized | 
| Total Bookings  | To get the total number of bookings happened | 
| Total Capacity | To get the total capacity of rooms present in hotels | 
| Total Succesful Bookings  | To get the total successful bookings happened for all hotels | 
| Occupancy %  | Occupancy means total successful bookings happened to the total rooms available(capacity) | 
| Average Rating  |  Get the average ratings given by the customers |
| No of days  | To get the total number of days present in the data. In our case, we have data from May to July. So 92 days.|
| Total canceled bookings | To get the"Cancelled" bookings out of all Total bookings happened  |
| Cancellation % |  Calculating the cancellaton percentage. |
| Total Checked Out |  To get the successful 'Checked out' bookings out of all Total bookings happened |
| Total no-show bookings  | "No show" means those customers who neither canceled nor attend to their booked rooms |
| No Show rate %  | Calculating the no show percentage.  |
| Booking % by Platform  |  To show the percentage contribution of each booking platform for bookings in hotels. |
| Booking % by Room class  |  To show the percentage contribution of each room class over total rooms booked. |
| ADR  |  Calculate the ADR(Average Daily rate). It is the ratio of revenue to the total rooms booked/sold. It is the measure of the average paid for rooms sold in a given time |
|  Realisation % |  calculate  the realisation percentage.It is nothing but the successful "checked out" percentage overall bookings happened.|
| RevPAR  |  Calculate the RevPAR(Revenue Per Available Room) RevPAR represents the revenue generated per available room, whether or not they are occupied. RevPAR helps hotels measure their revenue-generating performance to accurately price rooms. RevPAR can help hotels measure themselves against other properties or brands. |
| DBRN  |  calculate DBRN(Daily Booked Room Nights). This metrics tells on average how many rooms are booked for a day considering a time period |
| DSRN   |  calculate DSRN(Daily Sellable Room Nights). This metrics tells on average how many rooms are ready to sell for a day considering a time period. |
| DURN | calculate DURN(Daily Utilized Room Nights). This metric tells on average how many rooms are succesfully utilized by customers for a day considering a time period |
| Revenue WoW change % | To get the revenue change percentage week over week. Here, revcw  for current week, revpw for previous week |
|  Occupancy WoW change % | To get the occupancy change percentage week over week.Here, revcw  for current week ,revpw for previous week  |
| ADR WoW change %  | To get the ADR(Average Daily rate) change percentage week over week.Here, revcw  for current week, revpw for previous week  |
| Revpar WoW change % |  To get the RevPar(Revenue Per Available Room) change percentage week over week. Here, revcw  for current week, revpw for previous week |
| Realisation WoW change %  |  To get the Realisation change percentage week over week. Here, revcw  for current week, revpw for previous week |
| DSRN WoW change % | To get the DSRN(Daily Sellable Room Nights) change percentage week over week.Here, revcw  for current week, revpw for previous week  |

### Key Insights 🔍
- Mumbai leads in revenue generation, amassing a substantial 669 million, with Bangalore, Hyderabad, and Delhi following suit.
- Among the seven types of properties, AtliQ Exotica stands out with remarkable performance, ranking in 320 million in revenue, boasting a solid rating of 3.62, achieving an impressive 
  occupancy rate of 57%, and experiencing a cancellation rate of 24.4%.
- AtliQ Bay takes the crown for the highest occupancy rate, reaching an impressive 66%.
- Week 24 emerges as the most profitable week of all, with revenue soaring to 139.6 million.
- In terms of both occupancy and rating, Delhi takes the lead, closely trailed by Hyderabad, Mumbai, and Bangalore.
- Unfortunately, AtliQ incurred significant losses, totaling around 298 million, due to cancellations.
- Elite-type rooms witness the highest booking rates, but they also experience a comparatively elevated rate of cancellations.

