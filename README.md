# Ticket Sales Prediction Model

## Project Overview
This project focuses on predicting ticket sales for events using machine learning. The goal is to build a model that accurately estimates the number of tickets sold based on various features such as:

- **Capacity:** The maximum number of tickets that can be sold for the event.
- **Days Until Event:** The number of days remaining before the event starts.
- **Hours Until Event:** The number of hours remaining before the event starts.

## Purpose
The purpose of creating this project is to enhance the understanding of factors that influence ticket sales in the event industry. By leveraging machine learning techniques, we aim to provide event organizers and stakeholders with a predictive tool that can assist in:

- **Optimizing Ticket Pricing:** Understanding how ticket sales progress over time can help in setting optimal prices to maximize revenue.
- **Marketing Strategies:** Identifying trends in ticket sales can guide marketing efforts and promotional strategies.
- **Capacity Management:** Predicting sales accurately enables better planning of venue capacity and resource allocation.

## Future Scope
The future scope of this project includes:

- **Incorporating Additional Features:** Adding more features such as historical sales data, promotional activities, and customer demographics to enhance prediction accuracy.
- **Experimenting with Different Algorithms:** Testing various machine learning algorithms to determine which ones yield the best predictive performance.
- **Real-time Predictions:** Developing a user-friendly interface that allows event organizers to input data and receive real-time predictions.
- **Integration with Event Management Systems:** Creating APIs or tools that can integrate this prediction model into existing event management systems for automated decision-making.

## Outcomes of the Model
The outcomes of this model provide several benefits to stakeholders in the event management industry:

1. **Improved Accuracy in Predictions:** The model is designed to achieve a high level of accuracy (e.g., above 95%) when predicting ticket sales. This reliability allows for better planning and decision-making.
  
2. **Data-Driven Insights:** By analyzing past ticket sales and various influencing factors, the model provides insights that can guide future marketing and pricing strategies.

3. **Enhanced Revenue Generation:** By accurately predicting ticket sales, event organizers can optimize pricing strategies to maximize revenue while minimizing the risk of unsold tickets.

4. **Better Resource Allocation:** Understanding ticket sales patterns allows for more efficient allocation of resources, such as staffing and inventory, leading to cost savings.

5. **Actionable Recommendations:** The model can help identify trends and patterns in ticket sales, allowing event organizers to make timely and informed decisions regarding promotions, marketing campaigns, and inventory management.

## Dataset
- **File Name:** `recode.csv`
- **Source:** Google Drive (manual download)
- **Description:** The dataset contains information about ticket sales, including features that influence sales performance. It consists of multiple rows representing different events and their respective ticket sales data.

## Features of the Dataset
- **show_id:** Unique identifier for each show.
- **venue_id:** Unique identifier for the venue.
- **section_id:** Unique identifier for the section.
- **timestamp:** The time the data was recorded.
- **event_date:** The date of the event.
- **remaining_tickets:** The number of tickets left unsold.
- **capacity:** The total capacity of the venue.
- **sold_tickets:** The number of tickets that have been sold.
- **sold_percentage:** The percentage of tickets sold.
- **days_until_event:** The number of days until the event.
- **hours_until_event:** The number of hours until the event.
- **event_time_zone:** The time zone of the event.

## Getting Started

### Step 1: Download the Dataset
1. Download the dataset from the following link:
   [Download Dataset](https://drive.usercontent.google.com/open?id=1aQhPO1yHMxuTMWvAonNvrYV4rGN-PRjp&authuser=0)
2. Rename the downloaded file to `recode.csv`.

### Step 2: Setup Your Environment
1. **Install Python:** Ensure you have Python 3.x installed. You can download it from [python.org](https://www.python.org/downloads/).
2. **Install Required Libraries:** Create a `requirements.txt` file with the following contents:

## Step 3: Running the Model
Import the necessary libraries and load your dataset:
python
Copy code
import pandas as pd
df = pd.read_csv('recode.csv')
Train the model using machine learning techniques. An example command to fit a Random Forest model could be:
python
Copy code
from sklearn.ensemble import RandomForestRegressor
model = RandomForestRegressor()
model.fit(X_train, y_train)
