# LTA Hackathon Repository

 This repository contains curated datasets and resources for participants working on various problem statements related to Land Transport Authority (LTA) hackathon

## 📋 Table of Contents

- [Overview](#overview)
- [Repository Structure](#repository-structure)
- [Problem Statements](#problem-statements)
  - [Problem Statement 1](#problem-statement-1-ps1)
  - [Problem Statement 2](#problem-statement-2-ps2)
  - [Problem Statement 3](#problem-statement-3-ps3)
- [LTA DataMall API](#lta-datamall-api)
- [Getting Started](#getting-started)
- [Data Formats](#data-formats)
- [Resources](#resources)

---

## 🎯 Overview

This repository provides organized datasets for hackathon participants to build innovative solutions for Singapore's public transport challenges. Each problem statement folder contains relevant data sources to help you get started quickly.

---?

## 📁 Repository Structure

```
Hackathon-Repo/
├── PS1/                          # Problem Statement 1 Datasets
│   ├── 24hourWeatherForecast.json
│   ├── 4dayWeatherForecast.json
│   └── [Maintenance Scheduler Data - Encoded]
│
├── PS2/                          # Problem Statement 2 Datasets
│   ├── 24hourWeatherForecast.json
│   ├── 4dayWeatherForecast.json
│   ├── AmendmenttoMP2014RailStation.geojson
│   └── UsefulWebsites.txt      
│
├── PS3/                          # Problem Statement 3 Datasets
│   └── [To be determined]
│
└── LTA_DataMall_API_User_Guide.pdf
```

---

## 🚀 Problem Statements

### Problem Statement 1 (PS1)

**Focus Area:** AI Maintenance Scheduling

#### Available Datasets:
- **Weather Forecast Data**
  - `24hourWeatherForecast.json` - Hourly weather predictions for the next 24 hours
  - `4dayWeatherForecast.json` - Extended weather forecast for 4 days ahead
  
- **Maintenance Scheduler Data** *(Encoded)*
  - Contains start and end dates for various system maintenance schedules
  - Data is encoded and requires processing

#### Use Cases:
- Predictive maintenance scheduling based on weather conditions
- Service disruption planning
- Resource allocation optimization
- Weather-dependent operational adjustments

---

### Problem Statement 2 (PS2)

**Focus Area:** Train Disruption Management

#### Available Datasets:
- **Rail Infrastructure**
  - `AmendmenttoMP2014RailStation.geojson` - GeoJSON data of rail stations with amendments to Master Plan 2014
  
- **Weather Data**
  - `24hourWeatherForecast.json` - Short-term weather predictions
  - `4dayWeatherForecast.json` - Medium-term weather forecast
  
- **Live Updates**
  - `UsefulWebsites.txt` - Links to Telegram channels with real-time updates on:
    - Train faults
    - Service delays
    - Operational disruptions
    - Emergency notifications

#### Telegram Data Source:
- **SGMRT Telegram Channel**: [https://t.me/s/sgmrt](https://t.me/s/sgmrt?before=2527)
  - Real-time updates on MRT/LRT service status
  - Fault reports and delay notifications
  - Historical data available through message archives

#### Use Cases:
- Real-time incident detection and response
- Passenger information systems
- Service reliability analysis
- Predictive delay modeling
- Integration of weather impact on rail operations

---

### Problem Statement 3 (PS3)

**Focus Area:** *To Be Determined*

#### Status:
Datasets for Problem Statement 3 are currently being finalized. Check back for updates!

---

## 🔌 LTA DataMall API

All participants have access to the **LTA DataMall API** for real-time transport data.

### 📖 Documentation
Refer to `LTA_DataMall_API_User_Guide.pdf` for comprehensive API documentation.

### 🌐 API Base URL
```
https://datamall2.mytransport.sg/ltaodataservice/
```

### 🔑 Getting Started with the API

1. **Register for API Access**
   - Visit [LTA DataMall](https://datamall.lta.gov.sg/content/datamall/en.html)
   - Create an account and obtain your API key (AccountKey)

2. **Available Endpoints** (Examples)
   - **Bus Arrival**: `v3/BusArrival?BusStopCode={code}`
   - **Bus Services**: `BusServices`
   - **Bus Stops**: `BusStops`
   - **Bus Routes**: `BusRoutes`
   - **Taxi Availability**: `Taxi-Availability`
   - **Traffic Incidents**: `TrafficIncidents`
   - And many more...

3. **Sample API Call**

   **Using cURL:**
   ```bash
   curl -X GET "https://datamall2.mytransport.sg/ltaodataservice/v3/BusArrival?BusStopCode=83139" \
     -H "AccountKey: YOUR_API_KEY_HERE"
   ```

### 📊 Real-Time Data Available:
- Bus arrival times
- Bus services and routes
- Bus stop locations
- Taxi availability
- Carpark availability
- Traffic incidents
- Road works
- Traffic speed bands
- And more...


## 📄 Data Formats

### JSON Files
- Weather forecast data in standard JSON format
- Structured with metadata and value arrays
- Timestamps in ISO 8601 format

### GeoJSON Files
- Rail station data with geographic coordinates
- Compatible with mapping libraries (Leaflet, Mapbox, Google Maps)
- Contains feature properties and geometry

### API Responses
- JSON format with OData metadata
- Paginated results for large datasets
- Real-time data with timestamps

---

## 📚 Resources

### Official Documentation
- [LTA DataMall Portal](https://datamall.lta.gov.sg/content/datamall/en.html)
- [LTA DataMall API User Guide](./LTA_DataMall_API_User_Guide.pdf)
- [Data.gov.sg](https://data.gov.sg/) - Singapore's open data portal with additional transport, weather, and infrastructure datasets

### Live Data Sources
- [SGMRT Telegram Channel](https://t.me/s/sgmrt) - Real-time MRT/LRT updates

### Useful Tools
- **JSON Viewers**: [jsonviewer.stack.hu](http://jsonviewer.stack.hu/)
- **GeoJSON Viewers**: [geojson.io](http://geojson.io/)
- **API Testing**: [Postman](https://www.postman.com/), [Insomnia](https://insomnia.rest/)
- **

### Weather Data Sources
- Singapore Meteorological Service
- NEA Weather API (if applicable)

---

## 💡 Tips for Participants

1. **Start with the API**: Familiarize yourself with the LTA DataMall API early
2. **Understand the Data**: Spend time exploring the dataset structures
3. **Think Real-time**: Consider how to integrate live data feeds
4. **Weather Integration**: Many problems benefit from weather correlation
5. **User-Centric**: Focus on solving real commuter pain points
6. **Scalability**: Design solutions that can handle Singapore's transport scale

---

## 🤝 Support

For questions about:
- **Datasets**: Review the data files and API documentation
- **API Access**: Visit [LTA DataMall Support](https://datamall.lta.gov.sg/content/datamall/en/contact-us.html)
- **Problem Statements**: Consult with hackathon organizers

---

## 📝 License

Please refer to LTA DataMall's terms of use for API data usage guidelines.

---

## 🎉 Good Luck!

We're excited to see what innovative solutions you'll build with these datasets. Happy hacking! 🚀

---

