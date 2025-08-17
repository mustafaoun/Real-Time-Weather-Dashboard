# Real-Time Weather & AQI Dashboard

This project is a dynamic and interactive **Power BI dashboard** designed to provide real-time weather and air quality (AQI) data for major cities in Egypt. This repository serves as a comprehensive guide to the project, demonstrating the end-to-end process of data integration, transformation, and visualization. You can use this documentation to replicate the dashboard yourself. A video demonstration of the dashboard in action has been uploaded to this repository for a quick overview.

---

## 📊 Features

- **Live Data:** Fetches real-time weather and AQI data from a public API.  
- **Interactive Controls:** Users can select different cities to view data, and interactive charts allow for deep dives into specific metrics.  
- **Intuitive Design:** The dashboard uses conditional formatting and clear visualizations to make data easy to understand.  
- **Video Demo:** A short video is available in the repository to provide a visual walkthrough of the dashboard's features and interactivity.  
- **Scalable Architecture:** The data model and DAX measures are structured to be easily expanded to include more cities or different data points.  
- **Comprehensive Metrics:** Displays key weather information (temperature, wind speed, humidity, etc.) and multiple air quality indicators (PM2.5, CO, NO2, SO2).  

---

## 🛠️ Technologies & Skills

- **Power BI:** Used for the entire dashboard creation, from data sourcing to visualization.  
- **Power Query:** Leveraged extensively for connecting to the API, parsing JSON, and transforming raw data.  
- **DAX (Data Analysis Expressions):** Utilized for creating custom measures and conditional formatting rules to add dynamic behavior to the visualizations.  
- **API Integration:** Successfully established a data connection to a third-party REST API.  
- **Data Modeling:** Structured the data into a star schema with separate fact and dimension tables.  

---

## ⚙️ How It Works

### Data Sourcing
The dashboard connects to **WeatherAPI.com** via its REST API, which provides weather and AQI data for various locations in JSON format.

### Data Transformation
Power Query takes the raw JSON data and performs a series of cleaning and shaping steps:

- Parsing the JSON structure to extract relevant data points.  
- Splitting the data into two main tables: a **Current Weather** table and a **Forecast** table.  
- Creating columns for key metrics like temperature, humidity, wind, and various air pollutants.  

### Data Modeling
The cleansed data tables are loaded into the Power BI data model. The data is modeled to allow for seamless relationships between the tables, making it easy to filter and analyze.

### Visualization & Analysis
Interactive visualizations like slicers, cards, gauges, and line charts are used to display the data. DAX is used to write measures for dynamic calculations and to apply conditional formatting based on weather conditions or AQI levels.

---

## 🚀 Getting Started

To replicate this project, you will need **Power BI Desktop**.

1. **Get Your API Key:** You'll need a free API key from [WeatherAPI.com](https://www.weatherapi.com/).  
2. **Open Power BI Desktop:** Create a new, blank report.  
3. **Connect to Web Data:** Use the **Get Data > Web** option to connect to the WeatherAPI using the appropriate URL and your new API key.  
4. **Follow the How It Works section:** Use the steps outlined above to replicate the data transformation, data modeling, and visualization steps to build your own dashboard.  
5. **Refresh Data:** Refresh the data to pull in live information.  

---

## ⏭️ Future Enhancements

- **Historical Data:** Implement a data collection system (e.g., using Python scripts and a database) to store historical data and enable trend analysis.  
- **Alerting System:** Add an automated email or notification system to alert users when AQI levels in a specific city exceed a certain threshold.  
- **Expanded Forecast:** Extend the forecast to cover more than just a few days, providing a long-term outlook.  

---

## 📄 License

This project is licensed under the **[Apache License](https://www.apache.org/licenses/LICENSE-2.0)**.

If you want, I can also make a **slimmer, GitHub-ready version** with badges, a table of contents, and direct links for video and API references to make it look more professional. Do you want me to do that?
