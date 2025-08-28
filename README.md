# Food_Delivery_Demand_Forecasting_21 CaseCraft Analytics Project Sprint Project 21


## 🍔 Overview  
This project forecasts food delivery demand using synthetic order data enriched with timestamps, geolocation, promo flags, and delivery metrics. It blends time series decomposition, geospatial heatmaps, and regression modeling to optimize fleet planning and promotional strategy.

## 🎯 Objective  
To analyze hourly order volume, promo impact, and delivery time patterns, and build a predictive model for delivery duration.

## 🗺️ Dataset & Features  
- Orders: 1,000 synthetic entries  
- Features:  
  - `order_time`: hourly timestamp  
  - `location_lat`, `location_lon`: geospatial coordinates  
  - `promo_applied`: binary flag  
  - `delivery_time`: minutes  
  - `order_value`: ₹ amount  
  - Derived: `hour` of day

## 📊 Visual Explorations  
- **Line Plot**: Hourly order volume  
- **Heatmap**: Geospatial density of orders  
- **Boxplot**: Delivery time with vs without promo  
- **Scatterplot**: Order value vs delivery time  
- **Histogram**: Delivery time distribution  
- **Bar Chart**: Promo usage rate by hour  
- **Line Plot**: Average delivery time by hour  
- **Heatmap**: Feature correlations

## 🤖 Predictive Modeling  
- **Model**: Random Forest Regressor  
- **Features**: `order_value`, `promo_applied`, `hour`  
- **Target**: `delivery_time`  
- **Performance**:  
  - Mean Absolute Error: **8.70 minutes**

## 🧠 Key Insights  
1. **Hourly Demand**: Peaks between 7 PM and 10 PM  
2. **Promo Timing**: Usage spikes around lunch (1 PM) and dinner (8 PM)  
3. **Delivery Impact**: Promo orders show slightly longer delivery times  
4. **Spatial Clustering**: Dense order zones near commercial areas  
5. **Predictive Utility**: Hour of day is the strongest predictor of delivery time  
6. **Operational Leverage**: Promo and time-based insights support fleet allocation

## ✅ Final Conclusion  
Food delivery demand follows clear temporal and spatial patterns. Promo campaigns influence both volume and delivery speed. This framework enables predictive delivery time estimation, surge planning, and promo optimization—ideal for logistics and marketing teams.