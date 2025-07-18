# 🧳 Agentic AI Travel Assistant with CrewAI

An intelligent multi-agent system that automates personalized travel planning using [CrewAI](https://docs.crewai.com/). This assistant retrieves real-time data on flights, hotels, and weather, and generates a detailed, customized itinerary using APIs like Amadeus, OpenWeather, and HotelBeds.

## 🚀 Features

- 🔍 **Flight Search**: Fetches best flight options using Amadeus API.
- 🏨 **Hotel Recommendations**: Lists suitable hotels with ratings and pricing using HotelBeds API.
- 🌤 **Weather Forecast**: Provides weather insights for the destination via OpenWeather API.
- 🧠 **Itinerary Generation**: Crafts a detailed day-by-day travel plan combining all data sources with cultural tips, activity suggestions, and packing advice.

## 🧠 Tech Stack

- **CrewAI** – Agent orchestration and task management  
- **Python** – Core scripting language  
- **APIs** – Amadeus (flights), HotelBeds (hotels), OpenWeather (weather)  
- **Libraries** – `requests`, `tenacity`, `hashlib`, `datetime`, `json`, `os`

## 🛠️ Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/your-username/Agentic-AI-Travel-Assistant-with-CrewAI.git
cd Agentic-AI-Travel-Assistant-with-CrewAI
pip install crewai openai requests amadeus tenacity 
```

## 🔑 Environment Variables

Set up the following API keys as environment variables. You can use a .env file or export them manually in your shell:

```bash
export OPENAI_API_KEY="your_openai_api_key"
export AMADEUS_CLIENT_ID="your_amadeus_client_id"
export AMADEUS_CLIENT_SECRET="your_amadeus_client_secret"
export OPENWEATHER_API_KEY="your_openweather_api_key"
export HOTELBEDS_API_KEY="your_hotelbeds_api_key"
export HOTELBEDS_SECRET="your_hotelbeds_secret"
```
## 🧭 How to Run

1. Clone the repo
2. Install dependencies (CrewAI, requests, OpenAI, etc.)
3. Export necessary environment variables
4. Launch the notebook:

```bash
jupyter notebook main.ipynb
```


## 📊 Sample Output
```bash
TRIP 1: San Francisco to Rome
────────────────────
✔️ Flights found
✔️ Weather forecast ready
✔️ Hotels listed
✔️ Itinerary created!

🗓️ Day 1:
- Flight: Lufthansa LH459: 2025-08-10 13:00 → 2025-08-11 08:00
- Weather: 27°C, clear sky
- Hotel: Hotel Artemide
- Morning: Colosseum tour
- Afternoon: Lunch at Trastevere
- Evening: Tiber River walk + wine tasting
...
```


## 🌍 Future Improvements

- Add Streamlit-based UI
- Persist recommendations to a database
- Add more tools (e.g., local events, restaurant planner)

## 📌 License

This project is for demonstration and academic purposes only.
