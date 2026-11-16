# Indian Airlines Data Analysis Report ✈️📊

## 📌 Project Overview
This project analyzes a dataset of 300,153 domestic flights across six major Indian metropolitan hubs. The resulting Power BI dashboard visualizes the aviation market's unit economics, operational bottlenecks, and customer behavioral pricing models. The insights extracted from this data are structured to serve as the foundational logic for dynamic pricing algorithms and operational routing strategies.

## 📊 Dataset Profile
* **Records:** 300,153 verified flight logs
* **Scope:** 6 Airlines (Vistara, Air India, Indigo, SpiceJet, GO FIRST, AirAsia) across 6 Tier-1 Cities (Delhi, Mumbai, Bangalore, Kolkata, Hyderabad, Chennai).
* **Data Points Analyzed:** Airline, Flight ID, Source/Destination, Departure/Arrival Times, Stops, Class, Flight Duration, Days Left (Booking Window), and Ticket Price.

## 🏗️ Dashboard Architecture
The dashboard is separated into three highly focused analytical workflows:

### 1. Market & Financial Overview
*Analyzes high-level revenue generation and market distribution.*
* **KPIs:** Total Volume, Average Economy vs. Business Fares, Global Route Footprint.
* **The 80/20 Revenue Rule:** Visualizes how Business Class, despite being a fraction of total volume, captures over ~78% of the gross ticket revenue.
* **Market Share:** Contrasts volume-heavy budget carriers (Indigo) against premium-margin full-service carriers (Vistara/Air India).

### 2. Dynamic Pricing & Fare Analysis
*Analyzes the mathematical triggers that cause ticket prices to fluctuate.*
* **The Surge Pricing Curve:** A time-series analysis mapping average price against the days left to departure, revealing the exact day thresholds where automated pricing algorithms trigger aggressive fare hikes.
* **Time To Cost:** A scatter plot matrix evaluating the financial discount passengers receive for enduring longer flight durations.
* **Convenience Premiums:** Quantifies the price variance across specific departure windows (e.g., Morning vs. Red-Eye flights).

### 3. Operations & Logistics
*Analyzes physical routing, operational efficiency, and fleet deployment.*
* **Route Traffic Hub Matrix:** A heatmap highlighting the heaviest corridors of air traffic and the most lucrative city pairings.
* **Fleet Operational Speed:** Evaluates the average flight durations across competing airlines to measure routing efficiency.
* **Hub-and-Spoke vs. Point-to-Point:** Evaluates which airlines rely heavily on single/multi-stop layovers versus direct point-to-point routing.

## 💡 Key Business Insights
1. **The Premium Monopoly:** Only two carriers (Vistara and Air India) compete in the Business Class sector, allowing them to capture the vast majority of high-margin market revenue.
2. **Volume vs. Value:** Indigo dominates the market in sheer operational scale but operates strictly within the highly competitive, lower-margin economy tier. 
3. **Surge Thresholds:** There is a distinct, predictable mathematical decay in purchasing power around the 15-day booking window, which can be extracted to train predictive pricing RESTful APIs.

## 🛠️ Tech Stack & Methodologies
* **Data Visualization:** Power BI (Dashboards, Custom Visuals, Heatmaps)
* **Data Modeling:** DAX (Custom Measures, Aggregations, Filtering Logic)
* **Data Cleaning & Profiling:** Python (Pandas)

## 🚀 How to Run Locally
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Jitendra2103/Airline-Anaylysis.git
