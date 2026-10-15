# Airport Congestion Analysis: King Khalid International Airport (KKIA)

An Power BI dashboard that analyzes flight movements at King Khalid International Airport (RUH / OERK) in Riyadh to identify when and where congestion happens, and to recommend ways to reduce it.

## Business Problem

Congestion at KKIA affects passengers (waiting times, delays), airlines (schedule management), and airport operations (pressure on terminals and gates). This project uses flight data to find the main drivers of congestion: flights per hour, per terminal, per airline, and per destination.

## Dataset

- **Source:** [King Khalid International Airport Flights Dataset](https://www.kaggle.com/datasets/mohammedalsubaie/king-khalid-international-airport-flights-dataset/data) on Kaggle
- **Size:** 153,308 scheduled flight movements, 23 columns
- **Coverage:** arrivals and departures, 68 airlines
- **Preparation:** the flight files were combined from a folder and column types were set in Power Query. Hours are derived from the scheduled time in UTC.

The dataset is not included in this repository. Download it from the Kaggle link above.

## Dashboard

The Power BI report (`flights.pbix`) includes visuals for:

- Flight count per hour (congestion analysis)
- Flights per destination
- Flights per airline
- Terminal distribution

## Key Findings

- **Peak hours:** congestion is highest between **16:00 and 20:00 (UTC)**.
- **Terminal load:** Terminal 5 handles about 53% of all flights (around 81K of 153K).
- **Airline concentration:** Saudi Arabian Airlines, flynas, and flyadeal operate about 78% of all flights.
- **Top destinations:** Jeddah leads by a wide margin, followed by Dubai, Cairo, Abha, and Dammam.
- **Seasonality:** the initial data analysis shows flight volume rising in the summer months (June to August).

## Recommendations

1. Distribute flight schedules more evenly across the day.
2. Rebalance flights across terminals to relieve Terminal 5.
3. Improve gate and staff allocation using predictive analytics and real-time data.
4. Give airlines real-time visibility into terminal crowd levels and gate availability.
5. Plan extra staffing and counters for seasonal demand peaks.

## Tools

Power BI (Power Query, DAX)

## How to Open

The `flights.pbix` file in this repository is saved **without data**.

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Windows).
2. Download the dataset files from Kaggle and place them in a local folder.
3. Open `flights.pbix`, then go to **Transform data > Data source settings** and point the data source to that folder.
4. Click **Refresh** to load the data.
