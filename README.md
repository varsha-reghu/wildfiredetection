# wildfiredetection

# 🔥 AI-Based Environmental Disaster Prediction and Monitoring System

**Project Title:** A Case Study on California Wildfire Detection Using Satellite Imagery  
**Group 13 Members:**
- Ashish Thannivilayil Monachen (100915700)
- Renya Ann Regi (100918535)
- Rini Issac (100939351)
- Varsha Reghu (100930107)

---

## 📌 Project Overview

Wildfires are among the most devastating environmental disasters, with increasing frequency due to climate change. Traditional methods for wildfire detection are slow, reactive, and often lack real-time precision.

This project introduces **an AI-powered wildfire detection system** that uses **Convolutional Neural Networks (CNN)** to classify satellite images into wildfire or non-wildfire zones. It also integrates structured wildfire data to enhance contextual awareness and deploys predictions on an **interactive Streamlit dashboard**.

---

## 🎯 Key Features

- 🛰️ Satellite image-based wildfire classification (using CNN)
- 📈 Real-time dashboard for fire status and location tracking
- 📍 Geospatial mapping with wind direction, area burned, and emergency services
- 📁 Outputs stored in structured CSV for downstream integration
- 💡 Future expansion using LSTM (time-series weather data) and NLP (social media sentiment)

---

## 🛠 Technologies Used

- **Deep Learning**: CNN (Keras + TensorFlow)
- **Data Processing**: Pandas, NumPy, OpenCV
- **Visualization**: Streamlit, Folium, Leaflet.js
- **Notebook Development**: Jupyter, Google Colab
- **Dataset Sources**:
  - Satellite images (3,000 images, balanced)
  - California Wildfire CSV (100,230+ records from Kaggle)

---

## 🧪 Model Architecture

- **Input**: 224x224 RGB satellite image
- **CNN Layers**: 32 → 64 → 128 filters (3x3 kernel), with MaxPooling and ReLU
- **Dropout**: 0.25 for regularization
- **Dense Layers**: Fully connected, ending in sigmoid (binary classification)
- **Accuracy Achieved**: **91.3%**

---

## 🧾 Output

- **archive_fire.csv** includes:
  - Latitude, Longitude
  - Fire Name
  - Area Burned
  - Fire Status (Active/Not Active)
  - Wind Direction
  - Containment Level

These outputs feed into the Streamlit app for interactive map display and fire risk monitoring.

---

## 📊 Dashboard Features

- **Map Overlay**: Color-coded markers (red = active fire, green = safe)
- **Info Pop-ups**: Fire name, date, burn area, wind details
- **Satellite View Toggle**
- **Nearby Services**: Hospitals, fire stations
- **Live Geolocation Plotting**: Real-time feed from predictions

---

## 🧠 Future Enhancements

- 🔄 LSTM for weather-based fire spread prediction
- 💬 NLP sentiment analysis from Twitter & emergency alerts
- 🌐 Multispectral and thermal image support
- ☁️ Full cloud deployment on AWS or GCP for 24/7 monitoring

---

## 📌 Limitations

- Generalizability to other regions not validated yet
- Cloudy images may reduce classification confidence
- No direct real-time satellite feed integration (yet)

---

## 🌍 Ethical Considerations

- ✅ Fairness: Train on diverse regions
- ✅ Transparency: Model logic should be interpretable
- ✅ Privacy: Anonymize all public social signals
- ✅ Accountability: Human review is necessary for alerts

---

## 📂 Folder Structure (Expected)

```
wildfire_project/
├── wildfire.ipynb            # Core training and prediction notebook
├── archive_fire.csv          # Output predictions for dashboard
├── requirements.txt          # Python dependencies
├── streamlit_app.py          # Streamlit dashboard logic
├── images/                   # Wildfire / Non-wildfire image datasets
└── README.md                 # Project documentation
```

---

## 🔗 Useful Links

- 📁 **Dataset**: [Kaggle Wildfire Dataset](https://www.kaggle.com/datasets/vijayveersingh/the-california-wildfire-data)  
- 🛰️ **ESA Sentinel-2**: [ESA Earth Observation](https://www.esa.int/Applications/Observing_the_Earth/Copernicus/Sentinel-2)  
- 🚀 **Colab Notebook**: [Google Colab Link](https://colab.research.google.com/drive/1rtT7iq6w4GTAnJo44dRJIEMVtVBoyjhv#scrollTo=Z13-QMTLeZdD)

---

## 👥 Contributors

- Ashish T. Monachen — Model Development
- Renya Ann Regi — Frontend and Integration
- Rini Issac — Data Curation and Dashboard
- Varsha Reghu — Report and Visualization Design

---

## 📃 License

This project is for academic purposes and may be adapted under the MIT License with proper citation.

