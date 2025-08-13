✈️ Flight Price Analysis – Data Cleaning & EDA
📌 Project Overview
This project involves data cleaning and exploratory data analysis (EDA) on a flights dataset to uncover patterns, relationships, and key factors influencing flight ticket prices.
The analysis helps identify trends across airlines, routes, stops, and other factors, which can be useful for pricing strategy, travel planning, and predictive modeling.

📂 Dataset Information
Source: flight_price.csv
Shape: 10,683 rows × 11 columns

Columns:

Airline – Name of the airline

Date_of_Journey – Date of travel (DD/MM/YYYY)

Source – Departure city

Destination – Arrival city

Route – Route taken by the flight

Dep_Time – Departure time

Arrival_Time – Arrival time

Duration – Total travel time (hours/minutes)

Total_Stops – Number of stops

Additional_Info – Extra services or info (e.g., baggage, meals)

Price – Ticket price (target variable)

🛠 Data Cleaning Steps
Handling Missing Values

Route and Total_Stops had 1 missing value each → dropped or imputed as required.

Feature Transformation

Converted Date_of_Journey to datetime and extracted day and month.

Converted Duration to numeric minutes for better analysis.

Parsed Dep_Time and Arrival_Time into time-of-day formats.

Outlier Detection

Checked extreme values in Price (above ₹40,000) for possible capping.

📊 Key EDA Insights
Average Price: ₹9,087 | Min: ₹1,759 | Max: ₹79,512

Top Airlines (by flights): Jet Airways, IndiGo, Air India

Premium vs Budget: Business-class carriers have much higher fares; low-cost airlines dominate budget travel.

Stops Impact: In this dataset, flights with more stops tend to be more expensive (possibly due to distance covered).

Duration Relation: Longer flights generally cost more.

Seasonal Trend: Prices vary across months (potentially higher in peak travel months).

📈 Visualizations Included
Price distribution histogram

Price by airline (boxplot)

Price vs number of stops

Average price by source–destination pair

Departure time frequency

📄 PDF Report: Contains all plots & insights.

🚀 Future Work
Build a flight price prediction model using cleaned features.

Perform time-series analysis on prices over different months.

Add external features like holiday seasons or demand factors.

📜 Requirements
bash
Copy
Edit
pandas
numpy
matplotlib
seaborn
scipy
statsmodels
wordcloud
scikit-learn

📬 Author
Supratim Mukherjee
Data Science Enthusiast | Exploratory Data Analysis & Machine Learning