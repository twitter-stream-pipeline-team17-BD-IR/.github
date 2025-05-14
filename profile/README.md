<p align="center"> # 🌟 TweetStream Analytics Hub </p>

**Where Tweets Meet Technology** 🚀  
Real-time Twitter analytics using big data processing, sentiment analysis, and interactive visualizations.

---

## 🌍 Project Mission

To analyze and understand Twitter in real time by:

- Capturing live tweet streams
- Extracting hashtags and analyzing sentiment
- Storing data in a queryable format
- Visualizing insights through an interactive web interface

---

## 🔧 Overview

This project builds a real-time tweet analytics pipeline using cutting-edge tools:

- **Apache Kafka** – Real-time data streaming
- **Apache Spark** – Scalable processing & sentiment analysis
- **Elasticsearch** – Fast search and geospatial indexing
- **FastAPI** – Lightweight and powerful API service
- **React.js** – Interactive and responsive frontend
- **Leaflet.js** – Maps for geo-tagged tweets

---

## 🧱 System Components

### 1. **StreamProducer**
- Streams real or simulated tweet data to a Kafka topic.
- Reads geolocated tweets from JSON files.

### 2. **StreamConsumer**
#### a. Filter Consumer
- Consumes raw tweets from Kafka.
- Extracts text, hashtags, timestamp, and geo-coordinates.

#### b. Sentiment Analysis Consumer
- Performs sentiment analysis using Spark NLP or TextBlob.
- Classifies tweets as `Positive`, `Negative`, or `Neutral`.

### 3. **ElasticsearchManager**
- Manages index creation and data storage in Elasticsearch.
- Enables search by keyword, time, hashtag, and location.

### 4. **APIServices (FastAPI)**
- Provides RESTful APIs to fetch:
  - Tweets by keyword
  - Sentiment scores
  - Hashtag trends
  - Date-range and location-based analytics

### 5. **Frontend (React.js)**
- Real-time data visualization with:
  - 🗺️ Interactive tweet map (Leaflet)
  - 📈 Time-based trend charts (hourly/daily)
  - 😊 Sentiment gauge
  - 🔍 Search by keyword or hashtag

---

## 🗃️ Project Structure

| Module                 | Description                                                |
|------------------------|------------------------------------------------------------|
| `ElasticSearchManager` | Handles indexing and querying tweet data in Elasticsearch  |
| `StreamProducer`       | Sends tweet data into Kafka                                |
| `StreamConsumer`       | Filters and enriches tweets with sentiment info            |
| `Website`              | React-based web dashboard                                  |
| `APIServices`          | FastAPI backend to serve tweet analytics                   |


---

## 🔍 UI Preview

### 🏠 Home Page
- Search bar for querying tweets
- Summary of latest trends and sentiments

### 🗺️ Map Page
- Tweets displayed on an interactive map using geo-coordinates

---

## 🛠️ Prerequisites

Make sure the following are installed:

- Apache Kafka
- Apache Spark
- Elasticsearch (version 7.x or higher)
- Python 3.8+
- Node.js & npm (for React frontend)
- Docker (optional for Elasticsearch and Kafka setup)

---


