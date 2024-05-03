PARKING SPOT PREDICTOR
![image](https://github.com/stephaniemwai/Group-10-Capstone-Project/assets/143871178/dd0df8fa-4db5-4012-862a-af713bc134ba)

PROJECT OVERVIEW

Using data analytics and machine learning techniques, we explore the field of parking prediction and urban mobility. Our research develops a state-of-the-art algorithm that can effectively estimate parking spot availability in metropolitan locations by utilizing real-time parking occupancy data from several sources inclusive of historical records. We welcome you to journey with us as we explore the inner workings of our prediction model, emphasize significant discoveries, and demonstrate how it may revolutionize urban parking system optimization.

Preliminaries
As this project was a group project, the contributors to this work are as follows:
 Joylene Cherono
 Stephanie Mwai
 James Nyamu
 Prscilla Nzula
 Clare Gatambia

Table of contents

  Business Understanding
  Data Sourcing
  Data Understanding
  Data Preprocessing
  Exploratory Data Analysis
  Modelling
  Deployment
  Conclusion and Recommendation
  Next-Steps
Business Understanding

Finding a parking place in the busy urban environments of major cities throughout the world is a problem that worries locals, commuters, and tourists equally. The need for effective parking solutions is greater than ever due to the fast urbanization, rising traffic, and expanding population. Our initiative is to change parking management in metropolitan areas confronting comparable difficulties throughout the globe by utilizing data-driven insights in response to this urgent issue. It is impossible to exaggerate the significance of this endeavor for metropolitan areas. Urban centers are the epicenters of activity, drawing millions of people for business, pleasure, and employment because they are social, cultural, and economic magnets. Nonetheless, these cities' disorganized traffic and inadequate parking facilities provide serious difficulties for local government, companies, and citizens. Our initiative intends to improve urban mobility by reducing travel times, relieving traffic congestion, and offering accurate estimates of parking spot availability.

One of the key challenges lies in accessing reliable data on parking occupancy and usage patterns. Parking spaces in urban areas are often managed by various entities, including public agencies, private operators, and informal attendants, making data collection a complex and fragmented process. Moreover, concerns about data privacy and security have hindered efforts to gather comprehensive parking data, as authorities are cautious about disclosing sensitive information due to security reasons.

Despite these challenges, our project aims to collaborate with relevant stakeholders, including:

  City authorities: Vital for regulatory support, infrastructure planning, and policy implementation to enhance urban mobility and parking management.
  Parking operators: Key players responsible for managing parking facilities, providing valuable data, and implementing innovative solutions to optimize parking spot utilization.
  Technology partners: Essential for developing and implementing data-driven tools, such as predictive models and smart parking systems, to improve parking availability and streamline operations.
  Motorists (end-users): The primary beneficiaries of improved parking management solutions, as they will benefit from reduced search time, enhanced convenience, and better access to parking spots.

By fostering partnerships and promoting transparency, we seek to establish a data-sharing framework that respects privacy concerns while enabling the development of innovative solutions to improve parking management in urban centers worldwide. Optimizing parking and reducing congestion, enhances business efficiency, attracts investments, and stimulates economic activity. Encouraging alternative transportation modes reduces emissions and contributes to environmental conservation. Through data analytics, stakeholder collaboration, and innovative tech, we aim to create smarter, more efficient urban mobility ecosystems benefiting all.

Problem Statement

The absence of accurate and up-to-date data on parking spot availability not only impedes the development of effective predictive models but also limits the implementation of innovative solutions aimed at addressing urban mobility challenges. Without access to comprehensive data sources, parking prediction systems struggle to provide reliable real-time information, leading to suboptimal parking decisions and increased traffic congestion. Overcoming these challenges is crucial for creating a parking prediction system that not only improves parking navigation but also contributes to the overall sustainability and livability of urban areas by enhancing economic productivity, and fostering a more seamless urban mobility experience for all stakeholders.

Objectives
Main Objective

Develop a robust time series-based parking spot predictor that accurately forecasts parking spot availability in urban areas, leveraging historical parking data and real-time variables.
Other Objectives

    To collect and preprocess historical and parking data from various sources and integrate relevant time-varying features, such as time of day, day of the week, and holidays into the data.
    To understand the distribution of both numerical columns (capacity, occupancy) and categorical columns (is_holiday) in our data.
    To analyze the monthly and daily average occupancy and average parking availability across all parking facilities, identifying patterns and trends over time.
    To investigate the impact of holidays and time on parking availability, examining how these factors influence parking spot occupancy and demand.
    To explore various time series forecasting techniques, including ARIMA, XGBoost, and Prophet and evaluate the performance of each technique using metrics like MAE, MSE and RMSE.
    To develop and deploy a user-friendly interface that allows motorists to access real-time parking predictions and navigate to available parking spots efficiently.

Data Understanding

The dataset used for this project is available in the data directory. It includes historical information about parking lot occupancy, date, time location, and other relevant features.

Our main data was sourced from the Transport for New South Wales(TfNSW) website, more speficially, from their Car Park API.

The holiday data was scrapped from National Holidays in Australia in 2023.

Exploratory Data Analysis (EDA)

Analysis and visualization of data to understand its characteristics, patterns, and potential insights is done in this section. Histograms, kernel density plots, and box plots are used to understand the distribution of numerical variables and count plot for categorical variables. On bivariate analysis, relationships between pairs of variables are explored and visualized using bar plots, line plot and correlation heatmap. On multivariate analysis, parking availability patterns across different days of the week and times of the day are visualised using a heatmap
Modelling

Time series modeling is done using the following three models:- ARIMA to capture linear patterns, Prophet designed for seasonality and holidays, and XGBoost, a versatile ensemble method, to capturing complex non-linear relationships in time series data. Prophet model outperformed the rest of the models and was implemented and the final model.
Deployment (Streamlit)

Deployment using Streamlit was done to turn the data-driven Python script into an interactive user interface that allows the end user to select a parking facility and a prospective date. The output given is a predicted number of available parking spots for the given facility at the selected day.
Future Steps

    To implement a real-time data acquisition pipeline to continuously update the model with the latest parking occupancy data.

    To conduct pilot tests and gather feedback from end-users to assess the usability and effectiveness of the parking prediction system in real-world scenarios.

    To deploy the finalized parking spot predictor in urban areas, collaborating with city authorities and parking management companies to integrate it into existing infrastructure and promote widespread adoption.



