# AgriSmart – AI-Powered Agricultural Intelligence Platform

**Client: Syngenta**

AgriSmart is an intelligent, integrated agricultural solution designed to support modern farming decisions using AI and data-driven predictions. This project was built specifically for Syngenta to enhance crop monitoring, disease diagnosis, weather forecasting, and future price prediction using scalable cloud deployment.

---

## 🌿 Features

### 1. 🌱 Leaf Disease Detection
- Detects common plant leaf diseases using deep learning.
- Input: Image of plant leaf.
- Output: Disease classification and treatment suggestions.

### 2. 🍅 Tomato Fruit Disease Detection
- Identifies diseases like early blight, late blight, and bacterial spot.
- Uses convolutional neural networks (CNNs) for accurate detection.

### 3. 🌦️ Weather Forecasting
- Provides localized, short-term weather forecasts.
- Helps farmers plan irrigation and harvesting efficiently.

### 4. 📈 Future Price Prediction (Tomatoes)
- Predicts tomato market prices using time series models.
- Supports better decision-making on storage and selling time.

---

## ⚙️ Technologies Used

| Area                        | Technology                          |
|-----------------------------|--------------------------------------|
| Backend                     | Python, FastAPI                     |
| Machine Learning            | TensorFlow, scikit-learn, OpenCV    |
| Deep Learning Models        | CNNs for image classification       |
| Time Series Forecasting     | ARIMA, LSTM                         |
| Weather API Integration     | OpenWeatherMap API                  |
| Deployment                  | **AWS EC2**                         |
| Containerization            | **Docker**, Docker Hub Registry     |

---

## 🚀 Deployment Architecture

1. Application is containerized using Docker.
2. Docker images are pushed to **Docker Hub**.
3. Deployed and managed on **AWS EC2** instance.
4. API endpoints are exposed via FastAPI for:
   - Image uploads
   - Forecast results
   - Model predictions

---

## 🧪 How to Use

### Option 1: Clone and Run Locally
```bash
git clone https://github.com/Prerna-lily/agrismart_syngenta.git
cd agrismart_syngenta
docker build -t agrismart .
docker run -p 8000:8000 agrismart
